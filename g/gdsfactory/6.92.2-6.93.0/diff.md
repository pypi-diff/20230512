# Comparing `tmp/gdsfactory-6.92.2.tar.gz` & `tmp/gdsfactory-6.93.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsfactory-6.92.2.tar", last modified: Wed May 10 22:43:26 2023, max compression
+gzip compressed data, was "gdsfactory-6.93.0.tar", last modified: Thu May 11 23:08:15 2023, max compression
```

## Comparing `gdsfactory-6.92.2.tar` & `gdsfactory-6.93.0.tar`

### file list

```diff
@@ -1,684 +1,684 @@
--rw-r--r--   0        0        0     1072 2023-05-10 22:43:04.989752 gdsfactory-6.92.2/LICENSE
--rw-r--r--   0        0        0    14281 2023-05-10 22:43:04.989752 gdsfactory-6.92.2/README.md
--rw-r--r--   0        0        0     3415 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/__init__.py
--rw-r--r--   0        0        0     2096 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/add_keepout.py
--rw-r--r--   0        0        0    12629 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/add_labels.py
--rw-r--r--   0        0        0     3711 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/add_loopback.py
--rw-r--r--   0        0        0     5054 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/add_padding.py
--rw-r--r--   0        0        0    15465 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/add_pins.py
--rw-r--r--   0        0        0    14700 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/add_ports.py
--rw-r--r--   0        0        0     2884 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/add_tapers.py
--rw-r--r--   0        0        0     2257 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/add_tapers_cross_section.py
--rw-r--r--   0        0        0     1831 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/add_termination.py
--rw-r--r--   0        0        0     1676 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/asserts.py
--rw-r--r--   0        0        0    11843 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/cell.py
--rw-r--r--   0        0        0    15946 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/circuitviz.py
--rw-r--r--   0        0        0     5325 2023-05-10 22:43:04.997753 gdsfactory-6.92.2/gdsfactory/cli.py
--rw-r--r--   0        0        0    99181 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/component.py
--rw-r--r--   0        0        0    23360 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/component_layout.py
--rw-r--r--   0        0        0    29699 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/component_reference.py
--rw-r--r--   0        0        0     1205 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/C.py
--rw-r--r--   0        0        0     1144 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/L.py
--rw-r--r--   0        0        0    20964 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/__init__.py
--rw-r--r--   0        0        0     2621 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/add_fiducials.py
--rw-r--r--   0        0        0    14087 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/add_grating_couplers.py
--rw-r--r--   0        0        0     2014 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/add_trenches.py
--rw-r--r--   0        0        0     3207 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/align.py
--rw-r--r--   0        0        0     2622 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/array_component.py
--rw-r--r--   0        0        0     4705 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/array_with_fanout.py
--rw-r--r--   0        0        0     4322 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/array_with_via.py
--rw-r--r--   0        0        0     4042 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/awg.py
--rw-r--r--   0        0        0     1269 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/bbox.py
--rw-r--r--   0        0        0     2851 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/bend_circular.py
--rw-r--r--   0        0        0     2649 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/bend_circular_heater.py
--rw-r--r--   0        0        0     7903 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/bend_euler.py
--rw-r--r--   0        0        0     2682 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/bend_port.py
--rw-r--r--   0        0        0     3664 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/bend_s.py
--rw-r--r--   0        0        0     5373 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/bezier.py
--rw-r--r--   0        0        0     1605 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/cavity.py
--rw-r--r--   0        0        0     5766 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/cdc.py
--rw-r--r--   0        0        0     2929 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/cdsem_all.py
--rw-r--r--   0        0        0     1788 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/cdsem_bend180.py
--rw-r--r--   0        0        0     1631 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/cdsem_coupler.py
--rw-r--r--   0        0        0     1412 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/cdsem_straight.py
--rw-r--r--   0        0        0     1565 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/cdsem_straight_density.py
--rw-r--r--   0        0        0      793 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/circle.py
--rw-r--r--   0        0        0     5722 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coh_rx_dual_pol.py
--rw-r--r--   0        0        0     8922 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coh_rx_single_pol.py
--rw-r--r--   0        0        0     5043 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coh_tx_dual_pol.py
--rw-r--r--   0        0        0     6118 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coh_tx_single_pol.py
--rw-r--r--   0        0        0     2548 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/compass.py
--rw-r--r--   0        0        0     9856 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/component_lattice.py
--rw-r--r--   0        0        0     7174 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/component_sequence.py
--rw-r--r--   0        0        0      812 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/copy_layers.py
--rw-r--r--   0        0        0     3460 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler.py
--rw-r--r--   0        0        0     2113 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler90.py
--rw-r--r--   0        0        0     1802 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler90bend.py
--rw-r--r--   0        0        0     4666 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler_adiabatic.py
--rw-r--r--   0        0        0     1909 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler_asymmetric.py
--rw-r--r--   0        0        0     3970 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler_full.py
--rw-r--r--   0        0        0     3414 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler_ring.py
--rw-r--r--   0        0        0     1060 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler_straight.py
--rw-r--r--   0        0        0     1164 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler_straight_asymmetric.py
--rw-r--r--   0        0        0     2192 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/coupler_symmetric.py
--rw-r--r--   0        0        0     1848 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/cross.py
--rw-r--r--   0        0        0    12873 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/crossing_waveguide.py
--rw-r--r--   0        0        0      500 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
--rw-r--r--   0        0        0     1014 2023-05-10 22:43:05.001752 gdsfactory-6.92.2/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
--rw-r--r--   0        0        0    19749 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
--rw-r--r--   0        0        0    19751 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
--rw-r--r--   0        0        0    19749 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
--rw-r--r--   0        0        0    19751 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
--rw-r--r--   0        0        0    19775 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
--rw-r--r--   0        0        0     3143 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
--rw-r--r--   0        0        0     5272 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/cutback_2x2.py
--rw-r--r--   0        0        0     6450 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/cutback_bend.py
--rw-r--r--   0        0        0     3765 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/cutback_component.py
--rw-r--r--   0        0        0     2721 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/cutback_splitter.py
--rw-r--r--   0        0        0     2971 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/dbr.py
--rw-r--r--   0        0        0     4288 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/dbr_tapered.py
--rw-r--r--   0        0        0     2486 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/delay_snake.py
--rw-r--r--   0        0        0     3177 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/delay_snake2.py
--rw-r--r--   0        0        0     3237 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/delay_snake3.py
--rw-r--r--   0        0        0     4319 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/delay_snake_sbend.py
--rw-r--r--   0        0        0     1226 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/dicing_lane.py
--rw-r--r--   0        0        0     3471 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/die.py
--rw-r--r--   0        0        0     2975 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/die_bbox.py
--rw-r--r--   0        0        0     2863 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/die_bbox_frame.py
--rw-r--r--   0        0        0     8015 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/disk.py
--rw-r--r--   0        0        0     4112 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/edge_coupler_array.py
--rw-r--r--   0        0        0     1214 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/ellipse.py
--rw-r--r--   0        0        0     1800 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/extend_ports_list.py
--rw-r--r--   0        0        0     7944 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/extension.py
--rw-r--r--   0        0        0      981 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/fiber.py
--rw-r--r--   0        0        0     1432 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/fiber_array.py
--rw-r--r--   0        0        0      722 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/fiducial_squares.py
--rw-r--r--   0        0        0     3290 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/ge_detector_straight_si_contacts.py
--rw-r--r--   0        0        0     1063 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_array.py
--rw-r--r--   0        0        0     4682 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_dual_pol.py
--rw-r--r--   0        0        0     7110 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_elliptical.py
--rw-r--r--   0        0        0     7221 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
--rw-r--r--   0        0        0     4960 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_elliptical_lumerical.py
--rw-r--r--   0        0        0     4592 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_elliptical_trenches.py
--rw-r--r--   0        0        0     1773 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_functions.py
--rw-r--r--   0        0        0     9058 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_loss.py
--rw-r--r--   0        0        0     1786 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_loss_fiber_single.py
--rw-r--r--   0        0        0     4142 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_rectangular.py
--rw-r--r--   0        0        0     4685 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
--rw-r--r--   0        0        0     3887 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
--rw-r--r--   0        0        0     1578 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/grating_coupler_tree.py
--rw-r--r--   0        0        0     8773 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/greek_cross.py
--rw-r--r--   0        0        0     1019 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/hline.py
--rw-r--r--   0        0        0     3687 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/interdigital_capacitor.py
--rw-r--r--   0        0        0     1825 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/litho_calipers.py
--rw-r--r--   0        0        0     1244 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/litho_ruler.py
--rw-r--r--   0        0        0     1304 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/litho_steps.py
--rw-r--r--   0        0        0      650 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/logo.py
--rw-r--r--   0        0        0     1679 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/loop_mirror.py
--rw-r--r--   0        0        0     3873 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mmi1x2.py
--rw-r--r--   0        0        0     2814 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mmi1x2_with_sbend.py
--rw-r--r--   0        0        0     3858 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mmi2x2.py
--rw-r--r--   0        0        0     3299 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mmi2x2_with_sbend.py
--rw-r--r--   0        0        0     4947 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mmi_90degree_hybrid.py
--rw-r--r--   0        0        0     3265 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mode_converter.py
--rw-r--r--   0        0        0     7414 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mzi.py
--rw-r--r--   0        0        0     2499 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mzi_arm.py
--rw-r--r--   0        0        0     5835 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mzi_arms.py
--rw-r--r--   0        0        0    12214 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mzi_lattice.py
--rw-r--r--   0        0        0     4025 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mzi_pads_center.py
--rw-r--r--   0        0        0     1064 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mzi_phase_shifter.py
--rw-r--r--   0        0        0     6342 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mzit.py
--rw-r--r--   0        0        0     3502 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mzit_lattice.py
--rw-r--r--   0        0        0     6047 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/mzm.py
--rw-r--r--   0        0        0     3518 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/nxn.py
--rw-r--r--   0        0        0     1940 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/optimal_90deg.py
--rw-r--r--   0        0        0     3876 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/optimal_hairpin.py
--rw-r--r--   0        0        0     6131 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/optimal_step.py
--rw-r--r--   0        0        0     6327 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/pack_doe.py
--rw-r--r--   0        0        0     3860 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/pad.py
--rw-r--r--   0        0        0     1890 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/pad_gsg.py
--rw-r--r--   0        0        0     1157 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/pads_shorted.py
--rw-r--r--   0        0        0     3833 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/polarization_splitter_rotator.py
--rw-r--r--   0        0        0     1147 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/ramp.py
--rw-r--r--   0        0        0     1508 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/rectangle.py
--rw-r--r--   0        0        0     2972 2023-05-10 22:43:05.005753 gdsfactory-6.92.2/gdsfactory/components/rectangle_with_slits.py
--rw-r--r--   0        0        0     1508 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/regular_polygon.py
--rw-r--r--   0        0        0     3302 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/resistance_meander.py
--rw-r--r--   0        0        0     2642 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/resistance_sheet.py
--rw-r--r--   0        0        0     1273 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring.py
--rw-r--r--   0        0        0     4143 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_crow.py
--rw-r--r--   0        0        0     3272 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_crow_couplers.py
--rw-r--r--   0        0        0     2267 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_double.py
--rw-r--r--   0        0        0     3846 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_double_heater.py
--rw-r--r--   0        0        0     7757 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_double_pn.py
--rw-r--r--   0        0        0    12137 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_section_based.py
--rw-r--r--   0        0        0     2719 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_single.py
--rw-r--r--   0        0        0     1968 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_single_array.py
--rw-r--r--   0        0        0     6098 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_single_bend_coupler.py
--rw-r--r--   0        0        0     2714 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_single_dut.py
--rw-r--r--   0        0        0     4018 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_single_heater.py
--rw-r--r--   0        0        0     5267 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/ring_single_pn.py
--rw-r--r--   0        0        0     2282 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/seal_ring.py
--rw-r--r--   0        0        0     3758 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/snspd.py
--rw-r--r--   0        0        0     2059 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/spiral_double.py
--rw-r--r--   0        0        0     5871 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/spiral_external_io.py
--rw-r--r--   0        0        0    16658 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/spiral_heater.py
--rw-r--r--   0        0        0     9181 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/spiral_inner_io.py
--rw-r--r--   0        0        0     1754 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/splitter_chain.py
--rw-r--r--   0        0        0     5327 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/splitter_tree.py
--rw-r--r--   0        0        0     2526 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight.py
--rw-r--r--   0        0        0     1033 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight_array.py
--rw-r--r--   0        0        0     7914 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight_heater_doped_rib.py
--rw-r--r--   0        0        0     1922 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight_heater_doped_strip.py
--rw-r--r--   0        0        0     7891 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight_heater_meander.py
--rw-r--r--   0        0        0     8090 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight_heater_meander_doped.py
--rw-r--r--   0        0        0     5686 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight_heater_metal.py
--rw-r--r--   0        0        0     2809 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight_pin.py
--rw-r--r--   0        0        0     3974 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight_pin_slot.py
--rw-r--r--   0        0        0      655 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/straight_rib.py
--rw-r--r--   0        0        0      820 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/switch_tree.py
--rw-r--r--   0        0        0     7713 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/taper.py
--rw-r--r--   0        0        0     3530 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/taper_adiabatic.py
--rw-r--r--   0        0        0     2457 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/taper_cross_section.py
--rw-r--r--   0        0        0     2363 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/taper_from_csv.py
--rw-r--r--   0        0        0     1215 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/taper_parabolic.py
--rw-r--r--   0        0        0     1635 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/terminator.py
--rw-r--r--   0        0        0     2913 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/text.py
--rw-r--r--   0        0        0     3821 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/text_freetype.py
--rw-r--r--   0        0        0     3160 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/text_rectangular.py
--rw-r--r--   0        0        0     3943 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/text_rectangular_font.py
--rw-r--r--   0        0        0     2536 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/triangles.py
--rw-r--r--   0        0        0      715 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/verniers.py
--rw-r--r--   0        0        0     2468 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/version_stamp.py
--rw-r--r--   0        0        0     2436 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/via.py
--rw-r--r--   0        0        0     3060 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/via_corner.py
--rw-r--r--   0        0        0     5342 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/via_cutback.py
--rw-r--r--   0        0        0    15574 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/via_stack.py
--rw-r--r--   0        0        0     4554 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/via_stack_slot.py
--rw-r--r--   0        0        0     4944 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/via_stack_with_offset.py
--rw-r--r--   0        0        0     1088 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/wafer.py
--rw-r--r--   0        0        0     2542 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/wire.py
--rw-r--r--   0        0        0      978 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/components/wire_sbend.py
--rw-r--r--   0        0        0     7919 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/config.py
--rw-r--r--   0        0        0      481 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/conftest.py
--rw-r--r--   0        0        0    38409 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/constants.py
--rw-r--r--   0        0        0     1476 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/containers.py
--rw-r--r--   0        0        0    82607 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/cross_section.py
--rw-r--r--   0        0        0     2974 2023-05-10 22:43:05.009753 gdsfactory-6.92.2/gdsfactory/decorators.py
--rw-r--r--   0        0        0     7312 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/difftest.py
--rw-r--r--   0        0        0      988 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/events.py
--rw-r--r--   0        0        0      204 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/export/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/export/to_3d.py
--rw-r--r--   0        0        0     1940 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/export/to_np.py
--rw-r--r--   0        0        0     3058 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/export/to_stl.py
--rw-r--r--   0        0        0     7438 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/export/write_gerbers.py
--rw-r--r--   0        0        0     2968 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/filestorage.py
--rw-r--r--   0        0        0    11860 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/fill.py
--rw-r--r--   0        0        0     7799 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/font.py
--rw-r--r--   0        0        0     8073 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/functions.py
--rw-r--r--   0        0        0       20 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/gdsdiff/.gitattributes
--rw-r--r--   0        0        0       83 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/gdsdiff/.gitconfig
--rw-r--r--   0        0        0       72 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/gdsdiff/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/gdsdiff/gds_diff_git.py
--rw-r--r--   0        0        0     2935 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/gdsdiff/gdsdiff.py
--rw-r--r--   0        0        0      708 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/gdsdiff/install.py
--rw-r--r--   0        0        0      271 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/gdsdiff/sample.py
--rw-r--r--   0        0        0     1059 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/gdsdiff/test_xor.py
--rw-r--r--   0        0        0     1100 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/README.md
--rw-r--r--   0        0        0     1722 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/__init__.py
--rw-r--r--   0        0        0      169 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/generic_tech.sh
--rw-r--r--   0        0        0     8142 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/get_klayout_pyxs.py
--rw-r--r--   0        0        0       44 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/README.md
--rw-r--r--   0        0        0      104 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/Makefile
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/__init__.py
--rw-r--r--   0        0        0     2842 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/errors.py
--rw-r--r--   0        0        0      579 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/generic.drc
--rw-r--r--   0        0        0     2929 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/generic.lydrc
--rw-r--r--   0        0        0     1014 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/write_drc.py
--rw-r--r--   0        0        0     6193 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/grain.xml
--rw-r--r--   0        0        0    10140 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/icon_128x128.png
--rw-r--r--   0        0        0     4248 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/icon_64x64.png
--rw-r--r--   0        0        0     3980 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/README.md
--rw-r--r--   0        0        0     2419 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
--rw-r--r--   0        0        0     9696 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
--rw-r--r--   0        0        0    12347 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
--rw-r--r--   0        0        0     7540 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
--rw-r--r--   0        0        0     3437 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
--rw-r--r--   0        0        0      479 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
--rw-r--r--   0        0        0      582 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
--rw-r--r--   0        0        0      108 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
--rw-r--r--   0        0        0      186 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
--rw-r--r--   0        0        0      398 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
--rw-r--r--   0        0        0      574 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
--rw-r--r--   0        0        0     6034 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
--rw-r--r--   0        0        0    12078 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
--rw-r--r--   0        0        0      493 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
--rw-r--r--   0        0        0     2637 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
--rw-r--r--   0        0        0      921 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
--rw-r--r--   0        0        0    10945 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
--rw-r--r--   0        0        0      710 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0      538 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/python/__init__.py
--rw-r--r--   0        0        0      114 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
--rw-r--r--   0        0        0     4303 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
--rw-r--r--   0        0        0      269 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/Makefile
--rw-r--r--   0        0        0     1519 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/generic.layerstack
--rw-r--r--   0        0        0    40153 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
--rw-r--r--   0        0        0     7689 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyt
--rw-r--r--   0        0        0     4258 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
--rw-r--r--   0        0        0     4537 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
--rw-r--r--   0        0        0     4690 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
--rw-r--r--   0        0        0     5508 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
--rw-r--r--   0        0        0     1855 2023-05-10 22:43:05.013753 gdsfactory-6.92.2/gdsfactory/generic_tech/layer_map.py
--rw-r--r--   0        0        0     6511 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/generic_tech/layer_stack.py
--rw-r--r--   0        0        0    10547 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/generic_tech/layer_views.yaml
--rw-r--r--   0        0        0      158 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/generic_tech/simulation_settings.py
--rw-r--r--   0        0        0     1431 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/boolean.py
--rw-r--r--   0        0        0     3814 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/boolean_klayout.py
--rw-r--r--   0        0        0     1904 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/boolean_polygons.py
--rw-r--r--   0        0        0      598 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/check_duplicated_cells.py
--rw-r--r--   0        0        0     2719 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/check_exclusion.py
--rw-r--r--   0        0        0     2829 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/check_inclusion.py
--rw-r--r--   0        0        0     3566 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/check_space.py
--rw-r--r--   0        0        0     1904 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/check_width.py
--rw-r--r--   0        0        0     5005 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/fill_klayout.py
--rw-r--r--   0        0        0     7084 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/fill_tiled.py
--rw-r--r--   0        0        0     1697 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/fillet.py
--rw-r--r--   0        0        0     6664 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/functions.py
--rw-r--r--   0        0        0     2167 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/invert.py
--rw-r--r--   0        0        0     3685 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/layer_priority.py
--rw-r--r--   0        0        0     3046 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/manhattanize.py
--rw-r--r--   0        0        0     4192 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/maskprep.py
--rw-r--r--   0        0        0     4744 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/maskprep_flat.py
--rw-r--r--   0        0        0     3250 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/offset.py
--rw-r--r--   0        0        0     3842 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/outline.py
--rw-r--r--   0        0        0     2510 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/trim.py
--rw-r--r--   0        0        0     2948 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/union.py
--rw-r--r--   0        0        0     9629 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/write_drc.py
--rw-r--r--   0        0        0     1783 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/geometry/xor_diff.py
--rw-r--r--   0        0        0     1158 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/get_factories.py
--rw-r--r--   0        0        0    23561 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/get_netlist.py
--rw-r--r--   0        0        0    14426 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/get_netlist_flat.py
--rw-r--r--   0        0        0      682 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/get_netlist_klayout.py
--rw-r--r--   0        0        0     9745 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/grid.py
--rw-r--r--   0        0        0     4363 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/install.py
--rw-r--r--   0        0        0     1340 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/klive.py
--rw-r--r--   0        0        0      585 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/labels/__init__.py
--rw-r--r--   0        0        0     3563 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/labels/add_label_yaml.py
--rw-r--r--   0        0        0     3847 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/labels/ehva.py
--rw-r--r--   0        0        0     3810 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/labels/merge_test_metadata.py
--rw-r--r--   0        0        0     4668 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/labels/siepic.py
--rw-r--r--   0        0        0     4847 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/labels/write_labels.py
--rw-r--r--   0        0        0     1149 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/materials.py
--rw-r--r--   0        0        0     5247 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/name.py
--rw-r--r--   0        0        0    11586 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/pack.py
--rw-r--r--   0        0        0    50880 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/path.py
--rw-r--r--   0        0        0    25849 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/pdk.py
--rw-r--r--   0        0        0     6170 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/picmodel.py
--rw-r--r--   0        0        0     5068 2023-05-10 22:43:05.017753 gdsfactory-6.92.2/gdsfactory/pixelate.py
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/plugins/dagster/__init__.py
--rw-r--r--   0        0        0      976 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/plugins/dagster/workflow.py
--rw-r--r--   0        0        0      566 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/plugins/database/README.md
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/plugins/database/__init__.py
--rw-r--r--   0        0        0     6216 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/plugins/database/db_upload.py
--rw-r--r--   0        0        0    16143 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/plugins/database/models.py
--rw-r--r--   0        0        0    32209 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/port.py
--rw-r--r--   0        0        0    37609 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/quickplotter.py
--rw-r--r--   0        0        0      696 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/read/__init__.py
--rw-r--r--   0        0        0     1639 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/read/from_dphox.py
--rw-r--r--   0        0        0     1285 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/read/from_gdspaths.py
--rw-r--r--   0        0        0     1953 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/read/from_np.py
--rw-r--r--   0        0        0     2813 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/read/from_phidl.py
--rw-r--r--   0        0        0    38082 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/read/from_yaml.py
--rw-r--r--   0        0        0     5897 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/read/from_yaml_template.py
--rw-r--r--   0        0        0     5688 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/read/import_gds.py
--rw-r--r--   0        0        0     3407 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/read/labels.py
--rw-r--r--   0        0        0     3769 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/__init__.py
--rw-r--r--   0        0        0     2920 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/add_electrical_pads_shortest.py
--rw-r--r--   0        0        0     3015 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/add_electrical_pads_top.py
--rw-r--r--   0        0        0     3035 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/add_electrical_pads_top_dc.py
--rw-r--r--   0        0        0     8715 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/add_fiber_array.py
--rw-r--r--   0        0        0    10624 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/add_fiber_single.py
--rw-r--r--   0        0        0     8967 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/add_pads.py
--rw-r--r--   0        0        0    38940 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/all_angle.py
--rw-r--r--   0        0        0     3916 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/auto_taper.py
--rw-r--r--   0        0        0      982 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/factories.py
--rw-r--r--   0        0        0     4415 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/fanout.py
--rw-r--r--   0        0        0     2800 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/fanout2x2.py
--rw-r--r--   0        0        0    24342 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/get_bundle.py
--rw-r--r--   0        0        0     8632 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/get_bundle_corner.py
--rw-r--r--   0        0        0     6900 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/get_bundle_from_steps.py
--rw-r--r--   0        0        0    12949 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/get_bundle_from_waypoints.py
--rw-r--r--   0        0        0     5284 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/get_bundle_path_length_match.py
--rw-r--r--   0        0        0     1937 2023-05-10 22:43:05.021753 gdsfactory-6.92.2/gdsfactory/routing/get_bundle_sbend.py
--rw-r--r--   0        0        0    17064 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/get_bundle_u.py
--rw-r--r--   0        0        0     1510 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/get_input_labels.py
--rw-r--r--   0        0        0     9233 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/get_route.py
--rw-r--r--   0        0        0    10824 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/get_route_astar.py
--rw-r--r--   0        0        0     6119 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/get_route_from_steps.py
--rw-r--r--   0        0        0     2766 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/get_route_sbend.py
--rw-r--r--   0        0        0     3311 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/get_routes_bend180.py
--rw-r--r--   0        0        0     1854 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/get_routes_straight.py
--rw-r--r--   0        0        0    34394 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/manhattan.py
--rw-r--r--   0        0        0    10081 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/path_length_matching.py
--rw-r--r--   0        0        0    22568 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/route_fiber_array.py
--rw-r--r--   0        0        0     8679 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/route_fiber_single.py
--rw-r--r--   0        0        0    18132 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/route_ports_to_side.py
--rw-r--r--   0        0        0     4361 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/route_quad.py
--rw-r--r--   0        0        0    14370 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/route_sharp.py
--rw-r--r--   0        0        0    10167 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/route_south.py
--rw-r--r--   0        0        0     5072 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/sort_ports.py
--rw-r--r--   0        0        0     2477 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/routing/utils.py
--rw-r--r--   0        0        0     2889 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/01_component_pcell.py
--rw-r--r--   0        0        0      646 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
--rw-r--r--   0        0        0     1101 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/01_component_pcell_with_pins.py
--rw-r--r--   0        0        0      664 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
--rw-r--r--   0        0        0      347 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/02_component_autoname.py
--rw-r--r--   0        0        0      887 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/03_move.py
--rw-r--r--   0        0        0      881 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/04_connect.py
--rw-r--r--   0        0        0      710 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/05_remove_layers.py
--rw-r--r--   0        0        0      931 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/06_remapping_layers.py
--rw-r--r--   0        0        0     1082 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/07_flattening_device.py
--rw-r--r--   0        0        0      475 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/08_group.py
--rw-r--r--   0        0        0     1631 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/11_component_layout.py
--rw-r--r--   0        0        0     2245 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/12_component_refs.py
--rw-r--r--   0        0        0      955 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/13_component_netlist.py
--rw-r--r--   0        0        0     2592 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/14_component_connectivity.py
--rw-r--r--   0        0        0     1636 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/15_component_sequence1.py
--rw-r--r--   0        0        0     1680 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/16_component_sequence2.py
--rw-r--r--   0        0        0      965 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/17_ports.py
--rw-r--r--   0        0        0      489 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/18_port_markers.py
--rw-r--r--   0        0        0      361 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/19_references.py
--rw-r--r--   0        0        0      533 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/20_components.py
--rw-r--r--   0        0        0      507 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/21_add_fiber_array.py
--rw-r--r--   0        0        0      493 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/22_add_fiber_single.py
--rw-r--r--   0        0        0      569 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/22_add_pads.py
--rw-r--r--   0        0        0      848 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/23_reticle.py
--rw-r--r--   0        0        0     1588 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/23_reticle_passives.py
--rw-r--r--   0        0        0      457 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/24_doe.py
--rw-r--r--   0        0        0      687 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/24_doe_2.py
--rw-r--r--   0        0        0      692 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/24_doe_3.py
--rw-r--r--   0        0        0      306 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/25_slot_cross_section.py
--rw-r--r--   0        0        0     1363 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/30_lidar.py
--rw-r--r--   0        0        0     1412 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/30_lidar_pcell.py
--rw-r--r--   0        0        0     1943 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/30_lidar_with_pads.py
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/__init__.py
--rw-r--r--   0        0        0     1307 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing.py
--rw-r--r--   0        0        0      558 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
--rw-r--r--   0        0        0     6062 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
--rw-r--r--   0        0        0      444 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
--rw-r--r--   0        0        0      463 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
--rw-r--r--   0        0        0     1552 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
--rw-r--r--   0        0        0     1315 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
--rw-r--r--   0        0        0      602 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
--rw-r--r--   0        0        0     3317 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
--rw-r--r--   0        0        0     1484 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
--rw-r--r--   0        0        0     3045 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
--rw-r--r--   0        0        0     3782 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
--rw-r--r--   0        0        0     1988 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/big_device.py
--rw-r--r--   0        0        0       19 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/Makefile
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/benchmark/fill_demo.py
--rw-r--r--   0        0        0      343 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
--rw-r--r--   0        0        0      637 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/circuits/mask.pic.yml
--rw-r--r--   0        0        0      622 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
--rw-r--r--   0        0        0      569 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
--rw-r--r--   0        0        0      453 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/circuits/pads.pic.yml
--rw-r--r--   0        0        0      287 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/circuits/rectangles.pic.yml
--rw-r--r--   0        0        0     2260 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/drc_errors.py
--rw-r--r--   0        0        0     1014 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/drc_write.py
--rw-r--r--   0        0        0     4530 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/layers.py
--rw-r--r--   0        0        0      158 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/layers_sky130.py
--rw-r--r--   0        0        0      364 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/layers_xsection.py
--rw-r--r--   0        0        0     1062 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/lvs.py
--rw-r--r--   0        0        0      574 2023-05-10 22:43:05.025753 gdsfactory-6.92.2/gdsfactory/samples/demo/pcell.py
--rw-r--r--   0        0        0     4174 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/netlists/mzi.yml
--rw-r--r--   0        0        0     5840 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/netlists/mzi_full.yml
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/__init__.py
--rw-r--r--   0        0        0     4235 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/fab_c.py
--rw-r--r--   0        0        0      475 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/fab_d/__init__.py
--rw-r--r--   0        0        0     1880 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/fab_d/phase_shifters.py
--rw-r--r--   0        0        0     1715 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c.py
--rw-r--r--   0        0        0       50 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
--rw-r--r--   0        0        0       93 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
--rw-r--r--   0        0        0       85 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
--rw-r--r--   0        0        0      139 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
--rw-r--r--   0        0        0       90 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
--rw-r--r--   0        0        0      126 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
--rw-r--r--   0        0        0       48 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
--rw-r--r--   0        0        0     1023 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
--rw-r--r--   0        0        0     2100 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
--rw-r--r--   0        0        0     1839 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
--rw-r--r--   0        0        0     1267 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
--rw-r--r--   0        0        0     1592 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
--rw-r--r--   0        0        0     1061 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
--rw-r--r--   0        0        0     1054 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
--rw-r--r--   0        0        0     1577 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
--rw-r--r--   0        0        0     4313 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
--rw-r--r--   0        0        0     3625 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
--rw-r--r--   0        0        0     3603 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
--rw-r--r--   0        0        0     4271 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
--rw-r--r--   0        0        0      840 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
--rw-r--r--   0        0        0     2171 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
--rw-r--r--   0        0        0      316 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/schematic.py
--rw-r--r--   0        0        0    17692 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/schematic_editor.py
--rw-r--r--   0        0        0     4194 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/serialization.py
--rw-r--r--   0        0        0     1612 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/show.py
--rw-r--r--   0        0        0      724 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/__init__.py
--rw-r--r--   0        0        0     4369 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/add_simulation_markers.py
--rw-r--r--   0        0        0     2476 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/convert_sparameters.py
--rw-r--r--   0        0        0      547 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/devsim/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/devsim/doping.py
--rw-r--r--   0        0        0    11977 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/devsim/get_simulation.py
--rw-r--r--   0        0        0    23601 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19708 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/devsim/get_solver.py
--rw-r--r--   0        0        0     1632 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/devsim/test_devsim.py
--rw-r--r--   0        0        0      189 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/disable_print.py
--rw-r--r--   0        0        0       79 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/eme/__init__.py
--rw-r--r--   0        0        0    14784 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/eme/meow_eme.py
--rw-r--r--   0        0        0     1771 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/eme/test_meow_simulation.py
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/fem/__init__.py
--rw-r--r--   0        0        0     8968 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/fem/mode_solver.py
--rw-r--r--   0        0        0     2205 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/fem/test_mode_solver.py
--rw-r--r--   0        0        0     3351 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/get_effective_indices.py
--rw-r--r--   0        0        0     3109 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/get_modes_path.py
--rw-r--r--   0        0        0     3888 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/get_sparameters_path.py
--rw-r--r--   0        0        0     1863 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/__init__.py
--rw-r--r--   0        0        0     3194 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_material.py
--rw-r--r--   0        0        0     6137 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6054 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    11014 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15701 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    17944 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12302 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11914 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0      832 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6642 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-10 22:43:05.029753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    13951 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    21273 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8135 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9561 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0     1246 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/__init__.py
--rw-r--r--   0        0        0     6653 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/break_geometry.py
--rw-r--r--   0        0        0    11250 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/mesh.py
--rw-r--r--   0        0        0    11808 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/meshtracker.py
--rw-r--r--   0        0        0     7752 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/parse_component.py
--rw-r--r--   0        0        0     3644 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/parse_gds.py
--rw-r--r--   0        0        0     3605 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/parse_layerstack.py
--rw-r--r--   0        0        0     2990 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/refine.py
--rw-r--r--   0        0        0    10851 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     2489 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/tests/test_meshing.py
--rw-r--r--   0        0        0    14168 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     7441 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0    16326 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0     1524 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/__init__.py
--rw-r--r--   0        0        0     4368 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/get_results.py
--rw-r--r--   0        0        0    20009 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/get_simulation.py
--rw-r--r--   0        0        0    21061 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     2821 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/materials.py
--rw-r--r--   0        0        0    39677 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/modes.py
--rw-r--r--   0        0        0     8941 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/sim_run.yaml
--rw-r--r--   0        0        0     8114 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
--rw-r--r--   0        0        0     8114 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
--rw-r--r--   0        0        0     1597 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_modes.py
--rw-r--r--   0        0        0      262 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      879 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_results.py
--rw-r--r--   0        0        0     1505 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
--rw-r--r--   0        0        0     1270 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
--rw-r--r--   0        0        0     9297 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
--rw-r--r--   0        0        0     1732 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0     1224 2023-05-10 22:43:05.033753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/utils.py
--rw-r--r--   0        0        0    10515 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/write_sparameters.py
--rw-r--r--   0        0        0     7695 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0      588 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/lumerical/__init__.py
--rw-r--r--   0        0        0    16011 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/lumerical/interconnect.py
--rw-r--r--   0        0        0     4286 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/lumerical/settings.py
--rw-r--r--   0        0        0     2348 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/lumerical/test_read_sparameters.py
--rw-r--r--   0        0        0    19865 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     1504 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0      932 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/__init__.py
--rw-r--r--   0        0        0     1574 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/coupler.py
--rw-r--r--   0        0        0     4132 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2534 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     8846 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/find_modes.py
--rwxr-xr-x   0        0        0     7032 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4448 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2706 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     6956 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4462 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5257 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     7979 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2469 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/overlap.py
--rw-r--r--   0        0        0      418 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0      548 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1131 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      647 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      354 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0    15452 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/types.py
--rw-r--r--   0        0        0     1145 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/modes/waveguide.py
--rw-r--r--   0        0        0     2013 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3063 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0     7332 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/plot.py
--rw-r--r--   0        0        0     2480 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/plot_csv.py
--rw-r--r--   0        0        0      703 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/port_symmetries.py
--rw-r--r--   0        0        0     4637 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/process/diffusion.py
--rw-r--r--   0        0        0     5317 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/process/implant_tables.py
--rw-r--r--   0        0        0     6784 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      191 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/__init__.py
--rw-r--r--   0        0        0    14792 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/build_model.py
--rw-r--r--   0        0        0     7449 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/femwell_waveguide_model.py
--rw-r--r--   0        0        0     1571 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/interpolators.py
--rw-r--r--   0        0        0     6755 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/meep_FDTD_model.py
--rw-r--r--   0        0        0     4528 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/meow_eme_model.py
--rw-r--r--   0        0        0     5613 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/mlp.py
--rw-r--r--   0        0        0     7358 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/models.py
--rw-r--r--   0        0        0    13884 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/parameter.py
--rwxr-xr-x   0        0        0     2205 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/plot_model.py
--rw-r--r--   0        0        0     6805 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/read.py
--rw-r--r--   0        0        0     1350 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2220 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0     1397 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/sax/tests/test_parameters.py
--rw-r--r--   0        0        0     1357 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/add_gc.py
--rw-r--r--   0        0        0     3383 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/circuit.py
--rw-r--r--   0        0        0      891 2023-05-10 22:43:05.037753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/__init__.py
--rw-r--r--   0        0        0     1295 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/bend_circular.py
--rw-r--r--   0        0        0     1388 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/bend_euler.py
--rw-r--r--   0        0        0     2560 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler.py
--rw-r--r--   0        0        0     1046 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler_fdtd.py
--rw-r--r--   0        0        0     1848 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler_ring.py
--rw-r--r--   0        0        0     1329 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
--rw-r--r--   0        0        0      589 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
--rw-r--r--   0        0        0      913 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/gc.py
--rw-r--r--   0        0        0     2032 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/mmi1x2.py
--rw-r--r--   0        0        0     1910 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/mmi2x2.py
--rw-r--r--   0        0        0     2618 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/mzi.py
--rw-r--r--   0        0        0     1759 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/mzi_siepic.py
--rw-r--r--   0        0        0      487 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/mzi_thermal.py
--rw-r--r--   0        0        0     2597 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/ring_double.py
--rw-r--r--   0        0        0     1665 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/ring_double_siepic.py
--rw-r--r--   0        0        0     1782 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/ring_single.py
--rw-r--r--   0        0        0     1416 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/ring_single_siepic.py
--rw-r--r--   0        0        0     1099 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/straight.py
--rw-r--r--   0        0        0      800 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/get_transmission.py
--rw-r--r--   0        0        0     2516 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/model_from_gdsfactory.py
--rw-r--r--   0        0        0     3841 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/model_from_sparameters.py
--rw-r--r--   0        0        0     2438 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/plot_circuit.py
--rw-r--r--   0        0        0     1798 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
--rw-r--r--   0        0        0     2773 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/plot_model.py
--rw-r--r--   0        0        0     1261 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_circuit.py
--rw-r--r--   0        0        0       90 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
--rw-r--r--   0        0        0     1109 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components.py
--rw-r--r--   0        0        0       66 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
--rw-r--r--   0        0        0       69 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
--rw-r--r--   0        0        0       69 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
--rw-r--r--   0        0        0       92 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
--rw-r--r--   0        0        0       92 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
--rw-r--r--   0        0        0      412 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
--rw-r--r--   0        0        0      412 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
--rw-r--r--   0        0        0      114 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
--rw-r--r--   0        0        0      256 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
--rw-r--r--   0        0        0      460 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
--rw-r--r--   0        0        0      104 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
--rw-r--r--   0        0        0      166 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/simphony/types.py
--rw-r--r--   0        0        0      471 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/sipann/__init__.py
--rw-r--r--   0        0        0     1376 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/sipann/bend_circular.py
--rw-r--r--   0        0        0     1465 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/sipann/bend_euler.py
--rw-r--r--   0        0        0     2508 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/sipann/coupler.py
--rw-r--r--   0        0        0     1892 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/sipann/coupler_ring.py
--rw-r--r--   0        0        0      736 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/sipann/straight.py
--rw-r--r--   0        0        0      100 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/thermal/__init__.py
--rw-r--r--   0        0        0     7781 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/simulation/thermal/heater.py
--rw-r--r--   0        0        0     1744 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/snap.py
--rw-r--r--   0        0        0     4245 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/symbols.py
--rw-r--r--   0        0        0      524 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/technology/__init__.py
--rw-r--r--   0        0        0     7065 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/technology/klayout_tech.py
--rw-r--r--   0        0        0     1078 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/technology/layer_map.py
--rw-r--r--   0        0        0    14989 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/technology/layer_stack.py
--rw-r--r--   0        0        0    42052 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/technology/layer_views.py
--rw-r--r--   0        0        0     1984 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/technology/simulation_settings.py
--rw-r--r--   0        0        0     1635 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/types.py
--rw-r--r--   0        0        0    10000 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/typings.py
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/utils/__init__.py
--rw-r--r--   0        0        0     1304 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/utils/async_utils.py
--rw-r--r--   0        0        0      376 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/utils/color_utils.py
--rw-r--r--   0        0        0      558 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/utils/file_utils.py
--rw-r--r--   0        0        0      185 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/utils/function_utils.py
--rw-r--r--   0        0        0      676 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/utils/xml_utils.py
--rw-r--r--   0        0        0     1429 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/utils/yaml_utils.py
--rw-r--r--   0        0        0     4825 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/watch.py
--rw-r--r--   0        0        0        0 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/widgets/__init__.py
--rw-r--r--   0        0        0     7921 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/widgets/layout_viewer.py
--rw-r--r--   0        0        0     7464 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/gdsfactory/write_cells.py
--rw-r--r--   0        0        0     5467 2023-05-10 22:43:05.041753 gdsfactory-6.92.2/pyproject.toml
--rw-r--r--   0        0        0    18552 1970-01-01 00:00:00.000000 gdsfactory-6.92.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-11 23:07:58.955547 gdsfactory-6.93.0/LICENSE
+-rw-r--r--   0        0        0    14281 2023-05-11 23:07:58.955547 gdsfactory-6.93.0/README.md
+-rw-r--r--   0        0        0     3415 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/__init__.py
+-rw-r--r--   0        0        0     2096 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/add_keepout.py
+-rw-r--r--   0        0        0    12629 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/add_labels.py
+-rw-r--r--   0        0        0     3711 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/add_loopback.py
+-rw-r--r--   0        0        0     5054 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/add_padding.py
+-rw-r--r--   0        0        0    15465 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/add_pins.py
+-rw-r--r--   0        0        0    14700 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/add_ports.py
+-rw-r--r--   0        0        0     2884 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/add_tapers.py
+-rw-r--r--   0        0        0     2257 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/add_tapers_cross_section.py
+-rw-r--r--   0        0        0     1831 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/add_termination.py
+-rw-r--r--   0        0        0     1676 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/asserts.py
+-rw-r--r--   0        0        0    11843 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/cell.py
+-rw-r--r--   0        0        0    15946 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/circuitviz.py
+-rw-r--r--   0        0        0     5325 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/cli.py
+-rw-r--r--   0        0        0   100543 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/component.py
+-rw-r--r--   0        0        0    23360 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/component_layout.py
+-rw-r--r--   0        0        0    29699 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/component_reference.py
+-rw-r--r--   0        0        0     1205 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/C.py
+-rw-r--r--   0        0        0     1144 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/L.py
+-rw-r--r--   0        0        0    20964 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/__init__.py
+-rw-r--r--   0        0        0     2621 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/add_fiducials.py
+-rw-r--r--   0        0        0    14087 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/add_grating_couplers.py
+-rw-r--r--   0        0        0     2014 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/add_trenches.py
+-rw-r--r--   0        0        0     3207 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/align.py
+-rw-r--r--   0        0        0     2622 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/array_component.py
+-rw-r--r--   0        0        0     4705 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/array_with_fanout.py
+-rw-r--r--   0        0        0     4322 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/array_with_via.py
+-rw-r--r--   0        0        0     4042 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/awg.py
+-rw-r--r--   0        0        0     1269 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/bbox.py
+-rw-r--r--   0        0        0     2851 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/bend_circular.py
+-rw-r--r--   0        0        0     2649 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/bend_circular_heater.py
+-rw-r--r--   0        0        0     7903 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/bend_euler.py
+-rw-r--r--   0        0        0     2682 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/bend_port.py
+-rw-r--r--   0        0        0     3664 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/bend_s.py
+-rw-r--r--   0        0        0     5373 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/bezier.py
+-rw-r--r--   0        0        0     1605 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/cavity.py
+-rw-r--r--   0        0        0     5766 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/cdc.py
+-rw-r--r--   0        0        0     2929 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/cdsem_all.py
+-rw-r--r--   0        0        0     1788 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/cdsem_bend180.py
+-rw-r--r--   0        0        0     1631 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/cdsem_coupler.py
+-rw-r--r--   0        0        0     1412 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/cdsem_straight.py
+-rw-r--r--   0        0        0     1565 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/cdsem_straight_density.py
+-rw-r--r--   0        0        0      793 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/circle.py
+-rw-r--r--   0        0        0     5722 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/coh_rx_dual_pol.py
+-rw-r--r--   0        0        0     8922 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/coh_rx_single_pol.py
+-rw-r--r--   0        0        0     5043 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/coh_tx_dual_pol.py
+-rw-r--r--   0        0        0     6118 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/coh_tx_single_pol.py
+-rw-r--r--   0        0        0     2548 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/compass.py
+-rw-r--r--   0        0        0     9856 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/component_lattice.py
+-rw-r--r--   0        0        0     7174 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/component_sequence.py
+-rw-r--r--   0        0        0      812 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/copy_layers.py
+-rw-r--r--   0        0        0     3460 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/coupler.py
+-rw-r--r--   0        0        0     2113 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/coupler90.py
+-rw-r--r--   0        0        0     1802 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/coupler90bend.py
+-rw-r--r--   0        0        0     4666 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/coupler_adiabatic.py
+-rw-r--r--   0        0        0     1909 2023-05-11 23:07:58.963547 gdsfactory-6.93.0/gdsfactory/components/coupler_asymmetric.py
+-rw-r--r--   0        0        0     3970 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/coupler_full.py
+-rw-r--r--   0        0        0     3414 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/coupler_ring.py
+-rw-r--r--   0        0        0     1060 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/coupler_straight.py
+-rw-r--r--   0        0        0     1164 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/coupler_straight_asymmetric.py
+-rw-r--r--   0        0        0     2192 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/coupler_symmetric.py
+-rw-r--r--   0        0        0     1848 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/cross.py
+-rw-r--r--   0        0        0    12873 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/crossing_waveguide.py
+-rw-r--r--   0        0        0      500 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
+-rw-r--r--   0        0        0     1014 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
+-rw-r--r--   0        0        0    19749 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
+-rw-r--r--   0        0        0    19751 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
+-rw-r--r--   0        0        0    19749 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
+-rw-r--r--   0        0        0    19751 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
+-rw-r--r--   0        0        0    19775 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
+-rw-r--r--   0        0        0     3143 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
+-rw-r--r--   0        0        0     5272 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/cutback_2x2.py
+-rw-r--r--   0        0        0     6450 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/cutback_bend.py
+-rw-r--r--   0        0        0     3765 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/cutback_component.py
+-rw-r--r--   0        0        0     2721 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/cutback_splitter.py
+-rw-r--r--   0        0        0     2971 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/dbr.py
+-rw-r--r--   0        0        0     4288 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/dbr_tapered.py
+-rw-r--r--   0        0        0     2486 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/delay_snake.py
+-rw-r--r--   0        0        0     3177 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/delay_snake2.py
+-rw-r--r--   0        0        0     3237 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/delay_snake3.py
+-rw-r--r--   0        0        0     4319 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/delay_snake_sbend.py
+-rw-r--r--   0        0        0     1226 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/dicing_lane.py
+-rw-r--r--   0        0        0     3471 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/die.py
+-rw-r--r--   0        0        0     2975 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/die_bbox.py
+-rw-r--r--   0        0        0     2863 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/die_bbox_frame.py
+-rw-r--r--   0        0        0     8015 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/disk.py
+-rw-r--r--   0        0        0     4112 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/edge_coupler_array.py
+-rw-r--r--   0        0        0     1214 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/ellipse.py
+-rw-r--r--   0        0        0     1800 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/extend_ports_list.py
+-rw-r--r--   0        0        0     7944 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/extension.py
+-rw-r--r--   0        0        0      981 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/fiber.py
+-rw-r--r--   0        0        0     1432 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/fiber_array.py
+-rw-r--r--   0        0        0      722 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/fiducial_squares.py
+-rw-r--r--   0        0        0     3290 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/ge_detector_straight_si_contacts.py
+-rw-r--r--   0        0        0     1063 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_array.py
+-rw-r--r--   0        0        0     4682 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_dual_pol.py
+-rw-r--r--   0        0        0     7110 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_elliptical.py
+-rw-r--r--   0        0        0     7221 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
+-rw-r--r--   0        0        0     4960 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
+-rw-r--r--   0        0        0     4592 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
+-rw-r--r--   0        0        0     1773 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_functions.py
+-rw-r--r--   0        0        0     9058 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_loss.py
+-rw-r--r--   0        0        0     1786 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
+-rw-r--r--   0        0        0     4142 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_rectangular.py
+-rw-r--r--   0        0        0     4685 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
+-rw-r--r--   0        0        0     3887 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
+-rw-r--r--   0        0        0     1578 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/grating_coupler_tree.py
+-rw-r--r--   0        0        0     8773 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/greek_cross.py
+-rw-r--r--   0        0        0     1019 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/hline.py
+-rw-r--r--   0        0        0     3687 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/interdigital_capacitor.py
+-rw-r--r--   0        0        0     1825 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/litho_calipers.py
+-rw-r--r--   0        0        0     1244 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/litho_ruler.py
+-rw-r--r--   0        0        0     1304 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/litho_steps.py
+-rw-r--r--   0        0        0      650 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/logo.py
+-rw-r--r--   0        0        0     1679 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/loop_mirror.py
+-rw-r--r--   0        0        0     3873 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mmi1x2.py
+-rw-r--r--   0        0        0     2814 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mmi1x2_with_sbend.py
+-rw-r--r--   0        0        0     3858 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mmi2x2.py
+-rw-r--r--   0        0        0     3299 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mmi2x2_with_sbend.py
+-rw-r--r--   0        0        0     4947 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mmi_90degree_hybrid.py
+-rw-r--r--   0        0        0     3265 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mode_converter.py
+-rw-r--r--   0        0        0     7414 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mzi.py
+-rw-r--r--   0        0        0     2499 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mzi_arm.py
+-rw-r--r--   0        0        0     5835 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mzi_arms.py
+-rw-r--r--   0        0        0    12214 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mzi_lattice.py
+-rw-r--r--   0        0        0     4025 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mzi_pads_center.py
+-rw-r--r--   0        0        0     1064 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mzi_phase_shifter.py
+-rw-r--r--   0        0        0     6342 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mzit.py
+-rw-r--r--   0        0        0     3502 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mzit_lattice.py
+-rw-r--r--   0        0        0     6047 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/mzm.py
+-rw-r--r--   0        0        0     3518 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/nxn.py
+-rw-r--r--   0        0        0     1940 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/optimal_90deg.py
+-rw-r--r--   0        0        0     3876 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/optimal_hairpin.py
+-rw-r--r--   0        0        0     6131 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/optimal_step.py
+-rw-r--r--   0        0        0     6327 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/pack_doe.py
+-rw-r--r--   0        0        0     3860 2023-05-11 23:07:58.967547 gdsfactory-6.93.0/gdsfactory/components/pad.py
+-rw-r--r--   0        0        0     1890 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/pad_gsg.py
+-rw-r--r--   0        0        0     1157 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/pads_shorted.py
+-rw-r--r--   0        0        0     3833 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/polarization_splitter_rotator.py
+-rw-r--r--   0        0        0     1147 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ramp.py
+-rw-r--r--   0        0        0     1508 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/rectangle.py
+-rw-r--r--   0        0        0     2972 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/rectangle_with_slits.py
+-rw-r--r--   0        0        0     1508 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/regular_polygon.py
+-rw-r--r--   0        0        0     3302 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/resistance_meander.py
+-rw-r--r--   0        0        0     2642 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/resistance_sheet.py
+-rw-r--r--   0        0        0     1273 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring.py
+-rw-r--r--   0        0        0     4143 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_crow.py
+-rw-r--r--   0        0        0     3272 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_crow_couplers.py
+-rw-r--r--   0        0        0     2267 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_double.py
+-rw-r--r--   0        0        0     3846 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_double_heater.py
+-rw-r--r--   0        0        0     7757 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_double_pn.py
+-rw-r--r--   0        0        0    12137 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_section_based.py
+-rw-r--r--   0        0        0     2719 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_single.py
+-rw-r--r--   0        0        0     1968 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_single_array.py
+-rw-r--r--   0        0        0     6098 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_single_bend_coupler.py
+-rw-r--r--   0        0        0     2714 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_single_dut.py
+-rw-r--r--   0        0        0     4018 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_single_heater.py
+-rw-r--r--   0        0        0     5267 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/ring_single_pn.py
+-rw-r--r--   0        0        0     2282 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/seal_ring.py
+-rw-r--r--   0        0        0     3758 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/snspd.py
+-rw-r--r--   0        0        0     2059 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/spiral_double.py
+-rw-r--r--   0        0        0     5871 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/spiral_external_io.py
+-rw-r--r--   0        0        0    16658 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/spiral_heater.py
+-rw-r--r--   0        0        0     9181 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/spiral_inner_io.py
+-rw-r--r--   0        0        0     1754 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/splitter_chain.py
+-rw-r--r--   0        0        0     5327 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/splitter_tree.py
+-rw-r--r--   0        0        0     2526 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight.py
+-rw-r--r--   0        0        0     1033 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight_array.py
+-rw-r--r--   0        0        0     7914 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight_heater_doped_rib.py
+-rw-r--r--   0        0        0     1922 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight_heater_doped_strip.py
+-rw-r--r--   0        0        0     7891 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight_heater_meander.py
+-rw-r--r--   0        0        0     8090 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight_heater_meander_doped.py
+-rw-r--r--   0        0        0     5686 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight_heater_metal.py
+-rw-r--r--   0        0        0     2809 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight_pin.py
+-rw-r--r--   0        0        0     3974 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight_pin_slot.py
+-rw-r--r--   0        0        0      655 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/straight_rib.py
+-rw-r--r--   0        0        0      820 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/switch_tree.py
+-rw-r--r--   0        0        0     7713 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/taper.py
+-rw-r--r--   0        0        0     3530 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/taper_adiabatic.py
+-rw-r--r--   0        0        0     2457 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/taper_cross_section.py
+-rw-r--r--   0        0        0     2363 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/taper_from_csv.py
+-rw-r--r--   0        0        0     1215 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/taper_parabolic.py
+-rw-r--r--   0        0        0     1635 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/terminator.py
+-rw-r--r--   0        0        0     2913 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/text.py
+-rw-r--r--   0        0        0     3821 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/text_freetype.py
+-rw-r--r--   0        0        0     3160 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/text_rectangular.py
+-rw-r--r--   0        0        0     3943 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/text_rectangular_font.py
+-rw-r--r--   0        0        0     2536 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/triangles.py
+-rw-r--r--   0        0        0      715 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/verniers.py
+-rw-r--r--   0        0        0     2468 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/version_stamp.py
+-rw-r--r--   0        0        0     2436 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/via.py
+-rw-r--r--   0        0        0     3060 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/via_corner.py
+-rw-r--r--   0        0        0     5342 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/via_cutback.py
+-rw-r--r--   0        0        0    15574 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/via_stack.py
+-rw-r--r--   0        0        0     4554 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/via_stack_slot.py
+-rw-r--r--   0        0        0     4944 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/via_stack_with_offset.py
+-rw-r--r--   0        0        0     1088 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/wafer.py
+-rw-r--r--   0        0        0     2542 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/wire.py
+-rw-r--r--   0        0        0      978 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/components/wire_sbend.py
+-rw-r--r--   0        0        0     7919 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/config.py
+-rw-r--r--   0        0        0      481 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/conftest.py
+-rw-r--r--   0        0        0    38409 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/constants.py
+-rw-r--r--   0        0        0     1476 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/containers.py
+-rw-r--r--   0        0        0    82607 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/cross_section.py
+-rw-r--r--   0        0        0     2974 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/decorators.py
+-rw-r--r--   0        0        0     7312 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/difftest.py
+-rw-r--r--   0        0        0      988 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/events.py
+-rw-r--r--   0        0        0      204 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/export/__init__.py
+-rw-r--r--   0        0        0     3353 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/export/to_3d.py
+-rw-r--r--   0        0        0     1940 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/export/to_np.py
+-rw-r--r--   0        0        0     3058 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/export/to_stl.py
+-rw-r--r--   0        0        0     7438 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/export/write_gerbers.py
+-rw-r--r--   0        0        0     2968 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/filestorage.py
+-rw-r--r--   0        0        0    11860 2023-05-11 23:07:58.971547 gdsfactory-6.93.0/gdsfactory/fill.py
+-rw-r--r--   0        0        0     7799 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/font.py
+-rw-r--r--   0        0        0     8073 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/functions.py
+-rw-r--r--   0        0        0       20 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/gdsdiff/.gitattributes
+-rw-r--r--   0        0        0       83 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/gdsdiff/.gitconfig
+-rw-r--r--   0        0        0       72 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/gdsdiff/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/gdsdiff/gds_diff_git.py
+-rw-r--r--   0        0        0     2935 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/gdsdiff/gdsdiff.py
+-rw-r--r--   0        0        0      708 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/gdsdiff/install.py
+-rw-r--r--   0        0        0      271 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/gdsdiff/sample.py
+-rw-r--r--   0        0        0     1059 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/gdsdiff/test_xor.py
+-rw-r--r--   0        0        0     1100 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/README.md
+-rw-r--r--   0        0        0     1722 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/generic_tech.sh
+-rw-r--r--   0        0        0     8142 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/get_klayout_pyxs.py
+-rw-r--r--   0        0        0       44 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/README.md
+-rw-r--r--   0        0        0      104 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/Makefile
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/__init__.py
+-rw-r--r--   0        0        0     2842 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/errors.py
+-rw-r--r--   0        0        0      579 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/generic.drc
+-rw-r--r--   0        0        0     2929 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/generic.lydrc
+-rw-r--r--   0        0        0     1014 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/write_drc.py
+-rw-r--r--   0        0        0     6193 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/grain.xml
+-rw-r--r--   0        0        0    10140 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/icon_128x128.png
+-rw-r--r--   0        0        0     4248 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/icon_64x64.png
+-rw-r--r--   0        0        0     3980 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/README.md
+-rw-r--r--   0        0        0     2419 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
+-rw-r--r--   0        0        0     9696 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
+-rw-r--r--   0        0        0    12347 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
+-rw-r--r--   0        0        0     7540 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
+-rw-r--r--   0        0        0     3437 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
+-rw-r--r--   0        0        0      479 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
+-rw-r--r--   0        0        0      582 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
+-rw-r--r--   0        0        0      108 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
+-rw-r--r--   0        0        0      186 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
+-rw-r--r--   0        0        0      398 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
+-rw-r--r--   0        0        0      574 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
+-rw-r--r--   0        0        0     6034 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
+-rw-r--r--   0        0        0    12078 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
+-rw-r--r--   0        0        0      477 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
+-rw-r--r--   0        0        0     2682 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
+-rw-r--r--   0        0        0      921 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
+-rw-r--r--   0        0        0    10945 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
+-rw-r--r--   0        0        0      710 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0      538 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/python/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
+-rw-r--r--   0        0        0     4303 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
+-rw-r--r--   0        0        0      269 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/Makefile
+-rw-r--r--   0        0        0     1519 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
+-rw-r--r--   0        0        0    40161 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
+-rw-r--r--   0        0        0     7689 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyt
+-rw-r--r--   0        0        0     4258 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
+-rw-r--r--   0        0        0     4537 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
+-rw-r--r--   0        0        0     4690 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
+-rw-r--r--   0        0        0     5508 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
+-rw-r--r--   0        0        0     1855 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/layer_map.py
+-rw-r--r--   0        0        0     6511 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/layer_stack.py
+-rw-r--r--   0        0        0    10555 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/layer_views.yaml
+-rw-r--r--   0        0        0      158 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/generic_tech/simulation_settings.py
+-rw-r--r--   0        0        0     1431 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/boolean.py
+-rw-r--r--   0        0        0     3814 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/boolean_klayout.py
+-rw-r--r--   0        0        0     1904 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/boolean_polygons.py
+-rw-r--r--   0        0        0      598 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2719 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/check_exclusion.py
+-rw-r--r--   0        0        0     2829 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/check_inclusion.py
+-rw-r--r--   0        0        0     3566 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/check_space.py
+-rw-r--r--   0        0        0     1904 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/check_width.py
+-rw-r--r--   0        0        0     5005 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/fill_klayout.py
+-rw-r--r--   0        0        0     7084 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/fill_tiled.py
+-rw-r--r--   0        0        0     1697 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/fillet.py
+-rw-r--r--   0        0        0     6664 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/functions.py
+-rw-r--r--   0        0        0     2167 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/invert.py
+-rw-r--r--   0        0        0     3685 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/layer_priority.py
+-rw-r--r--   0        0        0     3046 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/manhattanize.py
+-rw-r--r--   0        0        0     4192 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/maskprep.py
+-rw-r--r--   0        0        0     4744 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/maskprep_flat.py
+-rw-r--r--   0        0        0     3250 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/offset.py
+-rw-r--r--   0        0        0     3842 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/outline.py
+-rw-r--r--   0        0        0     2510 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/trim.py
+-rw-r--r--   0        0        0     2948 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/union.py
+-rw-r--r--   0        0        0     9629 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/write_drc.py
+-rw-r--r--   0        0        0     1783 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/geometry/xor_diff.py
+-rw-r--r--   0        0        0     1158 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/get_factories.py
+-rw-r--r--   0        0        0    23561 2023-05-11 23:07:58.975547 gdsfactory-6.93.0/gdsfactory/get_netlist.py
+-rw-r--r--   0        0        0    14426 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/get_netlist_flat.py
+-rw-r--r--   0        0        0      682 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/get_netlist_klayout.py
+-rw-r--r--   0        0        0     9745 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/grid.py
+-rw-r--r--   0        0        0     4363 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/install.py
+-rw-r--r--   0        0        0     1340 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/klive.py
+-rw-r--r--   0        0        0      585 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/labels/__init__.py
+-rw-r--r--   0        0        0     3563 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/labels/add_label_yaml.py
+-rw-r--r--   0        0        0     3847 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/labels/ehva.py
+-rw-r--r--   0        0        0     3810 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/labels/merge_test_metadata.py
+-rw-r--r--   0        0        0     4668 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/labels/siepic.py
+-rw-r--r--   0        0        0     4847 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/labels/write_labels.py
+-rw-r--r--   0        0        0     1149 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/materials.py
+-rw-r--r--   0        0        0     5247 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/name.py
+-rw-r--r--   0        0        0    11586 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/pack.py
+-rw-r--r--   0        0        0    50880 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/path.py
+-rw-r--r--   0        0        0    25849 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/pdk.py
+-rw-r--r--   0        0        0     6170 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/picmodel.py
+-rw-r--r--   0        0        0     5068 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/pixelate.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/plugins/dagster/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/plugins/dagster/workflow.py
+-rw-r--r--   0        0        0      566 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/plugins/database/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/plugins/database/__init__.py
+-rw-r--r--   0        0        0     6216 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/plugins/database/db_upload.py
+-rw-r--r--   0        0        0    16143 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/plugins/database/models.py
+-rw-r--r--   0        0        0    32209 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/port.py
+-rw-r--r--   0        0        0    37609 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/quickplotter.py
+-rw-r--r--   0        0        0      696 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/read/__init__.py
+-rw-r--r--   0        0        0     1639 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/read/from_dphox.py
+-rw-r--r--   0        0        0     1285 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/read/from_gdspaths.py
+-rw-r--r--   0        0        0     1953 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/read/from_np.py
+-rw-r--r--   0        0        0     2813 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/read/from_phidl.py
+-rw-r--r--   0        0        0    38082 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/read/from_yaml.py
+-rw-r--r--   0        0        0     5897 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/read/from_yaml_template.py
+-rw-r--r--   0        0        0     5688 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/read/import_gds.py
+-rw-r--r--   0        0        0     3407 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/read/labels.py
+-rw-r--r--   0        0        0     3769 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/__init__.py
+-rw-r--r--   0        0        0     2920 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/add_electrical_pads_shortest.py
+-rw-r--r--   0        0        0     3015 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/add_electrical_pads_top.py
+-rw-r--r--   0        0        0     3035 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/add_electrical_pads_top_dc.py
+-rw-r--r--   0        0        0     8715 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/add_fiber_array.py
+-rw-r--r--   0        0        0    10624 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/add_fiber_single.py
+-rw-r--r--   0        0        0     8967 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/add_pads.py
+-rw-r--r--   0        0        0    38940 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/all_angle.py
+-rw-r--r--   0        0        0     3916 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/auto_taper.py
+-rw-r--r--   0        0        0      982 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/factories.py
+-rw-r--r--   0        0        0     4415 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/fanout.py
+-rw-r--r--   0        0        0     2800 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/fanout2x2.py
+-rw-r--r--   0        0        0    24342 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_bundle.py
+-rw-r--r--   0        0        0     8632 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_bundle_corner.py
+-rw-r--r--   0        0        0     6900 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_bundle_from_steps.py
+-rw-r--r--   0        0        0    12949 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_bundle_from_waypoints.py
+-rw-r--r--   0        0        0     5284 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_bundle_path_length_match.py
+-rw-r--r--   0        0        0     1937 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_bundle_sbend.py
+-rw-r--r--   0        0        0    17064 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_bundle_u.py
+-rw-r--r--   0        0        0     1510 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_input_labels.py
+-rw-r--r--   0        0        0     9233 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_route.py
+-rw-r--r--   0        0        0    10824 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_route_astar.py
+-rw-r--r--   0        0        0     6119 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_route_from_steps.py
+-rw-r--r--   0        0        0     2766 2023-05-11 23:07:58.979547 gdsfactory-6.93.0/gdsfactory/routing/get_route_sbend.py
+-rw-r--r--   0        0        0     3311 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/get_routes_bend180.py
+-rw-r--r--   0        0        0     1854 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/get_routes_straight.py
+-rw-r--r--   0        0        0    34394 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/manhattan.py
+-rw-r--r--   0        0        0    10081 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/path_length_matching.py
+-rw-r--r--   0        0        0    22568 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/route_fiber_array.py
+-rw-r--r--   0        0        0     8679 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/route_fiber_single.py
+-rw-r--r--   0        0        0    18132 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/route_ports_to_side.py
+-rw-r--r--   0        0        0     4361 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/route_quad.py
+-rw-r--r--   0        0        0    14370 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/route_sharp.py
+-rw-r--r--   0        0        0    10167 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/route_south.py
+-rw-r--r--   0        0        0     5072 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/sort_ports.py
+-rw-r--r--   0        0        0     2477 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/routing/utils.py
+-rw-r--r--   0        0        0     2889 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/01_component_pcell.py
+-rw-r--r--   0        0        0      646 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
+-rw-r--r--   0        0        0     1101 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/01_component_pcell_with_pins.py
+-rw-r--r--   0        0        0      664 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
+-rw-r--r--   0        0        0      347 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/02_component_autoname.py
+-rw-r--r--   0        0        0      887 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/03_move.py
+-rw-r--r--   0        0        0      881 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/04_connect.py
+-rw-r--r--   0        0        0      710 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/05_remove_layers.py
+-rw-r--r--   0        0        0      931 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/06_remapping_layers.py
+-rw-r--r--   0        0        0     1082 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/07_flattening_device.py
+-rw-r--r--   0        0        0      475 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/08_group.py
+-rw-r--r--   0        0        0     1631 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/11_component_layout.py
+-rw-r--r--   0        0        0     2245 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/12_component_refs.py
+-rw-r--r--   0        0        0      955 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/13_component_netlist.py
+-rw-r--r--   0        0        0     2592 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/14_component_connectivity.py
+-rw-r--r--   0        0        0     1636 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/15_component_sequence1.py
+-rw-r--r--   0        0        0     1680 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/16_component_sequence2.py
+-rw-r--r--   0        0        0      965 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/17_ports.py
+-rw-r--r--   0        0        0      489 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/18_port_markers.py
+-rw-r--r--   0        0        0      361 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/19_references.py
+-rw-r--r--   0        0        0      533 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/20_components.py
+-rw-r--r--   0        0        0      507 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/21_add_fiber_array.py
+-rw-r--r--   0        0        0      493 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/22_add_fiber_single.py
+-rw-r--r--   0        0        0      569 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/22_add_pads.py
+-rw-r--r--   0        0        0      848 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/23_reticle.py
+-rw-r--r--   0        0        0     1588 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/23_reticle_passives.py
+-rw-r--r--   0        0        0      457 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/24_doe.py
+-rw-r--r--   0        0        0      687 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/24_doe_2.py
+-rw-r--r--   0        0        0      692 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/24_doe_3.py
+-rw-r--r--   0        0        0      306 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/25_slot_cross_section.py
+-rw-r--r--   0        0        0     1363 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/30_lidar.py
+-rw-r--r--   0        0        0     1412 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/30_lidar_pcell.py
+-rw-r--r--   0        0        0     1943 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/30_lidar_with_pads.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/__init__.py
+-rw-r--r--   0        0        0     1307 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing.py
+-rw-r--r--   0        0        0      558 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
+-rw-r--r--   0        0        0     6062 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
+-rw-r--r--   0        0        0      444 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
+-rw-r--r--   0        0        0      463 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
+-rw-r--r--   0        0        0     1552 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
+-rw-r--r--   0        0        0     1315 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
+-rw-r--r--   0        0        0      602 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
+-rw-r--r--   0        0        0     3317 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
+-rw-r--r--   0        0        0     1484 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
+-rw-r--r--   0        0        0     3045 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
+-rw-r--r--   0        0        0     3782 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
+-rw-r--r--   0        0        0     1988 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/big_device.py
+-rw-r--r--   0        0        0       19 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/Makefile
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/benchmark/fill_demo.py
+-rw-r--r--   0        0        0      343 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
+-rw-r--r--   0        0        0      637 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/circuits/mask.pic.yml
+-rw-r--r--   0        0        0      622 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
+-rw-r--r--   0        0        0      569 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
+-rw-r--r--   0        0        0      453 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/circuits/pads.pic.yml
+-rw-r--r--   0        0        0      287 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
+-rw-r--r--   0        0        0     2260 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/drc_errors.py
+-rw-r--r--   0        0        0     1014 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/drc_write.py
+-rw-r--r--   0        0        0     4530 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/layers.py
+-rw-r--r--   0        0        0      158 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/layers_sky130.py
+-rw-r--r--   0        0        0      364 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/layers_xsection.py
+-rw-r--r--   0        0        0     1062 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/lvs.py
+-rw-r--r--   0        0        0      574 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/demo/pcell.py
+-rw-r--r--   0        0        0     4174 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/netlists/mzi.yml
+-rw-r--r--   0        0        0     5840 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/netlists/mzi_full.yml
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/__init__.py
+-rw-r--r--   0        0        0     4235 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/fab_c.py
+-rw-r--r--   0        0        0      475 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/fab_d/__init__.py
+-rw-r--r--   0        0        0     1880 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
+-rw-r--r--   0        0        0     1715 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c.py
+-rw-r--r--   0        0        0       50 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
+-rw-r--r--   0        0        0       93 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
+-rw-r--r--   0        0        0       85 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
+-rw-r--r--   0        0        0      139 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
+-rw-r--r--   0        0        0       90 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
+-rw-r--r--   0        0        0      126 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
+-rw-r--r--   0        0        0       48 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
+-rw-r--r--   0        0        0     1023 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
+-rw-r--r--   0        0        0     2100 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
+-rw-r--r--   0        0        0     1839 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
+-rw-r--r--   0        0        0     1283 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
+-rw-r--r--   0        0        0     1592 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
+-rw-r--r--   0        0        0     1061 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
+-rw-r--r--   0        0        0     1054 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
+-rw-r--r--   0        0        0     1577 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
+-rw-r--r--   0        0        0     4313 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
+-rw-r--r--   0        0        0     3625 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
+-rw-r--r--   0        0        0     3603 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
+-rw-r--r--   0        0        0     4271 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
+-rw-r--r--   0        0        0      840 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
+-rw-r--r--   0        0        0     2171 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
+-rw-r--r--   0        0        0      316 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/schematic.py
+-rw-r--r--   0        0        0    17692 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/schematic_editor.py
+-rw-r--r--   0        0        0     4194 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/serialization.py
+-rw-r--r--   0        0        0     1612 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/show.py
+-rw-r--r--   0        0        0      724 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/simulation/__init__.py
+-rw-r--r--   0        0        0     4369 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/simulation/add_simulation_markers.py
+-rw-r--r--   0        0        0     2476 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/simulation/convert_sparameters.py
+-rw-r--r--   0        0        0      547 2023-05-11 23:07:58.983547 gdsfactory-6.93.0/gdsfactory/simulation/devsim/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/devsim/doping.py
+-rw-r--r--   0        0        0    11977 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/devsim/get_simulation.py
+-rw-r--r--   0        0        0    23665 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19708 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/devsim/get_solver.py
+-rw-r--r--   0        0        0     1636 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/devsim/test_devsim.py
+-rw-r--r--   0        0        0      189 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/disable_print.py
+-rw-r--r--   0        0        0       79 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/eme/__init__.py
+-rw-r--r--   0        0        0    14784 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/eme/meow_eme.py
+-rw-r--r--   0        0        0     1771 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/eme/test_meow_simulation.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/fem/__init__.py
+-rw-r--r--   0        0        0     8968 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/fem/mode_solver.py
+-rw-r--r--   0        0        0     2205 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/fem/test_mode_solver.py
+-rw-r--r--   0        0        0     3447 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/get_effective_indices.py
+-rw-r--r--   0        0        0     3109 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/get_modes_path.py
+-rw-r--r--   0        0        0     3888 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/get_sparameters_path.py
+-rw-r--r--   0        0        0     2003 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/__init__.py
+-rw-r--r--   0        0        0     3194 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_material.py
+-rw-r--r--   0        0        0     6137 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6054 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    11014 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15915 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    18182 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12302 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11914 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0      832 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6642 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    14053 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    21281 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8143 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9577 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0     1246 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/break_geometry.py
+-rw-r--r--   0        0        0    11250 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/mesh.py
+-rw-r--r--   0        0        0    11808 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/meshtracker.py
+-rw-r--r--   0        0        0     7752 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3644 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/parse_gds.py
+-rw-r--r--   0        0        0     3605 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/parse_layerstack.py
+-rw-r--r--   0        0        0     2990 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/refine.py
+-rw-r--r--   0        0        0    10851 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     2489 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/tests/test_meshing.py
+-rw-r--r--   0        0        0    14168 2023-05-11 23:07:58.987547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     7441 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0    16326 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0     1624 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/get_results.py
+-rw-r--r--   0        0        0    20009 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/get_simulation.py
+-rw-r--r--   0        0        0    21071 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     2821 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/materials.py
+-rw-r--r--   0        0        0    26362 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/modes.py
+-rw-r--r--   0        0        0     8941 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/sim_run.yaml
+-rw-r--r--   0        0        0     8114 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
+-rw-r--r--   0        0        0     8114 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
+-rw-r--r--   0        0        0      728 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py
+-rw-r--r--   0        0        0      262 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      879 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_results.py
+-rw-r--r--   0        0        0     1505 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
+-rw-r--r--   0        0        0     1270 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
+-rw-r--r--   0        0        0     9297 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     1732 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0     1224 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/utils.py
+-rw-r--r--   0        0        0    10515 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/write_sparameters.py
+-rw-r--r--   0        0        0     7695 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0      588 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/lumerical/__init__.py
+-rw-r--r--   0        0        0    16011 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4286 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/lumerical/settings.py
+-rw-r--r--   0        0        0     2348 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/lumerical/test_read_sparameters.py
+-rw-r--r--   0        0        0    19865 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     1504 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0      932 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/__init__.py
+-rw-r--r--   0        0        0     1618 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/coupler.py
+-rw-r--r--   0        0        0     4166 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2773 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     8924 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/find_modes.py
+-rwxr-xr-x   0        0        0     7032 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4458 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2728 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     7138 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4462 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5411 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     8023 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2469 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/overlap.py
+-rw-r--r--   0        0        0      418 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0      548 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1137 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      649 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      354 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0    15492 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/types.py
+-rw-r--r--   0        0        0     1169 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/modes/waveguide.py
+-rw-r--r--   0        0        0     2013 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3081 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0     7332 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/plot.py
+-rw-r--r--   0        0        0     2480 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/plot_csv.py
+-rw-r--r--   0        0        0      703 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/port_symmetries.py
+-rw-r--r--   0        0        0     4637 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/process/diffusion.py
+-rw-r--r--   0        0        0     5317 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/process/implant_tables.py
+-rw-r--r--   0        0        0     6784 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      191 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/sax/__init__.py
+-rw-r--r--   0        0        0    14792 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/sax/build_model.py
+-rw-r--r--   0        0        0     7449 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/sax/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     1571 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/sax/interpolators.py
+-rw-r--r--   0        0        0     6755 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/sax/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4528 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/sax/meow_eme_model.py
+-rw-r--r--   0        0        0     5613 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/sax/mlp.py
+-rw-r--r--   0        0        0     7358 2023-05-11 23:07:58.991547 gdsfactory-6.93.0/gdsfactory/simulation/sax/models.py
+-rw-r--r--   0        0        0    13884 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sax/parameter.py
+-rwxr-xr-x   0        0        0     2205 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sax/plot_model.py
+-rw-r--r--   0        0        0     6805 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sax/read.py
+-rw-r--r--   0        0        0     1350 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2220 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0     1397 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0     1357 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/add_gc.py
+-rw-r--r--   0        0        0     3383 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/circuit.py
+-rw-r--r--   0        0        0      891 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/__init__.py
+-rw-r--r--   0        0        0     1295 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/bend_circular.py
+-rw-r--r--   0        0        0     1388 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/bend_euler.py
+-rw-r--r--   0        0        0     2560 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler.py
+-rw-r--r--   0        0        0     1046 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py
+-rw-r--r--   0        0        0     1848 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler_ring.py
+-rw-r--r--   0        0        0     1329 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
+-rw-r--r--   0        0        0      589 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
+-rw-r--r--   0        0        0      913 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/gc.py
+-rw-r--r--   0        0        0     2032 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/mmi1x2.py
+-rw-r--r--   0        0        0     1910 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/mmi2x2.py
+-rw-r--r--   0        0        0     2618 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/mzi.py
+-rw-r--r--   0        0        0     1759 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/mzi_siepic.py
+-rw-r--r--   0        0        0      487 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/mzi_thermal.py
+-rw-r--r--   0        0        0     2597 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/ring_double.py
+-rw-r--r--   0        0        0     1665 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py
+-rw-r--r--   0        0        0     1782 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/ring_single.py
+-rw-r--r--   0        0        0     1416 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py
+-rw-r--r--   0        0        0     1099 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/straight.py
+-rw-r--r--   0        0        0      800 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/get_transmission.py
+-rw-r--r--   0        0        0     2516 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py
+-rw-r--r--   0        0        0     3841 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/model_from_sparameters.py
+-rw-r--r--   0        0        0     2438 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/plot_circuit.py
+-rw-r--r--   0        0        0     1798 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
+-rw-r--r--   0        0        0     2773 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/plot_model.py
+-rw-r--r--   0        0        0     1261 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_circuit.py
+-rw-r--r--   0        0        0       90 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
+-rw-r--r--   0        0        0     1109 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components.py
+-rw-r--r--   0        0        0       66 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
+-rw-r--r--   0        0        0       69 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
+-rw-r--r--   0        0        0       69 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
+-rw-r--r--   0        0        0       92 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
+-rw-r--r--   0        0        0       92 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
+-rw-r--r--   0        0        0      412 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
+-rw-r--r--   0        0        0      412 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
+-rw-r--r--   0        0        0      114 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
+-rw-r--r--   0        0        0      256 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
+-rw-r--r--   0        0        0      460 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
+-rw-r--r--   0        0        0      104 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
+-rw-r--r--   0        0        0      166 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/simphony/types.py
+-rw-r--r--   0        0        0      471 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sipann/__init__.py
+-rw-r--r--   0        0        0     1376 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sipann/bend_circular.py
+-rw-r--r--   0        0        0     1465 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sipann/bend_euler.py
+-rw-r--r--   0        0        0     2508 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sipann/coupler.py
+-rw-r--r--   0        0        0     1892 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sipann/coupler_ring.py
+-rw-r--r--   0        0        0      736 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/sipann/straight.py
+-rw-r--r--   0        0        0      100 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/thermal/__init__.py
+-rw-r--r--   0        0        0     7781 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/simulation/thermal/heater.py
+-rw-r--r--   0        0        0     1744 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/snap.py
+-rw-r--r--   0        0        0     4245 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/symbols.py
+-rw-r--r--   0        0        0      524 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/technology/__init__.py
+-rw-r--r--   0        0        0     7065 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/technology/klayout_tech.py
+-rw-r--r--   0        0        0     1078 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/technology/layer_map.py
+-rw-r--r--   0        0        0    14989 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/technology/layer_stack.py
+-rw-r--r--   0        0        0    42052 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/technology/layer_views.py
+-rw-r--r--   0        0        0     1984 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/technology/simulation_settings.py
+-rw-r--r--   0        0        0     1635 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/types.py
+-rw-r--r--   0        0        0    10000 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/typings.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/utils/__init__.py
+-rw-r--r--   0        0        0     1304 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/utils/async_utils.py
+-rw-r--r--   0        0        0      376 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/utils/color_utils.py
+-rw-r--r--   0        0        0      558 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/utils/file_utils.py
+-rw-r--r--   0        0        0      185 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/utils/function_utils.py
+-rw-r--r--   0        0        0      676 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/utils/xml_utils.py
+-rw-r--r--   0        0        0     1429 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/utils/yaml_utils.py
+-rw-r--r--   0        0        0     4825 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/watch.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/widgets/__init__.py
+-rw-r--r--   0        0        0     7921 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/widgets/layout_viewer.py
+-rw-r--r--   0        0        0     7464 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/gdsfactory/write_cells.py
+-rw-r--r--   0        0        0     5467 2023-05-11 23:07:58.995547 gdsfactory-6.93.0/pyproject.toml
+-rw-r--r--   0        0        0    18552 1970-01-01 00:00:00.000000 gdsfactory-6.93.0/PKG-INFO
```

### Comparing `gdsfactory-6.92.2/LICENSE` & `gdsfactory-6.93.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/README.md` & `gdsfactory-6.93.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gdsfactory 6.92.2
+# gdsfactory 6.93.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
```

### Comparing `gdsfactory-6.92.2/gdsfactory/__init__.py` & `gdsfactory-6.93.0/gdsfactory/__init__.py`

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
-__version__ = "6.92.2"
+__version__ = "6.93.0"
```

### Comparing `gdsfactory-6.92.2/gdsfactory/add_keepout.py` & `gdsfactory-6.93.0/gdsfactory/add_keepout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/add_labels.py` & `gdsfactory-6.93.0/gdsfactory/add_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/add_loopback.py` & `gdsfactory-6.93.0/gdsfactory/add_loopback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/add_padding.py` & `gdsfactory-6.93.0/gdsfactory/add_padding.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/add_pins.py` & `gdsfactory-6.93.0/gdsfactory/add_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/add_ports.py` & `gdsfactory-6.93.0/gdsfactory/add_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/add_tapers.py` & `gdsfactory-6.93.0/gdsfactory/add_tapers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/add_tapers_cross_section.py` & `gdsfactory-6.93.0/gdsfactory/add_tapers_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/add_termination.py` & `gdsfactory-6.93.0/gdsfactory/add_termination.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/asserts.py` & `gdsfactory-6.93.0/gdsfactory/asserts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/cell.py` & `gdsfactory-6.93.0/gdsfactory/cell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/circuitviz.py` & `gdsfactory-6.93.0/gdsfactory/circuitviz.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/cli.py` & `gdsfactory-6.93.0/gdsfactory/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gdsfactory.write_cells import write_cells as write_cells_to_separate_gds
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
-VERSION = "6.92.2"
+VERSION = "6.93.0"
 LAYER_LABEL = LAYER.LABEL
 
 
 def print_version(ctx: Context, param: Option, value: bool) -> None:
     """Prints the version."""
     if not value or ctx.resilient_parsing:
         return
```

### Comparing `gdsfactory-6.92.2/gdsfactory/component.py` & `gdsfactory-6.93.0/gdsfactory/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -2112,4088 +2112,4173 @@
 000083f0: 6c79 676f 6e28 706f 6c79 676f 6e2e 706f  lygon(polygon.po
 00008400: 696e 7473 2c20 6c61 7965 722c 2064 6174  ints, layer, dat
 00008410: 6174 7970 6529 0a20 2020 2020 2020 2020  atype).         
 00008420: 2020 2073 656c 662e 5f61 6464 5f70 6f6c     self._add_pol
 00008430: 7967 6f6e 7328 706f 6c79 676f 6e29 0a20  ygons(polygon). 
 00008440: 2020 2020 2020 2020 2020 2072 6574 7572             retur
 00008450: 6e20 706f 6c79 676f 6e0a 0a20 2020 2020  n polygon..     
-00008460: 2020 2070 6f69 6e74 7320 3d20 6e70 2e61     points = np.a
-00008470: 7361 7272 6179 2870 6f69 6e74 7329 0a20  sarray(points). 
-00008480: 2020 2020 2020 2069 6620 706f 696e 7473         if points
-00008490: 2e6e 6469 6d20 3d3d 2031 3a0a 2020 2020  .ndim == 1:.    
-000084a0: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-000084b0: 7365 6c66 2e61 6464 5f70 6f6c 7967 6f6e  self.add_polygon
-000084c0: 2870 6f6c 792c 206c 6179 6572 3d6c 6179  (poly, layer=lay
-000084d0: 6572 2920 666f 7220 706f 6c79 2069 6e20  er) for poly in 
-000084e0: 706f 696e 7473 5d0a 2020 2020 2020 2020  points].        
-000084f0: 6966 206c 6179 6572 2069 7320 6e70 2e6e  if layer is np.n
-00008500: 616e 3a0a 2020 2020 2020 2020 2020 2020  an:.            
-00008510: 6c61 7965 7220 3d20 300a 0a20 2020 2020  layer = 0..     
-00008520: 2020 2069 6620 706f 696e 7473 2e6e 6469     if points.ndi
-00008530: 6d20 3d3d 2032 3a0a 2020 2020 2020 2020  m == 2:.        
-00008540: 2020 2020 2320 6164 6420 7369 6e67 6c65      # add single
-00008550: 2070 6f6c 7967 6f6e 2066 726f 6d20 706f   polygon from po
-00008560: 696e 7473 0a20 2020 2020 2020 2020 2020  ints.           
-00008570: 2069 6620 6c65 6e28 706f 696e 7473 5b30   if len(points[0
-00008580: 5d29 203e 2032 3a0a 2020 2020 2020 2020  ]) > 2:.        
-00008590: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
-000085a0: 7420 746f 2066 6f72 6d20 5b5b 312c 325d  t to form [[1,2]
-000085b0: 2c5b 332c 345d 2c5b 352c 365d 5d0a 2020  ,[3,4],[5,6]].  
-000085c0: 2020 2020 2020 2020 2020 2020 2020 706f                po
-000085d0: 696e 7473 203d 206e 702e 636f 6c75 6d6e  ints = np.column
-000085e0: 5f73 7461 636b 2870 6f69 6e74 7329 0a20  _stack(points). 
-000085f0: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-00008600: 2c20 6461 7461 7479 7065 203d 205f 7061  , datatype = _pa
-00008610: 7273 655f 6c61 7965 7228 6c61 7965 7229  rse_layer(layer)
-00008620: 0a20 2020 2020 2020 2020 2020 2070 6f6c  .            pol
-00008630: 7967 6f6e 203d 2050 6f6c 7967 6f6e 2870  ygon = Polygon(p
-00008640: 6f69 6e74 732c 206c 6179 6572 3d6c 6179  oints, layer=lay
-00008650: 6572 2c20 6461 7461 7479 7065 3d64 6174  er, datatype=dat
-00008660: 6174 7970 6529 0a20 2020 2020 2020 2020  atype).         
-00008670: 2020 2073 656c 662e 5f61 6464 5f70 6f6c     self._add_pol
-00008680: 7967 6f6e 7328 706f 6c79 676f 6e29 0a20  ygons(polygon). 
-00008690: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000086a0: 6e20 706f 6c79 676f 6e0a 2020 2020 2020  n polygon.      
-000086b0: 2020 656c 6966 2070 6f69 6e74 732e 6e64    elif points.nd
-000086c0: 696d 203d 3d20 333a 0a20 2020 2020 2020  im == 3:.       
-000086d0: 2020 2020 206c 6179 6572 2c20 6461 7461       layer, data
-000086e0: 7479 7065 203d 205f 7061 7273 655f 6c61  type = _parse_la
-000086f0: 7965 7228 6c61 7965 7229 0a20 2020 2020  yer(layer).     
-00008700: 2020 2020 2020 2070 6f6c 7967 6f6e 7320         polygons 
-00008710: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00008720: 2020 2020 506f 6c79 676f 6e28 7070 6f69      Polygon(ppoi
-00008730: 6e74 732c 206c 6179 6572 3d6c 6179 6572  nts, layer=layer
-00008740: 2c20 6461 7461 7479 7065 3d64 6174 6174  , datatype=datat
-00008750: 7970 6529 2066 6f72 2070 706f 696e 7473  ype) for ppoints
-00008760: 2069 6e20 706f 696e 7473 0a20 2020 2020   in points.     
-00008770: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00008780: 2020 2020 2073 656c 662e 5f61 6464 5f70       self._add_p
-00008790: 6f6c 7967 6f6e 7328 2a70 6f6c 7967 6f6e  olygons(*polygon
-000087a0: 7329 0a20 2020 2020 2020 2020 2020 2072  s).            r
-000087b0: 6574 7572 6e20 706f 6c79 676f 6e73 0a20  eturn polygons. 
-000087c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000087d0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-000087e0: 616c 7565 4572 726f 7228 6622 556e 6162  alueError(f"Unab
-000087f0: 6c65 2074 6f20 6164 6420 7b70 6f69 6e74  le to add {point
-00008800: 732e 6e64 696d 7d2d 6469 6d65 6e73 696f  s.ndim}-dimensio
-00008810: 6e61 6c20 706f 696e 7473 206f 626a 6563  nal points objec
-00008820: 7422 290a 0a20 2020 2064 6566 205f 6164  t")..    def _ad
-00008830: 645f 706f 6c79 676f 6e73 2873 656c 662c  d_polygons(self,
-00008840: 202a 706f 6c79 676f 6e73 3a20 4c69 7374   *polygons: List
-00008850: 5b50 6f6c 7967 6f6e 5d29 3a0a 2020 2020  [Polygon]):.    
-00008860: 2020 2020 7365 6c66 2e69 735f 756e 6c6f      self.is_unlo
-00008870: 636b 6564 2829 0a20 2020 2020 2020 2073  cked().        s
-00008880: 656c 662e 5f63 656c 6c2e 6164 6428 2a70  elf._cell.add(*p
-00008890: 6f6c 7967 6f6e 7329 0a0a 2020 2020 6465  olygons)..    de
-000088a0: 6620 636f 7079 2873 656c 6629 202d 3e20  f copy(self) -> 
-000088b0: 436f 6d70 6f6e 656e 743a 0a20 2020 2020  Component:.     
-000088c0: 2020 2072 6574 7572 6e20 636f 7079 2873     return copy(s
-000088d0: 656c 6629 0a0a 2020 2020 6465 6620 6164  elf)..    def ad
-000088e0: 645f 7265 665f 636f 6e74 6169 6e65 7228  d_ref_container(
-000088f0: 7365 6c66 2c20 636f 6d70 6f6e 656e 743a  self, component:
-00008900: 2043 6f6d 706f 6e65 6e74 2920 2d3e 2043   Component) -> C
-00008910: 6f6d 706f 6e65 6e74 5265 6665 7265 6e63  omponentReferenc
-00008920: 653a 0a20 2020 2020 2020 2022 2222 4164  e:.        """Ad
-00008930: 6420 7265 6665 7265 6e63 652c 2070 6f72  d reference, por
-00008940: 7473 2061 6e64 2063 6f70 795f 6368 696c  ts and copy_chil
-00008950: 645f 696e 666f 2e22 2222 0a20 2020 2020  d_info.""".     
-00008960: 2020 2072 6566 203d 2073 656c 6620 3c3c     ref = self <<
-00008970: 2063 6f6d 706f 6e65 6e74 0a20 2020 2020   component.     
-00008980: 2020 2073 656c 662e 6164 645f 706f 7274     self.add_port
-00008990: 7328 7265 662e 706f 7274 7329 0a20 2020  s(ref.ports).   
-000089a0: 2020 2020 2073 656c 662e 636f 7079 5f63       self.copy_c
-000089b0: 6869 6c64 5f69 6e66 6f28 636f 6d70 6f6e  hild_info(compon
-000089c0: 656e 7429 0a20 2020 2020 2020 2072 6574  ent).        ret
-000089d0: 7572 6e20 7265 660a 0a20 2020 2064 6566  urn ref..    def
-000089e0: 2063 6f70 795f 6368 696c 645f 696e 666f   copy_child_info
-000089f0: 2873 656c 662c 2063 6f6d 706f 6e65 6e74  (self, component
-00008a00: 3a20 436f 6d70 6f6e 656e 7429 202d 3e20  : Component) -> 
-00008a10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00008a20: 2243 6f70 7920 616e 6420 7365 7474 696e  "Copy and settin
-00008a30: 6773 2069 6e66 6f20 6672 6f6d 2063 6869  gs info from chi
-00008a40: 6c64 2063 6f6d 706f 6e65 6e74 2069 6e74  ld component int
-00008a50: 6f20 7061 7265 6e74 2e0a 0a20 2020 2020  o parent...     
-00008a60: 2020 2050 6172 656e 7420 636f 6d70 6f6e     Parent compon
-00008a70: 656e 7473 2063 616e 2061 6363 6573 7320  ents can access 
-00008a80: 6368 696c 6420 6365 6c6c 7320 7365 7474  child cells sett
-00008a90: 696e 6773 2e0a 2020 2020 2020 2020 2222  ings..        ""
-00008aa0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-00008ab0: 2069 7369 6e73 7461 6e63 6528 636f 6d70   isinstance(comp
-00008ac0: 6f6e 656e 742c 2028 436f 6d70 6f6e 656e  onent, (Componen
-00008ad0: 742c 2043 6f6d 706f 6e65 6e74 5265 6665  t, ComponentRefe
-00008ae0: 7265 6e63 6529 293a 0a20 2020 2020 2020  rence)):.       
-00008af0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00008b00: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00008b10: 2020 2020 2020 2066 227b 7479 7065 2863         f"{type(c
-00008b20: 6f6d 706f 6e65 6e74 297d 2220 2269 7320  omponent)}" "is 
-00008b30: 6e6f 7420 6120 436f 6d70 6f6e 656e 7420  not a Component 
-00008b40: 6f72 2043 6f6d 706f 6e65 6e74 5265 6665  or ComponentRefe
-00008b50: 7265 6e63 6522 0a20 2020 2020 2020 2020  rence".         
-00008b60: 2020 2029 0a0a 2020 2020 2020 2020 7365     )..        se
-00008b70: 6c66 2e67 6574 5f63 6869 6c64 5f6e 616d  lf.get_child_nam
-00008b80: 6520 3d20 5472 7565 0a20 2020 2020 2020  e = True.       
-00008b90: 2073 656c 662e 6368 696c 6420 3d20 636f   self.child = co
-00008ba0: 6d70 6f6e 656e 740a 2020 2020 2020 2020  mponent.        
-00008bb0: 7365 6c66 2e69 6e66 6f2e 7570 6461 7465  self.info.update
-00008bc0: 2863 6f6d 706f 6e65 6e74 2e69 6e66 6f29  (component.info)
-00008bd0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00008be0: 7474 696e 6773 2e75 7064 6174 6528 636f  ttings.update(co
-00008bf0: 6d70 6f6e 656e 742e 7365 7474 696e 6773  mponent.settings
-00008c00: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-00008c10: 0a20 2020 2064 6566 2073 697a 655f 696e  .    def size_in
-00008c20: 666f 2873 656c 6629 202d 3e20 5369 7a65  fo(self) -> Size
-00008c30: 496e 666f 3a0a 2020 2020 2020 2020 2222  Info:.        ""
-00008c40: 2253 697a 6520 696e 666f 206f 6620 7468  "Size info of th
-00008c50: 6520 636f 6d70 6f6e 656e 742e 2222 220a  e component.""".
-00008c60: 2020 2020 2020 2020 7265 7475 726e 2053          return S
-00008c70: 697a 6549 6e66 6f28 7365 6c66 2e62 626f  izeInfo(self.bbo
-00008c80: 7829 0a0a 2020 2020 6465 6620 6765 745f  x)..    def get_
-00008c90: 7365 7474 696e 6728 7365 6c66 2c20 7365  setting(self, se
-00008ca0: 7474 696e 673a 2073 7472 2920 2d3e 2055  tting: str) -> U
-00008cb0: 6e69 6f6e 5b73 7472 2c20 696e 742c 2066  nion[str, int, f
-00008cc0: 6c6f 6174 5d3a 0a20 2020 2020 2020 2072  loat]:.        r
-00008cd0: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
-00008ce0: 2020 2020 7365 6c66 2e69 6e66 6f2e 6765      self.info.ge
-00008cf0: 7428 7365 7474 696e 6729 0a20 2020 2020  t(setting).     
-00008d00: 2020 2020 2020 206f 7220 7365 6c66 2e73         or self.s
-00008d10: 6574 7469 6e67 732e 6675 6c6c 2e67 6574  ettings.full.get
-00008d20: 2873 6574 7469 6e67 290a 2020 2020 2020  (setting).      
-00008d30: 2020 2020 2020 6f72 2073 656c 662e 6d65        or self.me
-00008d40: 7461 6461 7461 5f63 6869 6c64 2e67 6574  tadata_child.get
-00008d50: 2873 6574 7469 6e67 290a 2020 2020 2020  (setting).      
-00008d60: 2020 290a 0a20 2020 2064 6566 2069 735f    )..    def is_
-00008d70: 756e 6c6f 636b 6564 2873 656c 6629 202d  unlocked(self) -
-00008d80: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00008d90: 2222 2252 6169 7365 7320 6572 726f 7220  """Raises error 
-00008da0: 6966 2043 6f6d 706f 6e65 6e74 2069 7320  if Component is 
-00008db0: 6c6f 636b 6564 2e22 2222 0a20 2020 2020  locked.""".     
-00008dc0: 2020 2069 6620 7365 6c66 2e5f 6c6f 636b     if self._lock
-00008dd0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-00008de0: 7261 6973 6520 4d75 7461 6269 6c69 7479  raise Mutability
-00008df0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00008e00: 2020 2020 2020 2066 2243 6f6d 706f 6e65         f"Compone
-00008e10: 6e74 207b 7365 6c66 2e6e 616d 6521 727d  nt {self.name!r}
-00008e20: 2063 616e 6e6f 7420 6265 206d 6f64 6966   cannot be modif
-00008e30: 6965 6420 6173 2069 7427 7320 616c 7265  ied as it's alre
-00008e40: 6164 7920 6f6e 2063 6163 6865 2e20 220a  ady on cache. ".
-00008e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e60: 2b20 6d75 7461 6269 6c69 7479 5f65 7272  + mutability_err
-00008e70: 6f72 5f6d 6573 7361 6765 0a20 2020 2020  or_message.     
-00008e80: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00008e90: 6620 5f61 6464 2873 656c 662c 2065 6c65  f _add(self, ele
-00008ea0: 6d65 6e74 2920 2d3e 204e 6f6e 653a 0a20  ment) -> None:. 
-00008eb0: 2020 2020 2020 2022 2222 4164 6420 6120         """Add a 
-00008ec0: 6e65 7720 656c 656d 656e 7420 6f72 206c  new element or l
-00008ed0: 6973 7420 6f66 2065 6c65 6d65 6e74 7320  ist of elements 
-00008ee0: 746f 2074 6869 7320 436f 6d70 6f6e 656e  to this Componen
-00008ef0: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
-00008f00: 3a0a 2020 2020 2020 2020 2020 2020 656c  :.            el
-00008f10: 656d 656e 743a 2050 6f6c 7967 6f6e 2c20  ement: Polygon, 
-00008f20: 436f 6d70 6f6e 656e 7452 6566 6572 656e  ComponentReferen
-00008f30: 6365 206f 7220 6974 6572 6162 6c65 0a20  ce or iterable. 
-00008f40: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00008f50: 6865 2065 6c65 6d65 6e74 206f 7220 6974  he element or it
-00008f60: 6572 6162 6c65 206f 6620 656c 656d 656e  erable of elemen
-00008f70: 7473 2074 6f20 6265 2069 6e73 6572 7465  ts to be inserte
-00008f80: 6420 696e 2074 6869 7320 6365 6c6c 2e0a  d in this cell..
-00008f90: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-00008fa0: 0a20 2020 2020 2020 2020 2020 204d 7574  .            Mut
-00008fb0: 6162 696c 6974 7945 7272 6f72 3a20 6966  abilityError: if
-00008fc0: 2063 6f6d 706f 6e65 6e74 2069 7320 6c6f   component is lo
-00008fd0: 636b 6564 2e0a 2020 2020 2020 2020 2222  cked..        ""
-00008fe0: 220a 2020 2020 2020 2020 7365 6c66 2e69  ".        self.i
-00008ff0: 735f 756e 6c6f 636b 6564 2829 0a20 2020  s_unlocked().   
-00009000: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00009010: 6365 2865 6c65 6d65 6e74 2c20 436f 6d70  ce(element, Comp
-00009020: 6f6e 656e 7452 6566 6572 656e 6365 293a  onentReference):
-00009030: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00009040: 662e 5f63 656c 6c2e 6164 6428 656c 656d  f._cell.add(elem
-00009050: 656e 742e 5f72 6566 6572 656e 6365 290a  ent._reference).
-00009060: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009070: 2e5f 7265 6665 7265 6e63 6573 2e61 7070  ._references.app
-00009080: 656e 6428 656c 656d 656e 7429 0a20 2020  end(element).   
-00009090: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000090a0: 2020 2020 2020 2073 656c 662e 5f63 656c         self._cel
-000090b0: 6c2e 6164 6428 656c 656d 656e 7429 0a0a  l.add(element)..
-000090c0: 2020 2020 6465 6620 6164 6428 7365 6c66      def add(self
-000090d0: 2c20 656c 656d 656e 7429 202d 3e20 4e6f  , element) -> No
-000090e0: 6e65 3a0a 2020 2020 2020 2020 2222 2241  ne:.        """A
-000090f0: 6464 2061 206e 6577 2065 6c65 6d65 6e74  dd a new element
-00009100: 206f 7220 6c69 7374 206f 6620 656c 656d   or list of elem
-00009110: 656e 7473 2074 6f20 7468 6973 2043 6f6d  ents to this Com
-00009120: 706f 6e65 6e74 2e0a 0a20 2020 2020 2020  ponent...       
-00009130: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00009140: 2020 2065 6c65 6d65 6e74 3a20 506f 6c79     element: Poly
-00009150: 676f 6e2c 2043 6f6d 706f 6e65 6e74 5265  gon, ComponentRe
-00009160: 6665 7265 6e63 6520 6f72 2069 7465 7261  ference or itera
-00009170: 626c 650a 2020 2020 2020 2020 2020 2020  ble.            
-00009180: 2020 2020 5468 6520 656c 656d 656e 7420      The element 
-00009190: 6f72 2069 7465 7261 626c 6520 6f66 2065  or iterable of e
-000091a0: 6c65 6d65 6e74 7320 746f 2062 6520 696e  lements to be in
-000091b0: 7365 7274 6564 2069 6e20 7468 6973 2063  serted in this c
-000091c0: 656c 6c2e 0a0a 2020 2020 2020 2020 5261  ell...        Ra
-000091d0: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-000091e0: 2020 4d75 7461 6269 6c69 7479 4572 726f    MutabilityErro
-000091f0: 723a 2069 6620 636f 6d70 6f6e 656e 7420  r: if component 
-00009200: 6973 206c 6f63 6b65 642e 0a20 2020 2020  is locked..     
-00009210: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00009220: 6620 6973 696e 7374 616e 6365 2865 6c65  f isinstance(ele
-00009230: 6d65 6e74 2c20 436f 6d70 6f6e 656e 7452  ment, ComponentR
-00009240: 6566 6572 656e 6365 293a 0a20 2020 2020  eference):.     
-00009250: 2020 2020 2020 2073 656c 662e 5f72 6567         self._reg
-00009260: 6973 7465 725f 7265 6665 7265 6e63 6528  ister_reference(
-00009270: 656c 656d 656e 7429 0a20 2020 2020 2020  element).       
-00009280: 2020 2020 2073 656c 662e 5f61 6464 2865       self._add(e
-00009290: 6c65 6d65 6e74 290a 2020 2020 2020 2020  lement).        
-000092a0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-000092b0: 656c 656d 656e 742c 2049 7465 7261 626c  element, Iterabl
-000092c0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-000092d0: 666f 7220 7375 6265 6c65 6d65 6e74 2069  for subelement i
-000092e0: 6e20 656c 656d 656e 743a 0a20 2020 2020  n element:.     
-000092f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009300: 6164 6428 7375 6265 6c65 6d65 6e74 290a  add(subelement).
-00009310: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00009320: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009330: 6164 6428 656c 656d 656e 7429 0a0a 2020  add(element)..  
-00009340: 2020 6465 6620 6164 645f 6172 7261 7928    def add_array(
-00009350: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00009360: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
-00009370: 3a20 436f 6d70 6f6e 656e 742c 0a20 2020  : Component,.   
-00009380: 2020 2020 2063 6f6c 756d 6e73 3a20 696e       columns: in
-00009390: 7420 3d20 322c 0a20 2020 2020 2020 2072  t = 2,.        r
-000093a0: 6f77 733a 2069 6e74 203d 2032 2c0a 2020  ows: int = 2,.  
-000093b0: 2020 2020 2020 7370 6163 696e 673a 2054        spacing: T
-000093c0: 7570 6c65 5b66 6c6f 6174 2c20 666c 6f61  uple[float, floa
-000093d0: 745d 203d 2028 3130 302c 2031 3030 292c  t] = (100, 100),
-000093e0: 0a20 2020 2020 2020 2061 6c69 6173 3a20  .        alias: 
-000093f0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00009400: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2043  None,.    ) -> C
-00009410: 6f6d 706f 6e65 6e74 5265 6665 7265 6e63  omponentReferenc
-00009420: 653a 0a20 2020 2020 2020 2022 2222 4372  e:.        """Cr
-00009430: 6561 7465 7320 6120 436f 6d70 6f6e 656e  eates a Componen
-00009440: 7452 6566 6572 656e 6365 2072 6566 6572  tReference refer
-00009450: 656e 6365 2074 6f20 6120 436f 6d70 6f6e  ence to a Compon
-00009460: 656e 742e 0a0a 2020 2020 2020 2020 4172  ent...        Ar
-00009470: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00009480: 636f 6d70 6f6e 656e 743a 2054 6865 2072  component: The r
-00009490: 6566 6572 656e 6365 6420 636f 6d70 6f6e  eferenced compon
-000094a0: 656e 742e 0a20 2020 2020 2020 2020 2020  ent..           
-000094b0: 2063 6f6c 756d 6e73 3a20 4e75 6d62 6572   columns: Number
-000094c0: 206f 6620 636f 6c75 6d6e 7320 696e 2074   of columns in t
-000094d0: 6865 2061 7272 6179 2e0a 2020 2020 2020  he array..      
-000094e0: 2020 2020 2020 726f 7773 3a20 4e75 6d62        rows: Numb
-000094f0: 6572 206f 6620 726f 7773 2069 6e20 7468  er of rows in th
-00009500: 6520 6172 7261 792e 0a20 2020 2020 2020  e array..       
-00009510: 2020 2020 2073 7061 6369 6e67 3a20 6172       spacing: ar
-00009520: 7261 792d 6c69 6b65 5b32 5d20 6f66 2069  ray-like[2] of i
-00009530: 6e74 206f 7220 666c 6f61 742e 0a20 2020  nt or float..   
-00009540: 2020 2020 2020 2020 2020 2020 2044 6973               Dis
-00009550: 7461 6e63 6520 6265 7477 6565 6e20 6164  tance between ad
-00009560: 6a61 6365 6e74 2063 6f6c 756d 6e73 2061  jacent columns a
-00009570: 6e64 2061 646a 6163 656e 7420 726f 7773  nd adjacent rows
-00009580: 2e0a 2020 2020 2020 2020 2020 2020 616c  ..            al
-00009590: 6961 733a 2073 7472 206f 7220 4e6f 6e65  ias: str or None
-000095a0: 2e20 416c 6961 7320 6f66 2074 6865 2072  . Alias of the r
-000095b0: 6566 6572 656e 6365 6420 436f 6d70 6f6e  eferenced Compon
-000095c0: 656e 742e 0a0a 2020 2020 2020 2020 5265  ent...        Re
-000095d0: 7475 726e 730a 2020 2020 2020 2020 2020  turns.          
-000095e0: 2020 613a 2043 6f6d 706f 6e65 6e74 5265    a: ComponentRe
-000095f0: 6665 7265 6e63 6520 636f 6e74 6169 6e69  ference containi
-00009600: 6e67 2072 6566 6572 656e 6365 7320 746f  ng references to
-00009610: 2074 6865 2043 6f6d 706f 6e65 6e74 2e0a   the Component..
-00009620: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009630: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-00009640: 7461 6e63 6528 636f 6d70 6f6e 656e 742c  tance(component,
-00009650: 2043 6f6d 706f 6e65 6e74 293a 0a20 2020   Component):.   
-00009660: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00009670: 7970 6545 7272 6f72 2822 6164 645f 6172  ypeError("add_ar
-00009680: 7261 7928 2920 6e65 6564 7320 6120 436f  ray() needs a Co
-00009690: 6d70 6f6e 656e 7420 6f62 6a65 6374 2e22  mponent object."
-000096a0: 290a 2020 2020 2020 2020 7265 6620 3d20  ).        ref = 
-000096b0: 436f 6d70 6f6e 656e 7452 6566 6572 656e  ComponentReferen
-000096c0: 6365 280a 2020 2020 2020 2020 2020 2020  ce(.            
-000096d0: 636f 6d70 6f6e 656e 743d 636f 6d70 6f6e  component=compon
-000096e0: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
-000096f0: 2063 6f6c 756d 6e73 3d69 6e74 2872 6f75   columns=int(rou
-00009700: 6e64 2863 6f6c 756d 6e73 2929 2c0a 2020  nd(columns)),.  
-00009710: 2020 2020 2020 2020 2020 726f 7773 3d69            rows=i
-00009720: 6e74 2872 6f75 6e64 2872 6f77 7329 292c  nt(round(rows)),
-00009730: 0a20 2020 2020 2020 2020 2020 2073 7061  .            spa
-00009740: 6369 6e67 3d73 7061 6369 6e67 2c0a 2020  cing=spacing,.  
-00009750: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00009760: 7265 662e 6e61 6d65 203d 204e 6f6e 650a  ref.name = None.
-00009770: 2020 2020 2020 2020 7365 6c66 2e5f 6164          self._ad
-00009780: 6428 7265 6629 0a20 2020 2020 2020 2073  d(ref).        s
-00009790: 656c 662e 5f72 6567 6973 7465 725f 7265  elf._register_re
-000097a0: 6665 7265 6e63 6528 7265 6665 7265 6e63  ference(referenc
-000097b0: 653d 7265 662c 2061 6c69 6173 3d61 6c69  e=ref, alias=ali
-000097c0: 6173 290a 2020 2020 2020 2020 7265 7475  as).        retu
-000097d0: 726e 2072 6566 0a0a 2020 2020 6465 6620  rn ref..    def 
-000097e0: 6469 7374 7269 6275 7465 280a 2020 2020  distribute(.    
-000097f0: 2020 2020 7365 6c66 2c20 656c 656d 656e      self, elemen
-00009800: 7473 3d22 616c 6c22 2c20 6469 7265 6374  ts="all", direct
-00009810: 696f 6e3d 2278 222c 2073 7061 6369 6e67  ion="x", spacing
-00009820: 3d31 3030 2c20 7365 7061 7261 7469 6f6e  =100, separation
-00009830: 3d54 7275 652c 2065 6467 653d 2263 656e  =True, edge="cen
-00009840: 7465 7222 0a20 2020 2029 3a0a 2020 2020  ter".    ):.    
-00009850: 2020 2020 2222 2244 6973 7472 6962 7574      """Distribut
-00009860: 6573 2074 6865 2073 7065 6369 6669 6564  es the specified
-00009870: 2065 6c65 6d65 6e74 7320 696e 2074 6865   elements in the
-00009880: 2043 6f6d 706f 6e65 6e74 2e0a 0a20 2020   Component...   
-00009890: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-000098a0: 2020 2020 2020 2065 6c65 6d65 6e74 7320         elements 
-000098b0: 3a20 6172 7261 792d 6c69 6b65 206f 6620  : array-like of 
-000098c0: 6f62 6a65 6374 7320 6f72 2027 616c 6c27  objects or 'all'
-000098d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000098e0: 2045 6c65 6d65 6e74 7320 746f 2064 6973   Elements to dis
-000098f0: 7472 6962 7574 652e 0a20 2020 2020 2020  tribute..       
-00009900: 2020 2020 2064 6972 6563 7469 6f6e 203a       direction :
-00009910: 207b 2778 272c 2027 7927 7d0a 2020 2020   {'x', 'y'}.    
-00009920: 2020 2020 2020 2020 2020 2020 4469 7265              Dire
-00009930: 6374 696f 6e20 6f66 2064 6973 7472 6962  ction of distrib
-00009940: 7574 696f 6e3b 2065 6974 6865 7220 6120  ution; either a 
-00009950: 6c69 6e65 2069 6e20 7468 6520 782d 6469  line in the x-di
-00009960: 7265 6374 696f 6e20 6f72 0a20 2020 2020  rection or.     
-00009970: 2020 2020 2020 2020 2020 2079 2d64 6972             y-dir
-00009980: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
-00009990: 2020 2020 7370 6163 696e 6720 3a20 696e      spacing : in
-000099a0: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
-000099b0: 2020 2020 2020 2020 2020 2044 6973 7461             Dista
-000099c0: 6e63 6520 6265 7477 6565 6e20 656c 656d  nce between elem
-000099d0: 656e 7473 2e0a 2020 2020 2020 2020 2020  ents..          
-000099e0: 2020 7365 7061 7261 7469 6f6e 203a 2062    separation : b
-000099f0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-00009a00: 2020 2020 4966 2054 7275 652c 2067 7561      If True, gua
-00009a10: 7261 6e74 6565 7320 656c 656d 656e 7473  rantees elements
-00009a20: 2061 7265 2073 6570 6172 6174 6564 2077   are separated w
-00009a30: 6974 6820 6120 6669 7865 6420 7370 6163  ith a fixed spac
-00009a40: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00009a50: 2020 2020 6265 7477 6565 6e3b 2069 6620      between; if 
-00009a60: 2046 616c 7365 2c20 656c 656d 656e 7473   False, elements
-00009a70: 2061 7265 2073 7061 6365 6420 6576 656e   are spaced even
-00009a80: 6c79 2061 6c6f 6e67 2061 2067 7269 642e  ly along a grid.
-00009a90: 0a20 2020 2020 2020 2020 2020 2065 6467  .            edg
-00009aa0: 6520 3a20 7b27 7827 2c20 2778 6d69 6e27  e : {'x', 'xmin'
-00009ab0: 2c20 2778 6d61 7827 2c20 2779 272c 2027  , 'xmax', 'y', '
-00009ac0: 796d 696e 272c 2027 796d 6178 277d 0a20  ymin', 'ymax'}. 
-00009ad0: 2020 2020 2020 2020 2020 2020 2020 2057                 W
-00009ae0: 6869 6368 2065 6467 6520 746f 2070 6572  hich edge to per
-00009af0: 666f 726d 2074 6865 2064 6973 7472 6962  form the distrib
-00009b00: 7574 696f 6e20 616c 6f6e 6720 2875 6e75  ution along (unu
-00009b10: 7365 6420 6966 0a20 2020 2020 2020 2020  sed if.         
-00009b20: 2020 2020 2020 2073 6570 6172 6174 696f         separatio
-00009b30: 6e20 3d3d 2054 7275 6529 0a0a 2020 2020  n == True)..    
-00009b40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00009b50: 6966 2065 6c65 6d65 6e74 7320 3d3d 2022  if elements == "
-00009b60: 616c 6c22 3a0a 2020 2020 2020 2020 2020  all":.          
-00009b70: 2020 656c 656d 656e 7473 203d 2073 656c    elements = sel
-00009b80: 662e 706f 6c79 676f 6e73 202b 2073 656c  f.polygons + sel
-00009b90: 662e 7265 6665 7265 6e63 6573 0a20 2020  f.references.   
-00009ba0: 2020 2020 205f 6469 7374 7269 6275 7465       _distribute
-00009bb0: 280a 2020 2020 2020 2020 2020 2020 656c  (.            el
-00009bc0: 656d 656e 7473 3d65 6c65 6d65 6e74 732c  ements=elements,
-00009bd0: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
-00009be0: 6563 7469 6f6e 3d64 6972 6563 7469 6f6e  ection=direction
-00009bf0: 2c0a 2020 2020 2020 2020 2020 2020 7370  ,.            sp
-00009c00: 6163 696e 673d 7370 6163 696e 672c 0a20  acing=spacing,. 
-00009c10: 2020 2020 2020 2020 2020 2073 6570 6172             separ
-00009c20: 6174 696f 6e3d 7365 7061 7261 7469 6f6e  ation=separation
-00009c30: 2c0a 2020 2020 2020 2020 2020 2020 6564  ,.            ed
-00009c40: 6765 3d65 6467 652c 0a20 2020 2020 2020  ge=edge,.       
-00009c50: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-00009c60: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
-00009c70: 616c 6967 6e28 7365 6c66 2c20 656c 656d  align(self, elem
-00009c80: 656e 7473 3d22 616c 6c22 2c20 616c 6967  ents="all", alig
-00009c90: 6e6d 656e 743d 2279 6d61 7822 293a 0a20  nment="ymax"):. 
-00009ca0: 2020 2020 2020 2022 2222 416c 6967 6e20         """Align 
-00009cb0: 656c 656d 656e 7473 2069 6e20 7468 6520  elements in the 
-00009cc0: 436f 6d70 6f6e 656e 742e 0a0a 2020 2020  Component...    
-00009cd0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00009ce0: 2020 2020 2020 656c 656d 656e 7473 203a        elements :
-00009cf0: 2061 7272 6179 2d6c 696b 6520 6f66 206f   array-like of o
-00009d00: 626a 6563 7473 2c20 6f72 2027 616c 6c27  bjects, or 'all'
-00009d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009d20: 2045 6c65 6d65 6e74 7320 696e 2074 6865   Elements in the
-00009d30: 2043 6f6d 706f 6e65 6e74 2074 6f20 616c   Component to al
-00009d40: 6967 6e2e 0a20 2020 2020 2020 2020 2020  ign..           
-00009d50: 2061 6c69 676e 6d65 6e74 203a 207b 2778   alignment : {'x
-00009d60: 272c 2027 7927 2c20 2778 6d69 6e27 2c20  ', 'y', 'xmin', 
-00009d70: 2778 6d61 7827 2c20 2779 6d69 6e27 2c20  'xmax', 'ymin', 
-00009d80: 2779 6d61 7827 7d0a 2020 2020 2020 2020  'ymax'}.        
-00009d90: 2020 2020 2020 2020 5768 6963 6820 6564          Which ed
-00009da0: 6765 2074 6f20 616c 6967 6e20 616c 6f6e  ge to align alon
-00009db0: 6720 2865 2e67 2e20 2779 6d61 7827 2077  g (e.g. 'ymax' w
-00009dc0: 696c 6c20 6d6f 7665 2074 6865 2065 6c65  ill move the ele
-00009dd0: 6d65 6e74 7320 7375 6368 0a20 2020 2020  ments such.     
-00009de0: 2020 2020 2020 2020 2020 2074 6861 7420             that 
-00009df0: 616c 6c20 6f66 2074 6865 6972 2074 6f70  all of their top
-00009e00: 6d6f 7374 2070 6f69 6e74 7320 6172 6520  most points are 
-00009e10: 616c 6967 6e65 6429 2e0a 2020 2020 2020  aligned)..      
-00009e20: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00009e30: 2065 6c65 6d65 6e74 7320 3d3d 2022 616c   elements == "al
-00009e40: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
-00009e50: 656c 656d 656e 7473 203d 2073 656c 662e  elements = self.
-00009e60: 706f 6c79 676f 6e73 202b 2073 656c 662e  polygons + self.
-00009e70: 7265 6665 7265 6e63 6573 0a20 2020 2020  references.     
-00009e80: 2020 205f 616c 6967 6e28 656c 656d 656e     _align(elemen
-00009e90: 7473 2c20 616c 6967 6e6d 656e 743d 616c  ts, alignment=al
-00009ea0: 6967 6e6d 656e 7429 0a20 2020 2020 2020  ignment).       
-00009eb0: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
-00009ec0: 2020 6465 6620 666c 6174 7465 6e28 7365    def flatten(se
-00009ed0: 6c66 2c20 7369 6e67 6c65 5f6c 6179 6572  lf, single_layer
-00009ee0: 3a20 4f70 7469 6f6e 616c 5b4c 6179 6572  : Optional[Layer
-00009ef0: 5370 6563 5d20 3d20 4e6f 6e65 293a 0a20  Spec] = None):. 
-00009f00: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00009f10: 7320 6120 666c 6174 7465 6e65 6420 636f  s a flattened co
-00009f20: 7079 206f 6620 7468 6520 636f 6d70 6f6e  py of the compon
-00009f30: 656e 742e 0a0a 2020 2020 2020 2020 466c  ent...        Fl
-00009f40: 6174 7465 6e73 2074 6865 2068 6965 7261  attens the hiera
-00009f50: 7263 6879 206f 6620 7468 6520 436f 6d70  rchy of the Comp
-00009f60: 6f6e 656e 7420 7375 6368 2074 6861 7420  onent such that 
-00009f70: 7468 6572 6520 6172 6520 6e6f 206c 6f6e  there are no lon
-00009f80: 6765 720a 2020 2020 2020 2020 616e 7920  ger.        any 
-00009f90: 7265 6665 7265 6e63 6573 2074 6f20 6f74  references to ot
-00009fa0: 6865 7220 436f 6d70 6f6e 656e 7473 2e20  her Components. 
-00009fb0: 416c 6c20 706f 6c79 676f 6e73 2061 6e64  All polygons and
-00009fc0: 206c 6162 656c 7320 6672 6f6d 0a20 2020   labels from.   
-00009fd0: 2020 2020 2075 6e64 6572 6c79 696e 6720       underlying 
-00009fe0: 7265 6665 7265 6e63 6573 2061 7265 2063  references are c
-00009ff0: 6f70 6965 6420 616e 6420 706c 6163 6564  opied and placed
-0000a000: 2069 6e20 7468 6520 746f 702d 6c65 7665   in the top-leve
-0000a010: 6c20 436f 6d70 6f6e 656e 742e 0a20 2020  l Component..   
-0000a020: 2020 2020 2049 6620 7369 6e67 6c65 5f6c       If single_l
-0000a030: 6179 6572 2069 7320 7370 6563 6966 6965  ayer is specifie
-0000a040: 642c 2061 6c6c 2070 6f6c 7967 6f6e 7320  d, all polygons 
-0000a050: 6172 6520 6d6f 7665 6420 746f 2074 6861  are moved to tha
-0000a060: 7420 6c61 7965 722e 0a0a 2020 2020 2020  t layer...      
-0000a070: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000a080: 2020 2020 7369 6e67 6c65 5f6c 6179 6572      single_layer
-0000a090: 3a20 6d6f 7665 2061 6c6c 2070 6f6c 7967  : move all polyg
-0000a0a0: 6f6e 7320 6172 6520 6d6f 7665 6420 746f  ons are moved to
-0000a0b0: 2074 6865 2073 7065 6369 6669 6564 2028   the specified (
-0000a0c0: 6f70 7469 6f6e 616c 292e 0a20 2020 2020  optional)..     
-0000a0d0: 2020 2022 2222 0a20 2020 2020 2020 2063     """.        c
-0000a0e0: 6f6d 706f 6e65 6e74 5f66 6c61 7420 3d20  omponent_flat = 
-0000a0f0: 436f 6d70 6f6e 656e 7428 290a 0a20 2020  Component()..   
-0000a100: 2020 2020 205f 6365 6c6c 203d 2073 656c       _cell = sel
-0000a110: 662e 5f63 656c 6c2e 636f 7079 286e 616d  f._cell.copy(nam
-0000a120: 653d 636f 6d70 6f6e 656e 745f 666c 6174  e=component_flat
-0000a130: 2e6e 616d 6529 0a20 2020 2020 2020 205f  .name).        _
-0000a140: 6365 6c6c 203d 205f 6365 6c6c 2e66 6c61  cell = _cell.fla
-0000a150: 7474 656e 2829 0a20 2020 2020 2020 2063  tten().        c
-0000a160: 6f6d 706f 6e65 6e74 5f66 6c61 742e 5f63  omponent_flat._c
-0000a170: 656c 6c20 3d20 5f63 656c 6c0a 2020 2020  ell = _cell.    
-0000a180: 2020 2020 6966 2073 696e 676c 655f 6c61      if single_la
-0000a190: 7965 7220 6973 206e 6f74 204e 6f6e 653a  yer is not None:
-0000a1a0: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-0000a1b0: 6d20 6764 7366 6163 746f 7279 2069 6d70  m gdsfactory imp
-0000a1c0: 6f72 7420 6765 745f 6c61 7965 720a 0a20  ort get_layer.. 
-0000a1d0: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-0000a1e0: 2c20 6461 7461 7479 7065 203d 2067 6574  , datatype = get
-0000a1f0: 5f6c 6179 6572 2873 696e 676c 655f 6c61  _layer(single_la
-0000a200: 7965 7229 0a20 2020 2020 2020 2020 2020  yer).           
-0000a210: 2066 6f72 2070 6f6c 7967 6f6e 2069 6e20   for polygon in 
-0000a220: 5f63 656c 6c2e 706f 6c79 676f 6e73 3a0a  _cell.polygons:.
-0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 706f 6c79 676f 6e2e 6c61 7965 7220 3d20  polygon.layer = 
-0000a250: 6c61 7965 720a 2020 2020 2020 2020 2020  layer.          
-0000a260: 2020 2020 2020 706f 6c79 676f 6e2e 6461        polygon.da
-0000a270: 7461 7479 7065 203d 2064 6174 6174 7970  tatype = datatyp
-0000a280: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
-0000a290: 7220 7061 7468 2069 6e20 5f63 656c 6c2e  r path in _cell.
-0000a2a0: 7061 7468 733a 0a20 2020 2020 2020 2020  paths:.         
-0000a2b0: 2020 2020 2020 2070 6174 682e 7365 745f         path.set_
-0000a2c0: 6c61 7965 7273 286c 6179 6572 290a 2020  layers(layer).  
-0000a2d0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000a2e0: 7468 2e73 6574 5f64 6174 6174 7970 6573  th.set_datatypes
-0000a2f0: 2864 6174 6174 7970 6529 0a0a 2020 2020  (datatype)..    
-0000a300: 2020 2020 636f 6d70 6f6e 656e 745f 666c      component_fl
-0000a310: 6174 2e69 6e66 6f20 3d20 7365 6c66 2e69  at.info = self.i
-0000a320: 6e66 6f2e 636f 7079 2829 0a20 2020 2020  nfo.copy().     
-0000a330: 2020 2063 6f6d 706f 6e65 6e74 5f66 6c61     component_fla
-0000a340: 742e 6164 645f 706f 7274 7328 7365 6c66  t.add_ports(self
-0000a350: 2e70 6f72 7473 290a 2020 2020 2020 2020  .ports).        
-0000a360: 7265 7475 726e 2063 6f6d 706f 6e65 6e74  return component
-0000a370: 5f66 6c61 740a 0a20 2020 2064 6566 2066  _flat..    def f
-0000a380: 6c61 7474 656e 5f72 6566 6572 656e 6365  latten_reference
-0000a390: 2873 656c 662c 2072 6566 3a20 436f 6d70  (self, ref: Comp
-0000a3a0: 6f6e 656e 7452 6566 6572 656e 6365 293a  onentReference):
-0000a3b0: 0a20 2020 2020 2020 2022 2222 4672 6f6d  .        """From
-0000a3c0: 2065 7869 7374 696e 6720 6365 6c6c 2072   existing cell r
-0000a3d0: 6570 6c61 6365 7320 7265 6665 7265 6e63  eplaces referenc
-0000a3e0: 6520 7769 7468 2061 2066 6c61 7474 656e  e with a flatten
-0000a3f0: 2072 6566 6572 656e 6365 205c 0a20 2020   reference \.   
-0000a400: 2020 2020 2077 6869 6368 2068 6173 2074       which has t
-0000a410: 6865 2074 7261 6e73 666f 726d 6174 696f  he transformatio
-0000a420: 6e73 2061 6c72 6561 6479 2061 7070 6c69  ns already appli
-0000a430: 6564 2e0a 0a20 2020 2020 2020 2054 7261  ed...        Tra
-0000a440: 6e73 666f 726d 6564 2072 6566 6572 656e  nsformed referen
-0000a450: 6365 206b 6565 7073 2074 6865 206f 7269  ce keeps the ori
-0000a460: 6769 6e61 6c20 6e61 6d65 2e0a 0a20 2020  ginal name...   
-0000a470: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000a480: 2020 2020 2020 2072 6566 3a20 7468 6520         ref: the 
-0000a490: 7265 6665 7265 6e63 6520 746f 2066 6c61  reference to fla
-0000a4a0: 7474 656e 2069 6e74 6f20 6120 6e65 7720  tten into a new 
-0000a4b0: 6365 6c6c 2e0a 0a20 2020 2020 2020 2022  cell...        "
-0000a4c0: 2222 0a20 2020 2020 2020 2066 726f 6d20  "".        from 
-0000a4d0: 6764 7366 6163 746f 7279 2e66 756e 6374  gdsfactory.funct
-0000a4e0: 696f 6e73 2069 6d70 6f72 7420 7472 616e  ions import tran
-0000a4f0: 7366 6f72 6d65 640a 0a20 2020 2020 2020  sformed..       
-0000a500: 2073 656c 662e 7265 6d6f 7665 2872 6566   self.remove(ref
-0000a510: 290a 2020 2020 2020 2020 6e65 775f 636f  ).        new_co
-0000a520: 6d70 6f6e 656e 7420 3d20 7472 616e 7366  mponent = transf
-0000a530: 6f72 6d65 6428 7265 662c 2064 6563 6f72  ormed(ref, decor
-0000a540: 6174 6f72 3d4e 6f6e 6529 0a20 2020 2020  ator=None).     
-0000a550: 2020 2073 656c 662e 6164 645f 7265 6628     self.add_ref(
-0000a560: 6e65 775f 636f 6d70 6f6e 656e 742c 2061  new_component, a
-0000a570: 6c69 6173 3d72 6566 2e6e 616d 6529 0a0a  lias=ref.name)..
-0000a580: 2020 2020 6465 6620 6164 645f 7265 6628      def add_ref(
-0000a590: 0a20 2020 2020 2020 2073 656c 662c 2063  .        self, c
-0000a5a0: 6f6d 706f 6e65 6e74 3a20 436f 6d70 6f6e  omponent: Compon
-0000a5b0: 656e 742c 2061 6c69 6173 3a20 4f70 7469  ent, alias: Opti
-0000a5c0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0000a5d0: 2c20 2a2a 6b77 6172 6773 0a20 2020 2029  , **kwargs.    )
-0000a5e0: 202d 3e20 436f 6d70 6f6e 656e 7452 6566   -> ComponentRef
-0000a5f0: 6572 656e 6365 3a0a 2020 2020 2020 2020  erence:.        
-0000a600: 2222 2241 6464 2043 6f6d 706f 6e65 6e74  """Add Component
-0000a610: 5265 6665 7265 6e63 6520 746f 2074 6865  Reference to the
-0000a620: 2063 7572 7265 6e74 2043 6f6d 706f 6e65   current Compone
-0000a630: 6e74 2e0a 0a20 2020 2020 2020 2041 7267  nt...        Arg
-0000a640: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-0000a650: 6f6d 706f 6e65 6e74 3a20 436f 6d70 6f6e  omponent: Compon
-0000a660: 656e 742e 0a20 2020 2020 2020 2020 2020  ent..           
-0000a670: 2061 6c69 6173 3a20 6e61 6d65 645f 7265   alias: named_re
-0000a680: 6665 7265 6e63 6573 2e0a 0a20 2020 2020  ferences...     
-0000a690: 2020 204b 6579 776f 7264 2041 7267 733a     Keyword Args:
-0000a6a0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-0000a6b0: 756d 6e73 3a20 4e75 6d62 6572 206f 6620  umns: Number of 
-0000a6c0: 636f 6c75 6d6e 7320 696e 2074 6865 2061  columns in the a
-0000a6d0: 7272 6179 2e0a 2020 2020 2020 2020 2020  rray..          
-0000a6e0: 2020 726f 7773 3a20 4e75 6d62 6572 206f    rows: Number o
-0000a6f0: 6620 726f 7773 2069 6e20 7468 6520 6172  f rows in the ar
-0000a700: 7261 792e 0a20 2020 2020 2020 2020 2020  ray..           
-0000a710: 2073 7061 6369 6e67 3a20 4469 7374 616e   spacing: Distan
-0000a720: 6365 7320 6265 7477 6565 6e20 6164 6a61  ces between adja
-0000a730: 6365 6e74 2063 6f6c 756d 6e73 2061 6e64  cent columns and
-0000a740: 2061 646a 6163 656e 7420 726f 7773 2e0a   adjacent rows..
-0000a750: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-0000a760: 696e 3a20 6172 7261 792d 6c69 6b65 5b32  in: array-like[2
-0000a770: 5d20 6f66 2069 6e74 206f 7220 666c 6f61  ] of int or floa
-0000a780: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-0000a790: 2020 506f 7369 7469 6f6e 2077 6865 7265    Position where
-0000a7a0: 2074 6865 2063 656c 6c20 6973 2069 6e73   the cell is ins
-0000a7b0: 6572 7465 642e 0a20 2020 2020 2020 2020  erted..         
-0000a7c0: 2020 2072 6f74 6174 696f 6e20 3a20 696e     rotation : in
-0000a7d0: 7420 6f72 2066 6c6f 6174 0a20 2020 2020  t or float.     
-0000a7e0: 2020 2020 2020 2020 2020 2041 6e67 6c65             Angle
-0000a7f0: 206f 6620 726f 7461 7469 6f6e 206f 6620   of rotation of 
-0000a800: 7468 6520 7265 6665 7265 6e63 6520 2869  the reference (i
-0000a810: 6e20 6064 6567 7265 6573 6029 2e0a 2020  n `degrees`)..  
-0000a820: 2020 2020 2020 2020 2020 6d61 676e 6966            magnif
-0000a830: 6963 6174 696f 6e20 3a20 696e 7420 6f72  ication : int or
-0000a840: 2066 6c6f 6174 0a20 2020 2020 2020 2020   float.         
-0000a850: 2020 2020 2020 204d 6167 6e69 6669 6361         Magnifica
-0000a860: 7469 6f6e 2066 6163 746f 7220 666f 7220  tion factor for 
-0000a870: 7468 6520 7265 6665 7265 6e63 652e 0a20  the reference.. 
-0000a880: 2020 2020 2020 2020 2020 2078 5f72 6566             x_ref
-0000a890: 6c65 6374 696f 6e20 3a20 626f 6f6c 0a20  lection : bool. 
-0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-0000a8b0: 6620 5472 7565 2c20 7468 6520 7265 6665  f True, the refe
-0000a8c0: 7265 6e63 6520 6973 2072 6566 6c65 6374  rence is reflect
-0000a8d0: 6564 2070 6172 616c 6c65 6c20 746f 2074  ed parallel to t
-0000a8e0: 6865 2078 2064 6972 6563 7469 6f6e 0a20  he x direction. 
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000a900: 6566 6f72 6520 6265 696e 6720 726f 7461  efore being rota
-0000a910: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
-0000a920: 206e 616d 6520 3a20 7374 7220 286f 7074   name : str (opt
-0000a930: 696f 6e61 6c29 0a20 2020 2020 2020 2020  ional).         
-0000a940: 2020 2020 2020 2041 206e 616d 6520 666f         A name fo
-0000a950: 7220 7468 6520 7265 6665 7265 6e63 6520  r the reference 
-0000a960: 2869 6620 7072 6f76 6964 6564 292e 0a0a  (if provided)...
-0000a970: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000a980: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0000a990: 7461 6e63 6528 636f 6d70 6f6e 656e 742c  tance(component,
-0000a9a0: 2043 6f6d 706f 6e65 6e74 293a 0a20 2020   Component):.   
-0000a9b0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-0000a9c0: 7970 6545 7272 6f72 2866 2274 7970 6520  ypeError(f"type 
-0000a9d0: 3d20 7b74 7970 6528 436f 6d70 6f6e 656e  = {type(Componen
-0000a9e0: 7429 7d20 6e65 6564 7320 746f 2062 6520  t)} needs to be 
-0000a9f0: 6120 436f 6d70 6f6e 656e 742e 2229 0a20  a Component."). 
-0000aa00: 2020 2020 2020 2072 6566 203d 2043 6f6d         ref = Com
-0000aa10: 706f 6e65 6e74 5265 6665 7265 6e63 6528  ponentReference(
-0000aa20: 636f 6d70 6f6e 656e 742c 202a 2a6b 7761  component, **kwa
-0000aa30: 7267 7329 0a20 2020 2020 2020 2073 656c  rgs).        sel
-0000aa40: 662e 5f61 6464 2872 6566 290a 2020 2020  f._add(ref).    
-0000aa50: 2020 2020 7365 6c66 2e5f 7265 6769 7374      self._regist
-0000aa60: 6572 5f72 6566 6572 656e 6365 2872 6566  er_reference(ref
-0000aa70: 6572 656e 6365 3d72 6566 2c20 616c 6961  erence=ref, alia
-0000aa80: 733d 616c 6961 7329 0a20 2020 2020 2020  s=alias).       
-0000aa90: 2072 6574 7572 6e20 7265 660a 0a20 2020   return ref..   
-0000aaa0: 2064 6566 205f 7265 6769 7374 6572 5f72   def _register_r
-0000aab0: 6566 6572 656e 6365 280a 2020 2020 2020  eference(.      
-0000aac0: 2020 7365 6c66 2c20 7265 6665 7265 6e63    self, referenc
-0000aad0: 653a 2043 6f6d 706f 6e65 6e74 5265 6665  e: ComponentRefe
-0000aae0: 7265 6e63 652c 2061 6c69 6173 3a20 4f70  rence, alias: Op
-0000aaf0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0000ab00: 6e65 0a20 2020 2029 202d 3e20 4e6f 6e65  ne.    ) -> None
-0000ab10: 3a0a 2020 2020 2020 2020 636f 6d70 6f6e  :.        compon
-0000ab20: 656e 7420 3d20 7265 6665 7265 6e63 652e  ent = reference.
-0000ab30: 7061 7265 6e74 0a20 2020 2020 2020 2072  parent.        r
-0000ab40: 6566 6572 656e 6365 2e6f 776e 6572 203d  eference.owner =
-0000ab50: 2073 656c 660a 0a20 2020 2020 2020 2069   self..        i
-0000ab60: 6620 616c 6961 7320 6973 204e 6f6e 653a  f alias is None:
-0000ab70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000ab80: 7265 6665 7265 6e63 652e 6e61 6d65 2069  reference.name i
-0000ab90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000aba0: 2020 2020 2020 2020 2020 2020 616c 6961              alia
-0000abb0: 7320 3d20 7265 6665 7265 6e63 652e 6e61  s = reference.na
-0000abc0: 6d65 0a20 2020 2020 2020 2020 2020 2065  me.            e
-0000abd0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000abe0: 2020 2020 2070 7265 6669 7820 3d20 280a       prefix = (.
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 2020 2020 636f 6d70 6f6e 656e 742e 7365      component.se
-0000ac10: 7474 696e 6773 2e66 756e 6374 696f 6e5f  ttings.function_
-0000ac20: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
-0000ac30: 2020 2020 2020 2020 2069 6620 6861 7361           if hasa
-0000ac40: 7474 7228 636f 6d70 6f6e 656e 742c 2022  ttr(component, "
-0000ac50: 7365 7474 696e 6773 2229 0a20 2020 2020  settings").     
-0000ac60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000ac70: 6e64 2068 6173 6174 7472 2863 6f6d 706f  nd hasattr(compo
-0000ac80: 6e65 6e74 2e73 6574 7469 6e67 732c 2022  nent.settings, "
-0000ac90: 6675 6e63 7469 6f6e 5f6e 616d 6522 290a  function_name").
-0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acb0: 2020 2020 656c 7365 2063 6f6d 706f 6e65      else compone
-0000acc0: 6e74 2e6e 616d 650a 2020 2020 2020 2020  nt.name.        
-0000acd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000ace0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000acf0: 7265 6665 7265 6e63 655f 6e61 6d65 735f  reference_names_
-0000ad00: 636f 756e 7465 722e 7570 6461 7465 287b  counter.update({
-0000ad10: 7072 6566 6978 3a20 317d 290a 2020 2020  prefix: 1}).    
-0000ad20: 2020 2020 2020 2020 2020 2020 616c 6961              alia
-0000ad30: 7320 3d20 6622 7b70 7265 6669 787d 5f7b  s = f"{prefix}_{
-0000ad40: 7365 6c66 2e5f 7265 6665 7265 6e63 655f  self._reference_
-0000ad50: 6e61 6d65 735f 636f 756e 7465 725b 7072  names_counter[pr
-0000ad60: 6566 6978 5d7d 220a 0a20 2020 2020 2020  efix]}"..       
-0000ad70: 2020 2020 2020 2020 2077 6869 6c65 2061           while a
-0000ad80: 6c69 6173 2069 6e20 7365 6c66 2e5f 6e61  lias in self._na
-0000ad90: 6d65 645f 7265 6665 7265 6e63 6573 3a0a  med_references:.
-0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adb0: 2020 2020 7365 6c66 2e5f 7265 6665 7265      self._refere
-0000adc0: 6e63 655f 6e61 6d65 735f 636f 756e 7465  nce_names_counte
-0000add0: 722e 7570 6461 7465 287b 7072 6566 6978  r.update({prefix
-0000ade0: 3a20 317d 290a 2020 2020 2020 2020 2020  : 1}).          
-0000adf0: 2020 2020 2020 2020 2020 616c 6961 7320            alias 
-0000ae00: 3d20 6622 7b70 7265 6669 787d 5f7b 7365  = f"{prefix}_{se
-0000ae10: 6c66 2e5f 7265 6665 7265 6e63 655f 6e61  lf._reference_na
-0000ae20: 6d65 735f 636f 756e 7465 725b 7072 6566  mes_counter[pref
-0000ae30: 6978 5d7d 220a 0a20 2020 2020 2020 2072  ix]}"..        r
-0000ae40: 6566 6572 656e 6365 2e6e 616d 6520 3d20  eference.name = 
-0000ae50: 616c 6961 730a 2020 2020 2020 2020 7365  alias.        se
-0000ae60: 6c66 2e5f 6e61 6d65 645f 7265 6665 7265  lf._named_refere
-0000ae70: 6e63 6573 5b61 6c69 6173 5d20 3d20 7265  nces[alias] = re
-0000ae80: 6665 7265 6e63 650a 0a20 2020 2040 7072  ference..    @pr
-0000ae90: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
-0000aea0: 6179 6572 7328 7365 6c66 2920 2d3e 2053  ayers(self) -> S
-0000aeb0: 6574 5b54 7570 6c65 5b69 6e74 2c20 696e  et[Tuple[int, in
-0000aec0: 745d 5d3a 0a20 2020 2020 2020 2022 2222  t]]:.        """
-0000aed0: 5265 7475 726e 7320 6120 7365 7420 6f66  Returns a set of
-0000aee0: 2074 6865 204c 6179 6572 7320 696e 2074   the Layers in t
-0000aef0: 6865 2043 6f6d 706f 6e65 6e74 2e22 2222  he Component."""
-0000af00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000af10: 7365 6c66 2e67 6574 5f6c 6179 6572 7328  self.get_layers(
-0000af20: 290a 0a20 2020 2064 6566 2067 6574 5f6c  )..    def get_l
-0000af30: 6179 6572 7328 7365 6c66 2920 2d3e 2053  ayers(self) -> S
-0000af40: 6574 5b54 7570 6c65 5b69 6e74 2c20 696e  et[Tuple[int, in
-0000af50: 745d 5d3a 0a20 2020 2020 2020 2022 2222  t]]:.        """
-0000af60: 5265 7475 726e 2061 2073 6574 206f 6620  Return a set of 
-0000af70: 286c 6179 6572 2c20 6461 7461 7479 7065  (layer, datatype
-0000af80: 292e 0a0a 2020 2020 2020 2020 2e2e 2063  )...        .. c
-0000af90: 6f64 6520 3a3a 0a0a 2020 2020 2020 2020  ode ::..        
-0000afa0: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
-0000afb0: 6374 6f72 7920 6173 2067 660a 2020 2020  ctory as gf.    
-0000afc0: 2020 2020 2020 2020 6766 2e63 6f6d 706f          gf.compo
-0000afd0: 6e65 6e74 732e 7374 7261 6967 6874 2829  nents.straight()
-0000afe0: 2e67 6574 5f6c 6179 6572 7328 2920 3d3d  .get_layers() ==
-0000aff0: 207b 2831 2c20 3029 2c20 2831 3131 2c20   {(1, 0), (111, 
-0000b000: 3029 7d0a 2020 2020 2020 2020 2222 220a  0)}.        """.
-0000b010: 2020 2020 2020 2020 706f 6c79 676f 6e73          polygons
-0000b020: 203d 2073 656c 662e 5f63 656c 6c2e 6765   = self._cell.ge
-0000b030: 745f 706f 6c79 676f 6e73 2864 6570 7468  t_polygons(depth
-0000b040: 3d4e 6f6e 6529 0a20 2020 2020 2020 2072  =None).        r
-0000b050: 6574 7572 6e20 7b28 706f 6c79 676f 6e2e  eturn {(polygon.
-0000b060: 6c61 7965 722c 2070 6f6c 7967 6f6e 2e64  layer, polygon.d
-0000b070: 6174 6174 7970 6529 2066 6f72 2070 6f6c  atatype) for pol
-0000b080: 7967 6f6e 2069 6e20 706f 6c79 676f 6e73  ygon in polygons
-0000b090: 7d0a 0a20 2020 2064 6566 2067 6574 5f6c  }..    def get_l
-0000b0a0: 6179 6572 5f6e 616d 6573 2873 656c 6629  ayer_names(self)
-0000b0b0: 202d 3e20 4c69 7374 5b54 7570 6c65 5b69   -> List[Tuple[i
-0000b0c0: 6e74 2c20 696e 745d 5d3a 0a20 2020 2020  nt, int]]:.     
-0000b0d0: 2020 2022 2222 5265 7475 726e 206c 6179     """Return lay
-0000b0e0: 6572 206e 616d 6573 2075 7365 6420 696e  er names used in
-0000b0f0: 2074 6865 2064 6573 6967 6e2e 0a0a 2020   the design...  
-0000b100: 2020 2020 2020 2e2e 2063 6f64 6520 3a3a        .. code ::
-0000b110: 0a0a 2020 2020 2020 2020 2020 2020 696d  ..            im
-0000b120: 706f 7274 2067 6473 6661 6374 6f72 7920  port gdsfactory 
-0000b130: 6173 2067 660a 2020 2020 2020 2020 2020  as gf.          
-0000b140: 2020 6766 2e63 6f6d 706f 6e65 6e74 732e    gf.components.
-0000b150: 7374 7261 6967 6874 2829 2e67 6574 5f6e  straight().get_n
-0000b160: 616d 6573 2829 203d 3d20 5b27 5747 275d  ames() == ['WG']
-0000b170: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000b180: 2020 2020 2069 6d70 6f72 7420 6764 7366       import gdsf
-0000b190: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
-0000b1a0: 2020 2020 2020 5044 4b20 3d20 6766 2e67        PDK = gf.g
-0000b1b0: 6574 5f61 6374 6976 655f 7064 6b28 290a  et_active_pdk().
-0000b1c0: 2020 2020 2020 2020 4c41 5945 5253 203d          LAYERS =
-0000b1d0: 2050 444b 2e6c 6179 6572 730a 2020 2020   PDK.layers.    
-0000b1e0: 2020 2020 6e61 6d65 5f74 6f5f 6c61 7965      name_to_laye
-0000b1f0: 7220 3d20 6469 6374 284c 4159 4552 5329  r = dict(LAYERS)
-0000b200: 0a20 2020 2020 2020 206c 6179 6572 5f74  .        layer_t
-0000b210: 6f5f 6e61 6d65 203d 207b 763a 206b 2066  o_name = {v: k f
-0000b220: 6f72 206b 2c20 7620 696e 206e 616d 655f  or k, v in name_
-0000b230: 746f 5f6c 6179 6572 2e69 7465 6d73 2829  to_layer.items()
-0000b240: 7d0a 2020 2020 2020 2020 6c61 7965 725f  }.        layer_
-0000b250: 6e61 6d65 7320 3d20 5b5d 0a0a 2020 2020  names = []..    
-0000b260: 2020 2020 666f 7220 6c61 7965 7220 696e      for layer in
-0000b270: 2073 656c 662e 6c61 7965 7273 3a0a 2020   self.layers:.  
-0000b280: 2020 2020 2020 2020 2020 6966 206c 6179            if lay
-0000b290: 6572 206e 6f74 2069 6e20 6c61 7965 725f  er not in layer_
-0000b2a0: 746f 5f6e 616d 653a 0a20 2020 2020 2020  to_name:.       
-0000b2b0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
-0000b2c0: 732e 7761 726e 2866 227b 6c61 7965 727d  s.warn(f"{layer}
-0000b2d0: 206e 6f74 2069 6e20 4c61 7965 724d 6170   not in LayerMap
-0000b2e0: 2e2e 2229 0a20 2020 2020 2020 2020 2020  ..").           
-0000b2f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000b300: 2020 2020 2020 206c 6179 6572 5f6e 616d         layer_nam
-0000b310: 6573 2e61 7070 656e 6428 6c61 7965 725f  es.append(layer_
-0000b320: 746f 5f6e 616d 655b 6c61 7965 725d 290a  to_name[layer]).
-0000b330: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-0000b340: 6179 6572 5f6e 616d 6573 0a0a 2020 2020  ayer_names..    
-0000b350: 6465 6620 5f69 7079 7468 6f6e 5f64 6973  def _ipython_dis
-0000b360: 706c 6179 5f28 7365 6c66 2920 2d3e 204e  play_(self) -> N
-0000b370: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000b380: 5368 6f77 2067 656f 6d65 7472 7920 696e  Show geometry in
-0000b390: 204b 4c61 796f 7574 2061 6e64 2069 6e20   KLayout and in 
-0000b3a0: 6d61 7470 6c6f 746c 6962 2066 6f72 204a  matplotlib for J
-0000b3b0: 7570 7974 6572 204e 6f74 6562 6f6f 6b73  upyter Notebooks
-0000b3c0: 2e22 2222 0a20 2020 2020 2020 2073 656c  .""".        sel
-0000b3d0: 662e 7368 6f77 2873 686f 775f 706f 7274  f.show(show_port
-0000b3e0: 733d 5472 7565 2920 2023 2073 686f 7720  s=True)  # show 
-0000b3f0: 696e 206b 6c61 796f 7574 0a20 2020 2020  in klayout.     
-0000b400: 2020 2073 656c 662e 706c 6f74 5f6b 6c61     self.plot_kla
-0000b410: 796f 7574 2829 0a20 2020 2020 2020 2070  yout().        p
-0000b420: 7269 6e74 2873 656c 6629 0a0a 2020 2020  rint(self)..    
-0000b430: 6465 6620 6164 645f 7069 6e73 5f74 7269  def add_pins_tri
-0000b440: 616e 676c 6528 0a20 2020 2020 2020 2073  angle(.        s
-0000b450: 656c 662c 0a20 2020 2020 2020 2070 6f72  elf,.        por
-0000b460: 745f 6d61 726b 6572 5f6c 6179 6572 3a20  t_marker_layer: 
-0000b470: 4c61 7965 7220 3d20 2831 2c20 3130 292c  Layer = (1, 10),
-0000b480: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-0000b490: 2222 2252 6574 7572 6e73 2063 6f6d 706f  """Returns compo
-0000b4a0: 6e65 6e74 2077 6974 6820 7472 6961 6e67  nent with triang
-0000b4b0: 756c 6172 2070 696e 732e 2222 220a 2020  ular pins.""".  
-0000b4c0: 2020 2020 2020 6672 6f6d 2067 6473 6661        from gdsfa
-0000b4d0: 6374 6f72 792e 6164 645f 7069 6e73 2069  ctory.add_pins i
-0000b4e0: 6d70 6f72 7420 6164 645f 7069 6e73 5f74  mport add_pins_t
-0000b4f0: 7269 616e 676c 650a 0a20 2020 2020 2020  riangle..       
-0000b500: 2063 6f6d 706f 6e65 6e74 203d 2073 656c   component = sel
-0000b510: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-0000b520: 2063 6f6d 706f 6e65 6e74 2e6e 616d 6520   component.name 
-0000b530: 3d20 7365 6c66 2e6e 616d 650a 2020 2020  = self.name.    
-0000b540: 2020 2020 6164 645f 7069 6e73 5f74 7269      add_pins_tri
-0000b550: 616e 676c 6528 636f 6d70 6f6e 656e 743d  angle(component=
-0000b560: 636f 6d70 6f6e 656e 742c 206c 6179 6572  component, layer
-0000b570: 3d70 6f72 745f 6d61 726b 6572 5f6c 6179  =port_marker_lay
-0000b580: 6572 290a 2020 2020 2020 2020 7265 7475  er).        retu
-0000b590: 726e 2063 6f6d 706f 6e65 6e74 0a0a 2020  rn component..  
-0000b5a0: 2020 6465 6620 706c 6f74 5f77 6964 6765    def plot_widge
-0000b5b0: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
-0000b5c0: 0a20 2020 2020 2020 2073 686f 775f 706f  .        show_po
-0000b5d0: 7274 733a 2062 6f6f 6c20 3d20 5472 7565  rts: bool = True
-0000b5e0: 2c0a 2020 2020 2020 2020 706f 7274 5f6d  ,.        port_m
-0000b5f0: 6172 6b65 725f 6c61 7965 723a 204c 6179  arker_layer: Lay
-0000b600: 6572 203d 2028 312c 2031 3029 2c0a 2020  er = (1, 10),.  
-0000b610: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-0000b620: 5265 7475 726e 7320 6970 7974 686f 6e20  Returns ipython 
-0000b630: 7769 6467 6574 2066 6f72 206b 6c61 796f  widget for klayo
-0000b640: 7574 2076 6973 7561 6c69 7a61 7469 6f6e  ut visualization
-0000b650: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0000b660: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
-0000b670: 775f 706f 7274 733a 2073 686f 7773 2063  w_ports: shows c
-0000b680: 6f6d 706f 6e65 6e74 2077 6974 6820 706f  omponent with po
-0000b690: 7274 206d 6172 6b65 7273 2061 6e64 206c  rt markers and l
-0000b6a0: 6162 656c 732e 0a20 2020 2020 2020 2020  abels..         
-0000b6b0: 2020 2070 6f72 745f 6d61 726b 6572 5f6c     port_marker_l
-0000b6c0: 6179 6572 3a20 666f 7220 7468 6520 706f  ayer: for the po
-0000b6d0: 7274 732e 0a20 2020 2020 2020 2022 2222  rts..        """
-0000b6e0: 0a20 2020 2020 2020 2066 726f 6d20 6764  .        from gd
-0000b6f0: 7366 6163 746f 7279 2e70 646b 2069 6d70  sfactory.pdk imp
-0000b700: 6f72 7420 6765 745f 6c61 7965 725f 7669  ort get_layer_vi
-0000b710: 6577 730a 2020 2020 2020 2020 6672 6f6d  ews.        from
-0000b720: 2067 6473 6661 6374 6f72 792e 7769 6467   gdsfactory.widg
-0000b730: 6574 732e 6c61 796f 7574 5f76 6965 7765  ets.layout_viewe
-0000b740: 7220 696d 706f 7274 204c 6179 6f75 7456  r import LayoutV
-0000b750: 6965 7765 720a 2020 2020 2020 2020 6672  iewer.        fr
-0000b760: 6f6d 2049 5079 7468 6f6e 2e64 6973 706c  om IPython.displ
-0000b770: 6179 2069 6d70 6f72 7420 6469 7370 6c61  ay import displa
-0000b780: 790a 0a20 2020 2020 2020 2063 6f6d 706f  y..        compo
-0000b790: 6e65 6e74 203d 2028 0a20 2020 2020 2020  nent = (.       
-0000b7a0: 2020 2020 2073 656c 662e 6164 645f 7069       self.add_pi
-0000b7b0: 6e73 5f74 7269 616e 676c 6528 706f 7274  ns_triangle(port
-0000b7c0: 5f6d 6172 6b65 725f 6c61 7965 723d 706f  _marker_layer=po
-0000b7d0: 7274 5f6d 6172 6b65 725f 6c61 7965 7229  rt_marker_layer)
-0000b7e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b7f0: 7368 6f77 5f70 6f72 7473 0a20 2020 2020  show_ports.     
-0000b800: 2020 2020 2020 2065 6c73 6520 7365 6c66         else self
-0000b810: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000b820: 2020 2020 6764 7370 6174 6820 3d20 636f      gdspath = co
-0000b830: 6d70 6f6e 656e 742e 7772 6974 655f 6764  mponent.write_gd
-0000b840: 7328 6c6f 6767 696e 673d 4661 6c73 6529  s(logging=False)
-0000b850: 0a20 2020 2020 2020 206c 7970 5f70 6174  .        lyp_pat
-0000b860: 6820 3d20 6764 7370 6174 682e 7769 7468  h = gdspath.with
-0000b870: 5f73 7566 6669 7828 222e 6c79 7022 290a  _suffix(".lyp").
-0000b880: 0a20 2020 2020 2020 206c 6179 6572 5f76  .        layer_v
-0000b890: 6965 7773 203d 2067 6574 5f6c 6179 6572  iews = get_layer
-0000b8a0: 5f76 6965 7773 2829 0a20 2020 2020 2020  _views().       
-0000b8b0: 206c 6179 6572 5f76 6965 7773 2e74 6f5f   layer_views.to_
-0000b8c0: 6c79 7028 6669 6c65 7061 7468 3d6c 7970  lyp(filepath=lyp
-0000b8d0: 5f70 6174 6829 0a0a 2020 2020 2020 2020  _path)..        
-0000b8e0: 6c61 796f 7574 203d 204c 6179 6f75 7456  layout = LayoutV
-0000b8f0: 6965 7765 7228 6764 7370 6174 682c 206c  iewer(gdspath, l
-0000b900: 7970 5f70 6174 6829 0a20 2020 2020 2020  yp_path).       
-0000b910: 2064 6973 706c 6179 286c 6179 6f75 742e   display(layout.
-0000b920: 7769 6467 6574 290a 0a20 2020 2064 6566  widget)..    def
-0000b930: 2070 6c6f 745f 6b6c 6179 6f75 7428 0a20   plot_klayout(. 
-0000b940: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000b950: 2020 2020 2073 686f 775f 706f 7274 733a       show_ports:
-0000b960: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
-0000b970: 2020 2020 2020 706f 7274 5f6d 6172 6b65        port_marke
-0000b980: 725f 6c61 7965 723a 204c 6179 6572 203d  r_layer: Layer =
-0000b990: 2028 312c 2031 3029 2c0a 2020 2020 2020   (1, 10),.      
-0000b9a0: 2020 7368 6f77 5f6c 6162 656c 733a 2062    show_labels: b
-0000b9b0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0000b9c0: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
-0000b9d0: 2020 2020 2222 2252 6574 7572 6e73 206b      """Returns k
-0000b9e0: 6c61 796f 7574 2069 6d61 6765 2e0a 0a20  layout image... 
-0000b9f0: 2020 2020 2020 2049 6620 6974 2066 6169         If it fai
-0000ba00: 6c73 2074 6f20 696d 706f 7274 206b 6c61  ls to import kla
-0000ba10: 796f 7574 2064 6566 6175 6c74 7320 746f  yout defaults to
-0000ba20: 206d 6174 706c 6f74 6c69 622e 0a0a 2020   matplotlib...  
-0000ba30: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0000ba40: 2020 2020 2020 2020 7368 6f77 5f70 6f72          show_por
-0000ba50: 7473 3a20 7368 6f77 7320 636f 6d70 6f6e  ts: shows compon
-0000ba60: 656e 7420 7769 7468 2070 6f72 7420 6d61  ent with port ma
-0000ba70: 726b 6572 7320 616e 6420 6c61 6265 6c73  rkers and labels
-0000ba80: 2e0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-0000ba90: 7274 5f6d 6172 6b65 725f 6c61 7965 723a  rt_marker_layer:
-0000baa0: 2066 6f72 2074 6865 2070 6f72 7473 2e0a   for the ports..
-0000bab0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-0000bac0: 5f6c 6162 656c 733a 2073 686f 7773 206c  _labels: shows l
-0000bad0: 6162 656c 732e 0a20 2020 2020 2020 2022  abels..        "
-0000bae0: 2222 0a0a 2020 2020 2020 2020 636f 6d70  ""..        comp
-0000baf0: 6f6e 656e 7420 3d20 280a 2020 2020 2020  onent = (.      
-0000bb00: 2020 2020 2020 7365 6c66 2e61 6464 5f70        self.add_p
-0000bb10: 696e 735f 7472 6961 6e67 6c65 2870 6f72  ins_triangle(por
-0000bb20: 745f 6d61 726b 6572 5f6c 6179 6572 3d70  t_marker_layer=p
-0000bb30: 6f72 745f 6d61 726b 6572 5f6c 6179 6572  ort_marker_layer
-0000bb40: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000bb50: 2073 686f 775f 706f 7274 730a 2020 2020   show_ports.    
-0000bb60: 2020 2020 2020 2020 656c 7365 2073 656c          else sel
-0000bb70: 660a 2020 2020 2020 2020 290a 0a20 2020  f.        )..   
-0000bb80: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000bb90: 2020 2020 2020 696d 706f 7274 206b 6c61        import kla
-0000bba0: 796f 7574 2e64 6220 6173 2064 6220 2023  yout.db as db  #
-0000bbb0: 206e 6f71 613a 2046 3430 310a 2020 2020   noqa: F401.    
-0000bbc0: 2020 2020 2020 2020 696d 706f 7274 206b          import k
-0000bbd0: 6c61 796f 7574 2e6c 6179 2061 7320 6c61  layout.lay as la
-0000bbe0: 790a 2020 2020 2020 2020 2020 2020 6672  y.            fr
-0000bbf0: 6f6d 2067 6473 6661 6374 6f72 792e 7064  om gdsfactory.pd
-0000bc00: 6b20 696d 706f 7274 2067 6574 5f6c 6179  k import get_lay
-0000bc10: 6572 5f76 6965 7773 0a20 2020 2020 2020  er_views.       
-0000bc20: 2020 2020 2066 726f 6d20 4950 7974 686f       from IPytho
-0000bc30: 6e2e 6469 7370 6c61 7920 696d 706f 7274  n.display import
-0000bc40: 2064 6973 706c 6179 0a20 2020 2020 2020   display.       
-0000bc50: 2020 2020 2066 726f 6d20 6970 7977 6964       from ipywid
-0000bc60: 6765 7473 2069 6d70 6f72 7420 496d 6167  gets import Imag
-0000bc70: 650a 0a20 2020 2020 2020 2020 2020 2067  e..            g
-0000bc80: 6473 7061 7468 203d 2063 6f6d 706f 6e65  dspath = compone
-0000bc90: 6e74 2e77 7269 7465 5f67 6473 286c 6f67  nt.write_gds(log
-0000bca0: 6769 6e67 3d46 616c 7365 290a 2020 2020  ging=False).    
-0000bcb0: 2020 2020 2020 2020 6c79 705f 7061 7468          lyp_path
-0000bcc0: 203d 2067 6473 7061 7468 2e77 6974 685f   = gdspath.with_
-0000bcd0: 7375 6666 6978 2822 2e6c 7970 2229 0a0a  suffix(".lyp")..
-0000bce0: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-0000bcf0: 725f 7669 6577 7320 3d20 6765 745f 6c61  r_views = get_la
-0000bd00: 7965 725f 7669 6577 7328 290a 2020 2020  yer_views().    
-0000bd10: 2020 2020 2020 2020 6c61 7965 725f 7669          layer_vi
-0000bd20: 6577 732e 746f 5f6c 7970 2866 696c 6570  ews.to_lyp(filep
-0000bd30: 6174 683d 6c79 705f 7061 7468 290a 0a20  ath=lyp_path).. 
-0000bd40: 2020 2020 2020 2020 2020 206c 6179 6f75             layou
-0000bd50: 745f 7669 6577 203d 206c 6179 2e4c 6179  t_view = lay.Lay
-0000bd60: 6f75 7456 6965 7728 290a 2020 2020 2020  outView().      
-0000bd70: 2020 2020 2020 6c61 796f 7574 5f76 6965        layout_vie
-0000bd80: 772e 6c6f 6164 5f6c 6179 6f75 7428 7374  w.load_layout(st
-0000bd90: 7228 6764 7370 6174 682e 6162 736f 6c75  r(gdspath.absolu
-0000bda0: 7465 2829 2929 0a20 2020 2020 2020 2020  te())).         
-0000bdb0: 2020 206c 6179 6f75 745f 7669 6577 2e6d     layout_view.m
-0000bdc0: 6178 5f68 6965 7228 290a 2020 2020 2020  ax_hier().      
-0000bdd0: 2020 2020 2020 6c61 796f 7574 5f76 6965        layout_vie
-0000bde0: 772e 6c6f 6164 5f6c 6179 6572 5f70 726f  w.load_layer_pro
-0000bdf0: 7073 2873 7472 286c 7970 5f70 6174 6829  ps(str(lyp_path)
-0000be00: 290a 0a20 2020 2020 2020 2020 2020 206c  )..            l
-0000be10: 6179 6f75 745f 7669 6577 2e73 6574 5f63  ayout_view.set_c
-0000be20: 6f6e 6669 6728 2274 6578 742d 7669 7369  onfig("text-visi
-0000be30: 626c 6522 2c20 2274 7275 6522 2069 6620  ble", "true" if 
-0000be40: 7368 6f77 5f6c 6162 656c 7320 656c 7365  show_labels else
-0000be50: 2022 6661 6c73 6522 290a 0a20 2020 2020   "false")..     
-0000be60: 2020 2020 2020 2070 6978 656c 5f62 7566         pixel_buf
-0000be70: 6665 7220 3d20 6c61 796f 7574 5f76 6965  fer = layout_vie
-0000be80: 772e 6765 745f 7069 7865 6c73 5f77 6974  w.get_pixels_wit
-0000be90: 685f 6f70 7469 6f6e 7328 3830 302c 2036  h_options(800, 6
-0000bea0: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
-0000beb0: 706e 675f 6461 7461 203d 2070 6978 656c  png_data = pixel
-0000bec0: 5f62 7566 6665 722e 746f 5f70 6e67 5f64  _buffer.to_png_d
-0000bed0: 6174 6128 290a 2020 2020 2020 2020 2020  ata().          
-0000bee0: 2020 696d 6167 6520 3d20 496d 6167 6528    image = Image(
-0000bef0: 7661 6c75 653d 706e 675f 6461 7461 2c20  value=png_data, 
-0000bf00: 666f 726d 6174 3d22 706e 6722 290a 2020  format="png").  
-0000bf10: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
-0000bf20: 7928 696d 6167 6529 0a0a 2020 2020 2020  y(image)..      
-0000bf30: 2020 6578 6365 7074 2049 6d70 6f72 7445    except ImportE
-0000bf40: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-0000bf50: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
-0000bf60: 2020 2020 2020 2020 2022 596f 7520 6361           "You ca
-0000bf70: 6e20 696e 7374 616c 6c20 6070 6970 2069  n install `pip i
-0000bf80: 6e73 7461 6c6c 2067 6473 6661 6374 6f72  nstall gdsfactor
-0000bf90: 795b 6675 6c6c 5d60 2066 6f72 2062 6574  y[full]` for bet
-0000bfa0: 7465 7220 7669 7375 616c 697a 6174 696f  ter visualizatio
-0000bfb0: 6e22 0a20 2020 2020 2020 2020 2020 2029  n".            )
-0000bfc0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
-0000bfd0: 706f 6e65 6e74 2e70 6c6f 7428 706c 6f74  ponent.plot(plot
-0000bfe0: 7465 723d 226d 6174 706c 6f74 6c69 6222  ter="matplotlib"
-0000bff0: 290a 0a20 2020 2064 6566 2070 6c6f 745f  )..    def plot_
-0000c000: 6a75 7079 7465 7228 7365 6c66 293a 0a20  jupyter(self):. 
-0000c010: 2020 2020 2020 2022 2222 5368 6f77 7320         """Shows 
-0000c020: 6375 7272 656e 7420 6764 7320 696e 206b  current gds in k
-0000c030: 6c61 796f 7574 2e20 5573 6573 204b 7765  layout. Uses Kwe
-0000c040: 6220 6966 2073 6572 7665 7220 7275 6e6e  b if server runn
-0000c050: 696e 672e 0a0a 2020 2020 2020 2020 6966  ing...        if
-0000c060: 206e 6f74 2074 7269 6573 2075 7369 6e67   not tries using
-0000c070: 204b 6c61 796f 7574 2077 6964 6765 7420   Klayout widget 
-0000c080: 616e 6420 6669 6e61 6c6c 7920 6465 6661  and finally defa
-0000c090: 756c 7473 2074 6f20 6d61 7470 6c6f 746c  ults to matplotl
-0000c0a0: 6962 2e0a 2020 2020 2020 2020 2222 220a  ib..        """.
-0000c0b0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000c0c0: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
-0000c0d0: 6f73 0a20 2020 2020 2020 2020 2020 2066  os.            f
-0000c0e0: 726f 6d20 6764 7366 6163 746f 7279 2e63  rom gdsfactory.c
-0000c0f0: 6f6e 6669 6720 696d 706f 7274 2050 4154  onfig import PAT
-0000c100: 480a 2020 2020 2020 2020 2020 2020 6672  H.            fr
-0000c110: 6f6d 2067 6473 6661 6374 6f72 792e 7064  om gdsfactory.pd
-0000c120: 6b20 696d 706f 7274 2067 6574 5f6c 6179  k import get_lay
-0000c130: 6572 5f76 6965 7773 0a20 2020 2020 2020  er_views.       
-0000c140: 2020 2020 2066 726f 6d20 4950 7974 686f       from IPytho
-0000c150: 6e2e 6469 7370 6c61 7920 696d 706f 7274  n.display import
-0000c160: 2049 4672 616d 650a 2020 2020 2020 2020   IFrame.        
-0000c170: 2020 2020 696d 706f 7274 206b 7765 622e      import kweb.
-0000c180: 7365 7276 6572 5f6a 7570 7974 6572 2061  server_jupyter a
-0000c190: 7320 6b6a 0a20 2020 2020 2020 2020 2020  s kj.           
-0000c1a0: 2066 726f 6d20 6874 6d6c 2069 6d70 6f72   from html impor
-0000c1b0: 7420 6573 6361 7065 0a0a 2020 2020 2020  t escape..      
-0000c1c0: 2020 2020 2020 6764 7370 6174 6820 3d20        gdspath = 
-0000c1d0: 7365 6c66 2e77 7269 7465 5f67 6473 2867  self.write_gds(g
-0000c1e0: 6473 6469 723d 5041 5448 2e67 6473 6c69  dsdir=PATH.gdsli
-0000c1f0: 6220 2f20 2265 7874 7261 222c 206c 6f67  b / "extra", log
-0000c200: 6769 6e67 3d46 616c 7365 290a 0a20 2020  ging=False)..   
-0000c210: 2020 2020 2020 2020 2064 6972 7061 7468           dirpath
-0000c220: 203d 2047 4453 4449 525f 5445 4d50 0a20   = GDSDIR_TEMP. 
-0000c230: 2020 2020 2020 2020 2020 2064 6972 7061             dirpa
-0000c240: 7468 2e6d 6b64 6972 2865 7869 7374 5f6f  th.mkdir(exist_o
-0000c250: 6b3d 5472 7565 2c20 7061 7265 6e74 733d  k=True, parents=
-0000c260: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-0000c270: 2020 6c79 705f 7061 7468 203d 2064 6972    lyp_path = dir
-0000c280: 7061 7468 202f 2022 6c61 7965 7273 2e6c  path / "layers.l
-0000c290: 7970 220a 0a20 2020 2020 2020 2020 2020  yp"..           
-0000c2a0: 206c 6179 6572 5f70 726f 7073 203d 2067   layer_props = g
-0000c2b0: 6574 5f6c 6179 6572 5f76 6965 7773 2829  et_layer_views()
-0000c2c0: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-0000c2d0: 6572 5f70 726f 7073 2e74 6f5f 6c79 7028  er_props.to_lyp(
-0000c2e0: 6669 6c65 7061 7468 3d6c 7970 5f70 6174  filepath=lyp_pat
-0000c2f0: 6829 0a0a 2020 2020 2020 2020 2020 2020  h)..            
-0000c300: 7372 6320 3d20 6622 6874 7470 3a2f 2f31  src = f"http://1
-0000c310: 3237 2e30 2e30 2e31 3a7b 6b6a 2e70 6f72  27.0.0.1:{kj.por
-0000c320: 747d 2f67 6473 3f67 6473 5f66 696c 653d  t}/gds?gds_file=
-0000c330: 7b65 7363 6170 6528 7374 7228 6764 7370  {escape(str(gdsp
-0000c340: 6174 6829 297d 266c 6179 6572 5f70 726f  ath))}&layer_pro
-0000c350: 7073 3d7b 6573 6361 7065 2873 7472 286c  ps={escape(str(l
-0000c360: 7970 5f70 6174 6829 297d 220a 2020 2020  yp_path))}".    
-0000c370: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000c380: 6562 7567 2873 7263 290a 0a20 2020 2020  ebug(src)..     
-0000c390: 2020 2020 2020 2069 6620 6b6a 2e6a 7570         if kj.jup
-0000c3a0: 7974 6572 5f73 6572 7665 7220 616e 6420  yter_server and 
-0000c3b0: 6e6f 7420 6f73 2e65 6e76 6972 6f6e 2e67  not os.environ.g
-0000c3c0: 6574 2822 444f 4353 222c 2046 616c 7365  et("DOCS", False
-0000c3d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000c3e0: 2020 2072 6574 7572 6e20 4946 7261 6d65     return IFrame
-0000c3f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000c400: 2020 2020 2020 7372 633d 7372 632c 0a20        src=src,. 
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c420: 2020 2077 6964 7468 3d31 3430 302c 0a20     width=1400,. 
-0000c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c440: 2020 2068 6569 6768 743d 3630 302c 0a20     height=600,. 
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000c460: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000c470: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000c480: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
-0000c490: 6c6f 745f 6b6c 6179 6f75 7428 290a 2020  lot_klayout().  
-0000c4a0: 2020 2020 2020 6578 6365 7074 2049 6d70        except Imp
-0000c4b0: 6f72 7445 7272 6f72 3a0a 2020 2020 2020  ortError:.      
-0000c4c0: 2020 2020 2020 7072 696e 7428 0a20 2020        print(.   
-0000c4d0: 2020 2020 2020 2020 2020 2020 2022 596f               "Yo
-0000c4e0: 7520 6361 6e20 696e 7374 616c 6c20 6070  u can install `p
-0000c4f0: 6970 2069 6e73 7461 6c6c 2067 6473 6661  ip install gdsfa
-0000c500: 6374 6f72 795b 6675 6c6c 5d60 2066 6f72  ctory[full]` for
-0000c510: 2062 6574 7465 7220 7669 7375 616c 697a   better visualiz
-0000c520: 6174 696f 6e22 0a20 2020 2020 2020 2020  ation".         
-0000c530: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000c540: 2072 6574 7572 6e20 7365 6c66 2e70 6c6f   return self.plo
-0000c550: 745f 6b6c 6179 6f75 7428 290a 0a20 2020  t_klayout()..   
-0000c560: 2064 6566 2070 6c6f 745f 6d61 7470 6c6f   def plot_matplo
-0000c570: 746c 6962 2873 656c 662c 202a 2a6b 7761  tlib(self, **kwa
-0000c580: 7267 7329 202d 3e20 4e6f 6e65 3a0a 2020  rgs) -> None:.  
-0000c590: 2020 2020 2020 2222 2250 6c6f 7420 636f        """Plot co
-0000c5a0: 6d70 6f6e 656e 7420 7573 696e 6720 6d61  mponent using ma
-0000c5b0: 7470 6c6f 746c 6962 2e0a 0a20 2020 2020  tplotlib...     
-0000c5c0: 2020 204b 6579 776f 7264 2041 7267 733a     Keyword Args:
-0000c5d0: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
-0000c5e0: 775f 706f 7274 733a 2053 6574 7320 7768  w_ports: Sets wh
-0000c5f0: 6574 6865 7220 706f 7274 7320 6172 6520  ether ports are 
-0000c600: 6472 6177 6e2e 0a20 2020 2020 2020 2020  drawn..         
-0000c610: 2020 2073 686f 775f 7375 6270 6f72 7473     show_subports
-0000c620: 3a20 5365 7473 2077 6865 7468 6572 2073  : Sets whether s
-0000c630: 7562 706f 7274 7320 2870 6f72 7473 2074  ubports (ports t
-0000c640: 6861 7420 6265 6c6f 6e67 2074 6f20 7265  hat belong to re
-0000c650: 6665 7265 6e63 6573 2920 6172 6520 6472  ferences) are dr
-0000c660: 6177 6e2e 0a20 2020 2020 2020 2020 2020  awn..           
-0000c670: 206c 6162 656c 5f61 6c69 6173 6573 3a20   label_aliases: 
-0000c680: 5365 7473 2077 6865 7468 6572 2061 6c69  Sets whether ali
-0000c690: 6173 6573 2061 7265 206c 6162 656c 6564  ases are labeled
-0000c6a0: 2077 6974 6820 6120 7465 7874 206e 616d   with a text nam
-0000c6b0: 652e 0a20 2020 2020 2020 2020 2020 206e  e..            n
-0000c6c0: 6577 5f77 696e 646f 773a 2049 6620 5472  ew_window: If Tr
-0000c6d0: 7565 2c20 6561 6368 2063 616c 6c20 746f  ue, each call to
-0000c6e0: 2071 7569 636b 706c 6f74 2829 2077 696c   quickplot() wil
-0000c6f0: 6c20 6765 6e65 7261 7465 2061 2073 6570  l generate a sep
-0000c700: 6172 6174 6520 7769 6e64 6f77 2e0a 2020  arate window..  
-0000c710: 2020 2020 2020 2020 2020 626c 6f63 6b69            blocki
-0000c720: 6e67 3a20 4966 2054 7275 652c 2063 616c  ng: If True, cal
-0000c730: 6c69 6e67 2071 7569 636b 706c 6f74 2829  ling quickplot()
-0000c740: 2077 696c 6c20 7061 7573 6520 6578 6563   will pause exec
-0000c750: 7574 696f 6e20 6f66 2028 2262 6c6f 636b  ution of ("block
-0000c760: 2229 2074 6865 0a20 2020 2020 2020 2020  ") the.         
-0000c770: 2020 2020 2020 2072 656d 6169 6e64 6572         remainder
-0000c780: 206f 6620 7468 6520 7079 7468 6f6e 2063   of the python c
-0000c790: 6f64 6520 756e 7469 6c20 7468 6520 7175  ode until the qu
-0000c7a0: 6963 6b70 6c6f 7428 2920 7769 6e64 6f77  ickplot() window
-0000c7b0: 2069 7320 636c 6f73 6564 2e0a 2020 2020   is closed..    
-0000c7c0: 2020 2020 2020 2020 2020 2020 4966 2046              If F
-0000c7d0: 616c 7365 2c20 7468 6520 7769 6e64 6f77  alse, the window
-0000c7e0: 2077 696c 6c20 6265 206f 7065 6e65 6420   will be opened 
-0000c7f0: 616e 6420 636f 6465 2077 696c 6c20 636f  and code will co
-0000c800: 6e74 696e 7565 2074 6f20 7275 6e2e 0a20  ntinue to run.. 
-0000c810: 2020 2020 2020 2020 2020 207a 6f6f 6d5f             zoom_
-0000c820: 6661 6374 6f72 3a20 5365 7473 2074 6865  factor: Sets the
-0000c830: 2073 6361 6c69 6e67 2066 6163 746f 7220   scaling factor 
-0000c840: 7768 656e 207a 6f6f 6d69 6e67 2074 6865  when zooming the
-0000c850: 2071 7569 636b 706c 6f74 2077 696e 646f   quickplot windo
-0000c860: 7720 7769 7468 2074 6865 0a20 2020 2020  w with the.     
-0000c870: 2020 2020 2020 2020 2020 206d 6f75 7365             mouse
-0000c880: 7768 6565 6c2f 7472 6163 6b70 6164 2e0a  wheel/trackpad..
-0000c890: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-0000c8a0: 7261 6374 6976 655f 7a6f 6f6d 3a20 456e  ractive_zoom: En
-0000c8b0: 6162 6c65 7320 7573 696e 6720 6d6f 7573  ables using mous
-0000c8c0: 6577 6865 656c 2f74 7261 636b 7061 6420  ewheel/trackpad 
-0000c8d0: 746f 207a 6f6f 6d2e 0a20 2020 2020 2020  to zoom..       
-0000c8e0: 2020 2020 2066 6f6e 7473 697a 653a 2066       fontsize: f
-0000c8f0: 6f72 206c 6162 656c 732e 0a20 2020 2020  or labels..     
-0000c900: 2020 2020 2020 206c 6179 6572 735f 6578         layers_ex
-0000c910: 636c 7564 6564 3a20 6c69 7374 206f 6620  cluded: list of 
-0000c920: 6c61 7965 7273 2074 6f20 6578 636c 7564  layers to exclud
-0000c930: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
-0000c940: 6179 6572 5f76 6965 7773 3a20 6c61 7965  ayer_views: laye
-0000c950: 725f 7669 6577 7320 636f 6c6f 7273 206c  r_views colors l
-0000c960: 6f61 6465 6420 6672 6f6d 204b 6c61 796f  oaded from Klayo
-0000c970: 7574 2e0a 2020 2020 2020 2020 2020 2020  ut..            
-0000c980: 6d69 6e5f 6173 7065 6374 3a20 6d69 6e69  min_aspect: mini
-0000c990: 6d75 6d20 6173 7065 6374 2072 6174 696f  mum aspect ratio
-0000c9a0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000c9b0: 2020 2020 2020 6672 6f6d 2067 6473 6661        from gdsfa
-0000c9c0: 6374 6f72 792e 7175 6963 6b70 6c6f 7474  ctory.quickplott
-0000c9d0: 6572 2069 6d70 6f72 7420 7175 6963 6b70  er import quickp
-0000c9e0: 6c6f 740a 0a20 2020 2020 2020 2071 7569  lot..        qui
-0000c9f0: 636b 706c 6f74 2873 656c 662c 202a 2a6b  ckplot(self, **k
-0000ca00: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
-0000ca10: 706c 6f74 2873 656c 662c 2070 6c6f 7474  plot(self, plott
-0000ca20: 6572 3a20 4f70 7469 6f6e 616c 5b50 6c6f  er: Optional[Plo
-0000ca30: 7474 6572 5d20 3d20 4e6f 6e65 2c20 2a2a  tter] = None, **
-0000ca40: 6b77 6172 6773 2920 2d3e 204e 6f6e 653a  kwargs) -> None:
-0000ca50: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-0000ca60: 726e 7320 636f 6d70 6f6e 656e 7420 706c  rns component pl
-0000ca70: 6f74 2075 7369 6e67 206b 6c61 796f 7574  ot using klayout
-0000ca80: 2c20 6d61 7470 6c6f 746c 6962 2c20 686f  , matplotlib, ho
-0000ca90: 6c6f 7669 6577 7320 6f72 2071 742e 0a0a  loviews or qt...
-0000caa0: 2020 2020 2020 2020 5765 2072 6563 6f6d          We recom
-0000cab0: 6d65 6e64 2075 7369 6e67 206b 6c61 796f  mend using klayo
-0000cac0: 7574 2e0a 0a20 2020 2020 2020 2041 7267  ut...        Arg
-0000cad0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
-0000cae0: 6c6f 7474 6572 3a20 706c 6f74 2062 6163  lotter: plot bac
-0000caf0: 6b65 6e64 2028 2768 6f6c 6f76 6965 7773  kend ('holoviews
-0000cb00: 272c 2027 6d61 7470 6c6f 746c 6962 272c  ', 'matplotlib',
-0000cb10: 2027 7174 272c 2027 6b6c 6179 6f75 7427   'qt', 'klayout'
-0000cb20: 292e 0a20 2020 2020 2020 2022 2222 0a20  )..        """. 
-0000cb30: 2020 2020 2020 2070 6c6f 7474 6572 203d         plotter =
-0000cb40: 2070 6c6f 7474 6572 206f 7220 434f 4e46   plotter or CONF
-0000cb50: 2e67 6574 2822 706c 6f74 7465 7222 2c20  .get("plotter", 
-0000cb60: 226d 6174 706c 6f74 6c69 6222 290a 0a20  "matplotlib").. 
-0000cb70: 2020 2020 2020 2069 6620 706c 6f74 7465         if plotte
-0000cb80: 7220 3d3d 2022 6b6c 6179 6f75 7422 3a0a  r == "klayout":.
-0000cb90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cba0: 2e70 6c6f 745f 6b6c 6179 6f75 7428 290a  .plot_klayout().
-0000cbb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000cbc0: 726e 0a0a 2020 2020 2020 2020 656c 6966  rn..        elif
-0000cbd0: 2070 6c6f 7474 6572 203d 3d20 226d 6174   plotter == "mat
-0000cbe0: 706c 6f74 6c69 6222 3a0a 2020 2020 2020  plotlib":.      
-0000cbf0: 2020 2020 2020 6672 6f6d 2067 6473 6661        from gdsfa
-0000cc00: 6374 6f72 792e 7175 6963 6b70 6c6f 7474  ctory.quickplott
-0000cc10: 6572 2069 6d70 6f72 7420 7175 6963 6b70  er import quickp
-0000cc20: 6c6f 740a 0a20 2020 2020 2020 2020 2020  lot..           
-0000cc30: 2071 7569 636b 706c 6f74 2873 656c 662c   quickplot(self,
-0000cc40: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-0000cc50: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-0000cc60: 2020 2020 2020 2065 6c69 6620 706c 6f74         elif plot
-0000cc70: 7465 7220 3d3d 2022 686f 6c6f 7669 6577  ter == "holoview
-0000cc80: 7322 3a0a 2020 2020 2020 2020 2020 2020  s":.            
-0000cc90: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000cca0: 2020 2020 2069 6d70 6f72 7420 686f 6c6f       import holo
-0000ccb0: 7669 6577 7320 6173 2068 760a 0a20 2020  views as hv..   
-0000ccc0: 2020 2020 2020 2020 2020 2020 2068 762e               hv.
-0000ccd0: 6578 7465 6e73 696f 6e28 2262 6f6b 6568  extension("bokeh
-0000cce0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-0000ccf0: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
-0000cd00: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
-0000cd10: 2020 2020 2020 2020 7072 696e 7428 2279          print("y
-0000cd20: 6f75 206e 6565 6420 746f 2060 7069 7020  ou need to `pip 
-0000cd30: 696e 7374 616c 6c20 686f 6c6f 7669 6577  install holoview
-0000cd40: 7360 2229 0a20 2020 2020 2020 2020 2020  s`").           
-0000cd50: 2020 2020 2072 6169 7365 2065 0a20 2020       raise e.   
-0000cd60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000cd70: 7365 6c66 2e70 6c6f 745f 686f 6c6f 7669  self.plot_holovi
-0000cd80: 6577 7328 2a2a 6b77 6172 6773 290a 0a20  ews(**kwargs).. 
-0000cd90: 2020 2020 2020 2065 6c69 6620 706c 6f74         elif plot
-0000cda0: 7465 7220 3d3d 2022 7174 223a 0a20 2020  ter == "qt":.   
-0000cdb0: 2020 2020 2020 2020 2066 726f 6d20 6764           from gd
-0000cdc0: 7366 6163 746f 7279 2e71 7569 636b 706c  sfactory.quickpl
-0000cdd0: 6f74 7465 7220 696d 706f 7274 2071 7569  otter import qui
-0000cde0: 636b 706c 6f74 320a 0a20 2020 2020 2020  ckplot2..       
-0000cdf0: 2020 2020 2071 7569 636b 706c 6f74 3228       quickplot2(
-0000ce00: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
-0000ce10: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000ce20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000ce30: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000ce40: 726f 7228 6622 7b70 6c6f 7474 6572 2172  ror(f"{plotter!r
-0000ce50: 7d20 6e6f 7420 696e 207b 506c 6f74 7465  } not in {Plotte
-0000ce60: 727d 2229 0a0a 2020 2020 6465 6620 706c  r}")..    def pl
-0000ce70: 6f74 5f68 6f6c 6f76 6965 7773 280a 2020  ot_holoviews(.  
-0000ce80: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000ce90: 2020 2020 6c61 7965 7273 5f65 7863 6c75      layers_exclu
-0000cea0: 6465 643a 204f 7074 696f 6e61 6c5b 4c61  ded: Optional[La
-0000ceb0: 7965 7273 5d20 3d20 4e6f 6e65 2c0a 2020  yers] = None,.  
-0000cec0: 2020 2020 2020 6c61 7965 725f 7669 6577        layer_view
-0000ced0: 733a 204f 7074 696f 6e61 6c5b 4c61 7965  s: Optional[Laye
-0000cee0: 7256 6965 7773 5d20 3d20 4e6f 6e65 2c0a  rViews] = None,.
-0000cef0: 2020 2020 2020 2020 6d69 6e5f 6173 7065          min_aspe
-0000cf00: 6374 3a20 666c 6f61 7420 3d20 302e 3235  ct: float = 0.25
-0000cf10: 2c0a 2020 2020 2020 2020 7061 6464 696e  ,.        paddin
-0000cf20: 673a 2066 6c6f 6174 203d 2030 2e35 2c0a  g: float = 0.5,.
-0000cf30: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-0000cf40: 2222 506c 6f74 2063 6f6d 706f 6e65 6e74  ""Plot component
-0000cf50: 2069 6e20 686f 6c6f 7669 6577 732e 0a0a   in holoviews...
-0000cf60: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000cf70: 2020 2020 2020 2020 2020 6c61 7965 7273            layers
-0000cf80: 5f65 7863 6c75 6465 643a 206c 6973 7420  _excluded: list 
-0000cf90: 6f66 206c 6179 6572 7320 746f 2065 7863  of layers to exc
-0000cfa0: 6c75 6465 2e0a 2020 2020 2020 2020 2020  lude..          
-0000cfb0: 2020 6c61 7965 725f 7669 6577 733a 206c    layer_views: l
-0000cfc0: 6179 6572 5f76 6965 7773 2063 6f6c 6f72  ayer_views color
-0000cfd0: 7320 6c6f 6164 6564 2066 726f 6d20 4b6c  s loaded from Kl
-0000cfe0: 6179 6f75 742e 0a20 2020 2020 2020 2020  ayout..         
-0000cff0: 2020 206d 696e 5f61 7370 6563 743a 206d     min_aspect: m
-0000d000: 696e 696d 756d 2061 7370 6563 7420 7261  inimum aspect ra
-0000d010: 7469 6f2e 0a20 2020 2020 2020 2020 2020  tio..           
-0000d020: 2070 6164 6469 6e67 3a20 6172 6f75 6e64   padding: around
-0000d030: 2062 6f75 6e64 696e 6720 626f 782e 0a0a   bounding box...
-0000d040: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0000d050: 0a20 2020 2020 2020 2020 2020 2048 6f6c  .            Hol
-0000d060: 6f76 6965 7773 204f 7665 726c 6179 2074  oviews Overlay t
-0000d070: 6f20 6469 7370 6c61 7920 616c 6c20 706f  o display all po
-0000d080: 6c79 676f 6e73 2e0a 2020 2020 2020 2020  lygons..        
-0000d090: 2222 220a 2020 2020 2020 2020 6672 6f6d  """.        from
-0000d0a0: 2067 6473 6661 6374 6f72 792e 6164 645f   gdsfactory.add_
-0000d0b0: 7069 6e73 2069 6d70 6f72 7420 6765 745f  pins import get_
-0000d0c0: 7069 6e5f 7472 6961 6e67 6c65 5f70 6f6c  pin_triangle_pol
-0000d0d0: 7967 6f6e 5f74 6970 0a20 2020 2020 2020  ygon_tip.       
-0000d0e0: 2066 726f 6d20 6764 7366 6163 746f 7279   from gdsfactory
-0000d0f0: 2e67 656e 6572 6963 5f74 6563 6820 696d  .generic_tech im
-0000d100: 706f 7274 204c 4159 4552 5f56 4945 5753  port LAYER_VIEWS
-0000d110: 0a0a 2020 2020 2020 2020 6966 206c 6179  ..        if lay
-0000d120: 6572 5f76 6965 7773 2069 7320 4e6f 6e65  er_views is None
-0000d130: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
-0000d140: 7965 725f 7669 6577 7320 3d20 4c41 5945  yer_views = LAYE
-0000d150: 525f 5649 4557 530a 0a20 2020 2020 2020  R_VIEWS..       
-0000d160: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000d170: 2020 696d 706f 7274 2068 6f6c 6f76 6965    import holovie
-0000d180: 7773 2061 7320 6876 0a0a 2020 2020 2020  ws as hv..      
-0000d190: 2020 2020 2020 6876 2e65 7874 656e 7369        hv.extensi
-0000d1a0: 6f6e 2822 626f 6b65 6822 290a 2020 2020  on("bokeh").    
-0000d1b0: 2020 2020 6578 6365 7074 2049 6d70 6f72      except Impor
-0000d1c0: 7445 7272 6f72 2061 7320 653a 0a20 2020  tError as e:.   
-0000d1d0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-0000d1e0: 796f 7520 6e65 6564 2074 6f20 6070 6970  you need to `pip
-0000d1f0: 2069 6e73 7461 6c6c 2068 6f6c 6f76 6965   install holovie
-0000d200: 7773 6022 290a 2020 2020 2020 2020 2020  ws`").          
-0000d210: 2020 7261 6973 6520 650a 0a20 2020 2020    raise e..     
-0000d220: 2020 2073 656c 662e 5f62 625f 7661 6c69     self._bb_vali
-0000d230: 6420 3d20 4661 6c73 6520 2023 2072 6563  d = False  # rec
-0000d240: 6f6d 7075 7465 2074 6865 2062 6f75 6e64  ompute the bound
-0000d250: 696e 6720 626f 780a 2020 2020 2020 2020  ing box.        
-0000d260: 6220 3d20 7365 6c66 2e62 626f 7820 2b20  b = self.bbox + 
-0000d270: 2828 2d70 6164 6469 6e67 2c20 2d70 6164  ((-padding, -pad
-0000d280: 6469 6e67 292c 2028 7061 6464 696e 672c  ding), (padding,
-0000d290: 2070 6164 6469 6e67 2929 0a20 2020 2020   padding)).     
-0000d2a0: 2020 2062 203d 206e 702e 6172 7261 7928     b = np.array(
-0000d2b0: 622e 666c 6174 290a 2020 2020 2020 2020  b.flat).        
-0000d2c0: 6365 6e74 6572 203d 206e 702e 6172 7261  center = np.arra
-0000d2d0: 7928 286e 702e 7375 6d28 625b 3a3a 325d  y((np.sum(b[::2]
-0000d2e0: 2920 2f20 322c 206e 702e 7375 6d28 625b  ) / 2, np.sum(b[
-0000d2f0: 313a 3a32 5d29 202f 2032 2929 0a20 2020  1::2]) / 2)).   
-0000d300: 2020 2020 2073 697a 6520 3d20 6e70 2e61       size = np.a
-0000d310: 7272 6179 2828 6e70 2e61 6273 2862 5b32  rray((np.abs(b[2
-0000d320: 5d20 2d20 625b 305d 292c 206e 702e 6162  ] - b[0]), np.ab
-0000d330: 7328 625b 335d 202d 2062 5b31 5d29 2929  s(b[3] - b[1])))
-0000d340: 0a20 2020 2020 2020 2064 7820 3d20 6e70  .        dx = np
-0000d350: 2e61 7272 6179 280a 2020 2020 2020 2020  .array(.        
-0000d360: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-0000d370: 2020 2020 2020 6e70 2e6d 6178 696d 756d        np.maximum
-0000d380: 286d 696e 5f61 7370 6563 7420 2a20 7369  (min_aspect * si
-0000d390: 7a65 5b31 5d2c 2073 697a 655b 305d 2920  ze[1], size[0]) 
-0000d3a0: 2f20 322c 0a20 2020 2020 2020 2020 2020  / 2,.           
-0000d3b0: 2020 2020 206e 702e 6d61 7869 6d75 6d28       np.maximum(
-0000d3c0: 7369 7a65 5b31 5d2c 206d 696e 5f61 7370  size[1], min_asp
-0000d3d0: 6563 7420 2a20 7369 7a65 5b30 5d29 202f  ect * size[0]) /
-0000d3e0: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
-0000d3f0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-0000d400: 2020 2020 6220 3d20 6e70 2e68 7374 6163      b = np.hstac
-0000d410: 6b28 2863 656e 7465 7220 2d20 6478 2c20  k((center - dx, 
-0000d420: 6365 6e74 6572 202b 2064 7829 290a 0a20  center + dx)).. 
-0000d430: 2020 2020 2020 2070 6c6f 7473 5f74 6f5f         plots_to_
-0000d440: 6f76 6572 6c61 7920 3d20 5b5d 0a20 2020  overlay = [].   
-0000d450: 2020 2020 206c 6179 6572 735f 6578 636c       layers_excl
-0000d460: 7564 6564 203d 205b 5d20 6966 206c 6179  uded = [] if lay
-0000d470: 6572 735f 6578 636c 7564 6564 2069 7320  ers_excluded is 
-0000d480: 4e6f 6e65 2065 6c73 6520 6c61 7965 7273  None else layers
-0000d490: 5f65 7863 6c75 6465 640a 0a20 2020 2020  _excluded..     
-0000d4a0: 2020 2066 6f72 206c 6179 6572 2c20 706f     for layer, po
-0000d4b0: 6c79 676f 6e20 696e 2073 656c 662e 6765  lygon in self.ge
-0000d4c0: 745f 706f 6c79 676f 6e73 2862 795f 7370  t_polygons(by_sp
-0000d4d0: 6563 3d54 7275 6529 2e69 7465 6d73 2829  ec=True).items()
-0000d4e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000d4f0: 206c 6179 6572 2069 6e20 6c61 7965 7273   layer in layers
-0000d500: 5f65 7863 6c75 6465 643a 0a20 2020 2020  _excluded:.     
-0000d510: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000d520: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
-0000d530: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000d540: 2020 2020 2020 6c61 7965 725f 7669 6577        layer_view
-0000d550: 203d 206c 6179 6572 5f76 6965 7773 2e67   = layer_views.g
-0000d560: 6574 5f66 726f 6d5f 7475 706c 6528 6c61  et_from_tuple(la
-0000d570: 7965 7229 0a20 2020 2020 2020 2020 2020  yer).           
-0000d580: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-0000d590: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-0000d5a0: 2020 2020 6c61 7965 7273 203d 206c 6973      layers = lis
-0000d5b0: 7428 6c61 7965 725f 7669 6577 732e 6765  t(layer_views.ge
-0000d5c0: 745f 6c61 7965 725f 7669 6577 7328 292e  t_layer_views().
-0000d5d0: 6b65 7973 2829 290a 2020 2020 2020 2020  keys()).        
-0000d5e0: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-0000d5f0: 2e77 6172 6e28 6622 7b6c 6179 6572 2172  .warn(f"{layer!r
-0000d600: 7d20 6e6f 7420 6465 6669 6e65 6420 696e  } not defined in
-0000d610: 207b 6c61 7965 7273 7d22 290a 2020 2020   {layers}").    
-0000d620: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-0000d630: 725f 7669 6577 203d 204c 6179 6572 5669  r_view = LayerVi
-0000d640: 6577 286c 6179 6572 3d6c 6179 6572 290a  ew(layer=layer).
-0000d650: 2020 2020 2020 2020 2020 2020 2320 544f              # TO
-0000d660: 444f 3a20 4d61 7463 6820 7570 206f 7074  DO: Match up opt
-0000d670: 696f 6e73 2077 6974 6820 4c61 7965 7256  ions with LayerV
-0000d680: 6965 7773 0a20 2020 2020 2020 2020 2020  iews.           
-0000d690: 2070 6c6f 7473 5f74 6f5f 6f76 6572 6c61   plots_to_overla
-0000d6a0: 792e 6170 7065 6e64 280a 2020 2020 2020  y.append(.      
-0000d6b0: 2020 2020 2020 2020 2020 6876 2e50 6f6c            hv.Pol
-0000d6c0: 7967 6f6e 7328 706f 6c79 676f 6e2c 206c  ygons(polygon, l
-0000d6d0: 6162 656c 3d73 7472 286c 6179 6572 5f76  abel=str(layer_v
-0000d6e0: 6965 772e 6e61 6d65 2929 2e6f 7074 7328  iew.name)).opts(
-0000d6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d700: 2020 2020 2064 6174 615f 6173 7065 6374       data_aspect
-0000d710: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
-0000d720: 2020 2020 2020 2020 6672 616d 655f 7769          frame_wi
-0000d730: 6474 683d 3530 302c 0a20 2020 2020 2020  dth=500,.       
-0000d740: 2020 2020 2020 2020 2020 2020 2079 6c69               yli
-0000d750: 6d3d 2862 5b31 5d2c 2062 5b33 5d29 2c0a  m=(b[1], b[3]),.
-0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d770: 2020 2020 786c 696d 3d28 625b 305d 2c20      xlim=(b[0], 
-0000d780: 625b 325d 292c 0a20 2020 2020 2020 2020  b[2]),.         
-0000d790: 2020 2020 2020 2020 2020 2066 696c 6c5f             fill_
-0000d7a0: 636f 6c6f 723d 6c61 7965 725f 7669 6577  color=layer_view
-0000d7b0: 2e66 696c 6c5f 636f 6c6f 722e 6173 5f72  .fill_color.as_r
-0000d7c0: 6762 2829 206f 7220 2222 2c0a 2020 2020  gb() or "",.    
-0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7e0: 6c69 6e65 5f63 6f6c 6f72 3d6c 6179 6572  line_color=layer
-0000d7f0: 5f76 6965 772e 6672 616d 655f 636f 6c6f  _view.frame_colo
-0000d800: 722e 6173 5f72 6762 2829 206f 7220 2222  r.as_rgb() or ""
-0000d810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d820: 2020 2020 2020 6669 6c6c 5f61 6c70 6861        fill_alpha
-0000d830: 3d6c 6179 6572 5f76 6965 772e 6765 745f  =layer_view.get_
-0000d840: 616c 7068 6128 2920 6f72 2022 222c 0a20  alpha() or "",. 
-0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d860: 2020 206c 696e 655f 616c 7068 613d 6c61     line_alpha=la
-0000d870: 7965 725f 7669 6577 2e67 6574 5f61 6c70  yer_view.get_alp
-0000d880: 6861 2829 206f 7220 2222 2c0a 2020 2020  ha() or "",.    
-0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8a0: 746f 6f6c 733d 5b22 686f 7665 7222 5d2c  tools=["hover"],
-0000d8b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d8c0: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
-0000d8d0: 0a20 2020 2020 2020 2066 6f72 206e 616d  .        for nam
-0000d8e0: 652c 2070 6f72 7420 696e 2073 656c 662e  e, port in self.
-0000d8f0: 706f 7274 732e 6974 656d 7328 293a 0a20  ports.items():. 
-0000d900: 2020 2020 2020 2020 2020 206e 616d 6520             name 
-0000d910: 3d20 7374 7228 6e61 6d65 290a 2020 2020  = str(name).    
-0000d920: 2020 2020 2020 2020 706f 6c79 676f 6e2c          polygon,
-0000d930: 2070 7469 7020 3d20 6765 745f 7069 6e5f   ptip = get_pin_
-0000d940: 7472 6961 6e67 6c65 5f70 6f6c 7967 6f6e  triangle_polygon
-0000d950: 5f74 6970 2870 6f72 743d 706f 7274 290a  _tip(port=port).
-0000d960: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
-0000d970: 7473 5f74 6f5f 6f76 6572 6c61 792e 6170  ts_to_overlay.ap
-0000d980: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
-0000d990: 2020 2020 2020 6876 2e50 6f6c 7967 6f6e        hv.Polygon
-0000d9a0: 7328 706f 6c79 676f 6e2c 206c 6162 656c  s(polygon, label
-0000d9b0: 3d6e 616d 6529 2e6f 7074 7328 0a20 2020  =name).opts(.   
-0000d9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9d0: 2064 6174 615f 6173 7065 6374 3d31 2c0a   data_aspect=1,.
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 2020 2020 6672 616d 655f 7769 6474 683d      frame_width=
-0000da00: 3530 302c 0a20 2020 2020 2020 2020 2020  500,.           
-0000da10: 2020 2020 2020 2020 2066 696c 6c5f 616c           fill_al
-0000da20: 7068 613d 302c 0a20 2020 2020 2020 2020  pha=0,.         
-0000da30: 2020 2020 2020 2020 2020 2079 6c69 6d3d             ylim=
-0000da40: 2862 5b31 5d2c 2062 5b33 5d29 2c0a 2020  (b[1], b[3]),.  
-0000da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da60: 2020 786c 696d 3d28 625b 305d 2c20 625b    xlim=(b[0], b[
-0000da70: 325d 292c 0a20 2020 2020 2020 2020 2020  2]),.           
-0000da80: 2020 2020 2020 2020 2063 6f6c 6f72 3d22           color="
-0000da90: 7265 6422 2c0a 2020 2020 2020 2020 2020  red",.          
-0000daa0: 2020 2020 2020 2020 2020 6c69 6e65 5f61            line_a
-0000dab0: 6c70 6861 3d6c 6179 6572 5f76 6965 772e  lpha=layer_view.
-0000dac0: 6765 745f 616c 7068 6128 2920 6f72 2022  get_alpha() or "
-0000dad0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000dae0: 2020 2020 2020 2074 6f6f 6c73 3d5b 2268         tools=["h
-0000daf0: 6f76 6572 225d 2c0a 2020 2020 2020 2020  over"],.        
-0000db00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000db10: 2020 2020 2020 2020 2020 2a20 6876 2e54            * hv.T
-0000db20: 6578 7428 7074 6970 5b30 5d2c 2070 7469  ext(ptip[0], pti
-0000db30: 705b 315d 2c20 6e61 6d65 290a 2020 2020  p[1], name).    
-0000db40: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000db50: 2020 2072 6574 7572 6e20 6876 2e4f 7665     return hv.Ove
-0000db60: 726c 6179 2870 6c6f 7473 5f74 6f5f 6f76  rlay(plots_to_ov
-0000db70: 6572 6c61 7929 2e6f 7074 7328 0a20 2020  erlay).opts(.   
-0000db80: 2020 2020 2020 2020 2073 686f 775f 6c65           show_le
-0000db90: 6765 6e64 3d54 7275 652c 2073 6861 7265  gend=True, share
-0000dba0: 645f 6178 6573 3d46 616c 7365 2c20 796c  d_axes=False, yl
-0000dbb0: 696d 3d28 625b 315d 2c20 625b 335d 292c  im=(b[1], b[3]),
-0000dbc0: 2078 6c69 6d3d 2862 5b30 5d2c 2062 5b32   xlim=(b[0], b[2
-0000dbd0: 5d29 0a20 2020 2020 2020 2029 0a0a 2020  ]).        )..  
-0000dbe0: 2020 6465 6620 7368 6f77 280a 2020 2020    def show(.    
-0000dbf0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000dc00: 2020 7368 6f77 5f70 6f72 7473 3a20 626f    show_ports: bo
-0000dc10: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-0000dc20: 2020 2020 7368 6f77 5f73 7562 706f 7274      show_subport
-0000dc30: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
-0000dc40: 0a20 2020 2020 2020 2070 6f72 745f 6d61  .        port_ma
-0000dc50: 726b 6572 5f6c 6179 6572 3a20 4c61 7965  rker_layer: Laye
-0000dc60: 7220 3d20 2831 2c20 3130 292c 0a20 2020  r = (1, 10),.   
-0000dc70: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
-0000dc80: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
-0000dc90: 2020 2020 2020 2222 2253 686f 7720 636f        """Show co
-0000dca0: 6d70 6f6e 656e 7420 696e 204b 4c61 796f  mponent in KLayo
-0000dcb0: 7574 2e0a 0a20 2020 2020 2020 2072 6574  ut...        ret
-0000dcc0: 7572 6e73 2061 2063 6f70 7920 6f66 2074  urns a copy of t
-0000dcd0: 6865 2043 6f6d 706f 6e65 6e74 2c20 736f  he Component, so
-0000dce0: 2074 6865 206f 7269 6769 6e61 6c20 636f   the original co
-0000dcf0: 6d70 6f6e 656e 7420 7265 6d61 696e 7320  mponent remains 
-0000dd00: 696e 7461 6374 2e0a 2020 2020 2020 2020  intact..        
-0000dd10: 7769 7468 2070 696e 7320 6d61 726b 6572  with pins marker
-0000dd20: 7320 6f6e 2065 6163 6820 706f 7274 2073  s on each port s
-0000dd30: 686f 775f 706f 7274 7320 3d20 5472 7565  how_ports = True
-0000dd40: 2c20 616e 6420 6f70 7469 6f6e 616c 6c79  , and optionally
-0000dd50: 2061 6c73 6f0a 2020 2020 2020 2020 7468   also.        th
-0000dd60: 6520 706f 7274 7320 6672 6f6d 2074 6865  e ports from the
-0000dd70: 2072 6566 6572 656e 6365 7320 2873 686f   references (sho
-0000dd80: 775f 7375 6270 6f72 7473 3d54 7275 6529  w_subports=True)
-0000dd90: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000dda0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-0000ddb0: 5f70 6f72 7473 3a20 7368 6f77 7320 636f  _ports: shows co
-0000ddc0: 6d70 6f6e 656e 7420 7769 7468 2070 6f72  mponent with por
-0000ddd0: 7420 6d61 726b 6572 7320 616e 6420 6c61  t markers and la
-0000dde0: 6265 6c73 2e0a 2020 2020 2020 2020 2020  bels..          
-0000ddf0: 2020 7368 6f77 5f73 7562 706f 7274 733a    show_subports:
-0000de00: 2061 6464 2070 6f72 7473 206d 6172 6b65   add ports marke
-0000de10: 7273 2061 6e64 206c 6162 656c 7320 746f  rs and labels to
-0000de20: 2072 6566 6572 656e 6365 732e 0a20 2020   references..   
-0000de30: 2020 2020 2020 2020 2070 6f72 745f 6d61           port_ma
-0000de40: 726b 6572 5f6c 6179 6572 3a20 666f 7220  rker_layer: for 
-0000de50: 7468 6520 706f 7274 732e 0a0a 2020 2020  the ports...    
-0000de60: 2020 2020 4b65 7977 6f72 6420 4172 6773      Keyword Args
-0000de70: 3a0a 2020 2020 2020 2020 2020 2020 6764  :.            gd
-0000de80: 7370 6174 683a 2047 4453 2066 696c 6520  spath: GDS file 
-0000de90: 7061 7468 2074 6f20 7772 6974 6520 746f  path to write to
-0000dea0: 2e0a 2020 2020 2020 2020 2020 2020 6764  ..            gd
-0000deb0: 7364 6972 3a20 6469 7265 6374 6f72 7920  sdir: directory 
-0000dec0: 666f 7220 7468 6520 4744 5320 6669 6c65  for the GDS file
-0000ded0: 2e20 4465 6661 756c 7473 2074 6f20 2f74  . Defaults to /t
-0000dee0: 6d70 2f2e 0a20 2020 2020 2020 2020 2020  mp/..           
-0000def0: 2075 6e69 743a 2075 6e69 7420 7369 7a65   unit: unit size
-0000df00: 2066 6f72 206f 626a 6563 7473 2069 6e20   for objects in 
-0000df10: 6c69 6272 6172 792e 2031 756d 2062 7920  library. 1um by 
-0000df20: 6465 6661 756c 742e 0a20 2020 2020 2020  default..       
-0000df30: 2020 2020 2070 7265 6369 7369 6f6e 3a20       precision: 
-0000df40: 666f 7220 6f62 6a65 6374 2064 696d 656e  for object dimen
-0000df50: 7369 6f6e 7320 696e 2074 6865 206c 6962  sions in the lib
-0000df60: 7261 7279 2028 6d29 2e20 316e 6d20 6279  rary (m). 1nm by
-0000df70: 2064 6566 6175 6c74 2e0a 2020 2020 2020   default..      
-0000df80: 2020 2020 2020 7469 6d65 7374 616d 703a        timestamp:
-0000df90: 2044 6566 6175 6c74 7320 746f 2032 3031   Defaults to 201
-0000dfa0: 392d 3130 2d32 352e 2049 6620 4e6f 6e65  9-10-25. If None
-0000dfb0: 2075 7365 7320 6375 7272 656e 7420 7469   uses current ti
-0000dfc0: 6d65 2e0a 2020 2020 2020 2020 2222 220a  me..        """.
-0000dfd0: 2020 2020 2020 2020 6672 6f6d 2067 6473          from gds
-0000dfe0: 6661 6374 6f72 792e 6164 645f 7069 6e73  factory.add_pins
-0000dff0: 2069 6d70 6f72 7420 6164 645f 7069 6e73   import add_pins
-0000e000: 5f74 7269 616e 676c 650a 2020 2020 2020  _triangle.      
-0000e010: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
-0000e020: 792e 7368 6f77 2069 6d70 6f72 7420 7368  y.show import sh
-0000e030: 6f77 0a0a 2020 2020 2020 2020 636f 6d70  ow..        comp
-0000e040: 6f6e 656e 7420 3d20 280a 2020 2020 2020  onent = (.      
-0000e050: 2020 2020 2020 7365 6c66 2e61 6464 5f70        self.add_p
-0000e060: 696e 735f 7472 6961 6e67 6c65 2870 6f72  ins_triangle(por
-0000e070: 745f 6d61 726b 6572 5f6c 6179 6572 3d70  t_marker_layer=p
-0000e080: 6f72 745f 6d61 726b 6572 5f6c 6179 6572  ort_marker_layer
-0000e090: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000e0a0: 2073 686f 775f 706f 7274 730a 2020 2020   show_ports.    
-0000e0b0: 2020 2020 2020 2020 656c 7365 2073 656c          else sel
-0000e0c0: 660a 2020 2020 2020 2020 290a 0a20 2020  f.        )..   
-0000e0d0: 2020 2020 2069 6620 7368 6f77 5f73 7562       if show_sub
-0000e0e0: 706f 7274 733a 0a20 2020 2020 2020 2020  ports:.         
-0000e0f0: 2020 2063 6f6d 706f 6e65 6e74 203d 2073     component = s
-0000e100: 656c 662e 636f 7079 2829 0a20 2020 2020  elf.copy().     
-0000e110: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
-0000e120: 2e6e 616d 6520 3d20 7365 6c66 2e6e 616d  .name = self.nam
-0000e130: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
-0000e140: 7220 7265 6665 7265 6e63 6520 696e 2063  r reference in c
-0000e150: 6f6d 706f 6e65 6e74 2e72 6566 6572 656e  omponent.referen
-0000e160: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
-0000e170: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0000e180: 6365 2863 6f6d 706f 6e65 6e74 2c20 436f  ce(component, Co
-0000e190: 6d70 6f6e 656e 7452 6566 6572 656e 6365  mponentReference
-0000e1a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000e1b0: 2020 2020 2020 2061 6464 5f70 696e 735f         add_pins_
-0000e1c0: 7472 6961 6e67 6c65 280a 2020 2020 2020  triangle(.      
-0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1e0: 2020 636f 6d70 6f6e 656e 743d 636f 6d70    component=comp
-0000e1f0: 6f6e 656e 742c 0a20 2020 2020 2020 2020  onent,.         
-0000e200: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000e210: 6566 6572 656e 6365 3d72 6566 6572 656e  eference=referen
-0000e220: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
-0000e230: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-0000e240: 723d 706f 7274 5f6d 6172 6b65 725f 6c61  r=port_marker_la
-0000e250: 7965 722c 0a20 2020 2020 2020 2020 2020  yer,.           
-0000e260: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000e270: 2020 2020 7368 6f77 2863 6f6d 706f 6e65      show(compone
-0000e280: 6e74 2c20 2a2a 6b77 6172 6773 290a 0a20  nt, **kwargs).. 
-0000e290: 2020 2064 6566 205f 7772 6974 655f 6c69     def _write_li
-0000e2a0: 6272 6172 7928 0a20 2020 2020 2020 2073  brary(.        s
-0000e2b0: 656c 662c 0a20 2020 2020 2020 2067 6473  elf,.        gds
-0000e2c0: 7061 7468 3a20 4f70 7469 6f6e 616c 5b50  path: Optional[P
-0000e2d0: 6174 6854 7970 655d 203d 204e 6f6e 652c  athType] = None,
-0000e2e0: 0a20 2020 2020 2020 2067 6473 6469 723a  .        gdsdir:
-0000e2f0: 204f 7074 696f 6e61 6c5b 5061 7468 5479   Optional[PathTy
-0000e300: 7065 5d20 3d20 4e6f 6e65 2c0a 2020 2020  pe] = None,.    
-0000e310: 2020 2020 7469 6d65 7374 616d 703a 204f      timestamp: O
-0000e320: 7074 696f 6e61 6c5b 6461 7465 7469 6d65  ptional[datetime
-0000e330: 2e64 6174 6574 696d 655d 203d 205f 7469  .datetime] = _ti
-0000e340: 6d65 7374 616d 7032 3031 392c 0a20 2020  mestamp2019,.   
-0000e350: 2020 2020 206c 6f67 6769 6e67 3a20 626f       logging: bo
-0000e360: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
-0000e370: 2020 2077 6974 685f 6f61 7369 733a 2062     with_oasis: b
-0000e380: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0000e390: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
-0000e3a0: 2020 2029 202d 3e20 5061 7468 3a0a 2020     ) -> Path:.  
-0000e3b0: 2020 2020 2020 2222 2257 7269 7465 2063        """Write c
-0000e3c0: 6f6d 706f 6e65 6e74 2074 6f20 4744 5320  omponent to GDS 
-0000e3d0: 6f72 204f 4153 4953 2061 6e64 2072 6574  or OASIS and ret
-0000e3e0: 7572 6e73 2067 6473 7061 7468 2e0a 0a20  urns gdspath... 
-0000e3f0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000e400: 2020 2020 2020 2020 2067 6473 7061 7468           gdspath
-0000e410: 3a20 4744 5320 6669 6c65 2070 6174 6820  : GDS file path 
-0000e420: 746f 2077 7269 7465 2074 6f2e 0a20 2020  to write to..   
-0000e430: 2020 2020 2020 2020 2067 6473 6469 723a           gdsdir:
-0000e440: 2064 6972 6563 746f 7279 2066 6f72 2074   directory for t
-0000e450: 6865 2047 4453 2066 696c 652e 2044 6566  he GDS file. Def
-0000e460: 6175 6c74 7320 746f 202f 746d 702f 7261  aults to /tmp/ra
-0000e470: 6e64 6f6d 4669 6c65 2f67 6473 6661 6374  ndomFile/gdsfact
-0000e480: 6f72 792e 0a20 2020 2020 2020 2020 2020  ory..           
-0000e490: 2074 696d 6573 7461 6d70 3a20 4465 6661   timestamp: Defa
-0000e4a0: 756c 7473 2074 6f20 3230 3139 2d31 302d  ults to 2019-10-
-0000e4b0: 3235 2066 6f72 2063 6f6e 7369 7374 656e  25 for consisten
-0000e4c0: 7420 6861 7368 2e0a 2020 2020 2020 2020  t hash..        
-0000e4d0: 2020 2020 2020 2020 4966 204e 6f6e 6520          If None 
-0000e4e0: 7573 6573 2063 7572 7265 6e74 2074 696d  uses current tim
-0000e4f0: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
-0000e500: 6f67 6769 6e67 3a20 6469 7361 626c 6520  ogging: disable 
-0000e510: 4744 5320 7061 7468 206c 6f67 6769 6e67  GDS path logging
-0000e520: 2c20 666f 7220 6578 616d 706c 6520 666f  , for example fo
-0000e530: 7220 7368 6f77 696e 6720 6974 2069 6e20  r showing it in 
-0000e540: 4b4c 6179 6f75 742e 0a20 2020 2020 2020  KLayout..       
-0000e550: 2020 2020 2077 6974 685f 6f61 7369 733a       with_oasis:
-0000e560: 2049 6620 5472 7565 2c20 6669 6c65 2077   If True, file w
-0000e570: 696c 6c20 6265 2077 7269 7474 656e 2074  ill be written t
-0000e580: 6f20 4f41 5349 532e 204f 7468 6572 7769  o OASIS. Otherwi
-0000e590: 7365 2c20 6669 6c65 2077 696c 6c20 6265  se, file will be
-0000e5a0: 2077 7269 7474 656e 2074 6f20 4744 532e   written to GDS.
-0000e5b0: 0a0a 2020 2020 2020 2020 4b65 7977 6f72  ..        Keywor
-0000e5c0: 6420 4172 6773 3a0a 2020 2020 2020 2020  d Args:.        
-0000e5d0: 2020 2020 4b65 7977 6f72 6420 6172 6775      Keyword argu
-0000e5e0: 6d65 6e74 7320 7769 6c6c 206f 7665 7272  ments will overr
-0000e5f0: 6964 6520 7468 6520 6163 7469 7665 2050  ide the active P
-0000e600: 444b 2773 2064 6566 6175 6c74 2047 6473  DK's default Gds
-0000e610: 5772 6974 6553 6574 7469 6e67 7320 616e  WriteSettings an
-0000e620: 6420 4f61 7369 7357 7269 7465 5365 7474  d OasisWriteSett
-0000e630: 696e 6773 2e0a 0a20 2020 2020 2020 2020  ings...         
-0000e640: 2020 2047 6473 2073 6574 7469 6e67 733a     Gds settings:
-0000e650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e660: 2075 6e69 743a 2075 6e69 7420 7369 7a65   unit: unit size
-0000e670: 2066 6f72 206f 626a 6563 7473 2069 6e20   for objects in 
-0000e680: 6c69 6272 6172 792e 2031 756d 2062 7920  library. 1um by 
-0000e690: 6465 6661 756c 742e 0a20 2020 2020 2020  default..       
-0000e6a0: 2020 2020 2020 2020 2070 7265 6369 7369           precisi
-0000e6b0: 6f6e 3a20 666f 7220 6469 6d65 6e73 696f  on: for dimensio
-0000e6c0: 6e73 2069 6e20 7468 6520 6c69 6272 6172  ns in the librar
-0000e6d0: 7920 286d 292e 2031 6e6d 2062 7920 6465  y (m). 1nm by de
-0000e6e0: 6661 756c 742e 0a20 2020 2020 2020 2020  fault..         
-0000e6f0: 2020 2020 2020 206f 6e5f 6475 706c 6963         on_duplic
-0000e700: 6174 655f 6365 6c6c 3a20 7370 6563 6966  ate_cell: specif
-0000e710: 7920 686f 7720 746f 2072 6573 6f6c 7665  y how to resolve
-0000e720: 2064 7570 6c69 6361 7465 2d6e 616d 6564   duplicate-named
-0000e730: 2063 656c 6c73 2e20 4368 6f6f 7365 206f   cells. Choose o
-0000e740: 6e65 206f 6620 7468 6520 666f 6c6c 6f77  ne of the follow
-0000e750: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-0000e760: 2020 2020 2020 2020 2022 7761 726e 2220           "warn" 
-0000e770: 2864 6566 6175 6c74 293a 206f 7665 7277  (default): overw
-0000e780: 7269 7465 2061 6c6c 2064 7570 6c69 6361  rite all duplica
-0000e790: 7465 2063 656c 6c73 2077 6974 6820 6f6e  te cells with on
-0000e7a0: 6520 6f66 2074 6865 2064 7570 6c69 6361  e of the duplica
-0000e7b0: 7465 7320 2861 7262 6974 7261 7269 6c79  tes (arbitrarily
-0000e7c0: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e7d0: 2020 2020 2020 2022 6572 726f 7222 3a20         "error": 
-0000e7e0: 7468 726f 7720 6120 5661 6c75 6545 7272  throw a ValueErr
-0000e7f0: 6f72 2077 6865 6e20 6174 7465 6d70 7469  or when attempti
-0000e800: 6e67 2074 6f20 7772 6974 6520 6120 6764  ng to write a gd
-0000e810: 7320 7769 7468 2064 7570 6c69 6361 7465  s with duplicate
-0000e820: 2063 656c 6c73 2e0a 2020 2020 2020 2020   cells..        
-0000e830: 2020 2020 2020 2020 2020 2020 226f 7665              "ove
-0000e840: 7277 7269 7465 223a 206f 7665 7277 7269  rwrite": overwri
-0000e850: 7465 2061 6c6c 2064 7570 6c69 6361 7465  te all duplicate
-0000e860: 2063 656c 6c73 2077 6974 6820 6f6e 6520   cells with one 
-0000e870: 6f66 2074 6865 2064 7570 6c69 6361 7465  of the duplicate
-0000e880: 732c 2077 6974 686f 7574 2077 6172 6e69  s, without warni
-0000e890: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-0000e8a0: 2020 2020 2020 2020 4e6f 6e65 3a20 646f          None: do
-0000e8b0: 206e 6f74 2074 7279 2074 6f20 7265 736f   not try to reso
-0000e8c0: 6c76 6520 2861 7420 796f 7572 206f 776e  lve (at your own
-0000e8d0: 2072 6973 6b21 290a 2020 2020 2020 2020   risk!).        
-0000e8e0: 2020 2020 2020 2020 666c 6174 7465 6e5f          flatten_
-0000e8f0: 696e 7661 6c69 645f 7265 6673 3a20 666c  invalid_refs: fl
-0000e900: 6174 7465 6e73 2063 6f6d 706f 6e65 6e74  attens component
-0000e910: 2072 6566 6572 656e 6365 7320 7768 6963   references whic
-0000e920: 6820 6861 7665 2069 6e76 616c 6964 2074  h have invalid t
-0000e930: 7261 6e73 666f 726d 6174 696f 6e73 2e0a  ransformations..
-0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 6d61 785f 706f 696e 7473 3a20 4d61 7869  max_points: Maxi
-0000e960: 6d61 6c20 6e75 6d62 6572 206f 6620 7665  mal number of ve
-0000e970: 7274 6963 6573 2070 6572 2070 6f6c 7967  rtices per polyg
-0000e980: 6f6e 2e20 506f 6c79 676f 6e73 2077 6974  on. Polygons wit
-0000e990: 6820 6d6f 7265 2076 6572 7469 6365 7320  h more vertices 
-0000e9a0: 7468 6174 2074 6869 7320 6172 6520 6175  that this are au
-0000e9b0: 746f 6d61 7469 6361 6c6c 7920 6672 6163  tomatically frac
-0000e9c0: 7475 7265 642e 0a0a 2020 2020 2020 2020  tured...        
-0000e9d0: 2020 2020 4f61 7369 7320 7365 7474 696e      Oasis settin
-0000e9e0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000e9f0: 2020 2020 636f 6d70 7265 7373 696f 6e5f      compression_
-0000ea00: 6c65 7665 6c3a 204c 6576 656c 206f 6620  level: Level of 
-0000ea10: 636f 6d70 7265 7373 696f 6e20 666f 7220  compression for 
-0000ea20: 6365 6c6c 7320 2862 6574 7765 656e 2030  cells (between 0
-0000ea30: 2061 6e64 2039 292e 0a20 2020 2020 2020   and 9)..       
-0000ea40: 2020 2020 2020 2020 2020 2020 2053 6574               Set
-0000ea50: 7469 6e67 2074 6f20 3020 7769 6c6c 2064  ting to 0 will d
-0000ea60: 6973 6162 6c65 2063 656c 6c20 636f 6d70  isable cell comp
-0000ea70: 7265 7373 696f 6e2c 2031 2067 6976 6573  ression, 1 gives
-0000ea80: 2074 6865 2062 6573 7420 7370 6565 6420   the best speed 
-0000ea90: 616e 6420 392c 2074 6865 2062 6573 7420  and 9, the best 
-0000eaa0: 636f 6d70 7265 7373 696f 6e2e 0a20 2020  compression..   
-0000eab0: 2020 2020 2020 2020 2020 2020 2064 6574               det
-0000eac0: 6563 745f 7265 6374 616e 676c 6573 3a20  ect_rectangles: 
-0000ead0: 5374 6f72 6520 7265 6374 616e 676c 6573  Store rectangles
-0000eae0: 2069 6e20 636f 6d70 7265 7373 6564 2066   in compressed f
-0000eaf0: 6f72 6d61 742e 0a20 2020 2020 2020 2020  ormat..         
-0000eb00: 2020 2020 2020 2064 6574 6563 745f 7472         detect_tr
-0000eb10: 6170 657a 6f69 6473 3a20 5374 6f72 6520  apezoids: Store 
-0000eb20: 7472 6170 657a 6f69 6473 2069 6e20 636f  trapezoids in co
-0000eb30: 6d70 7265 7373 6564 2066 6f72 6d61 742e  mpressed format.
-0000eb40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eb50: 2063 6972 636c 655f 746f 6c65 7261 6e63   circle_toleranc
-0000eb60: 653a 2054 6f6c 6572 616e 6365 2066 6f72  e: Tolerance for
-0000eb70: 2064 6574 6563 7469 6e67 2063 6972 636c   detecting circl
-0000eb80: 6573 2e20 4966 206c 6573 7320 6f72 2065  es. If less or e
-0000eb90: 7175 616c 2074 6f20 302c 206e 6f20 6465  qual to 0, no de
-0000eba0: 7465 6374 696f 6e20 6973 2070 6572 666f  tection is perfo
-0000ebb0: 726d 6564 2e20 4369 7263 6c65 7320 6172  rmed. Circles ar
-0000ebc0: 6520 7374 6f72 6564 2069 6e20 636f 6d70  e stored in comp
-0000ebd0: 7265 7373 6564 2066 6f72 6d61 742e 0a20  ressed format.. 
-0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000ebf0: 616c 6964 6174 696f 6e20 2822 6372 6333  alidation ("crc3
-0000ec00: 3222 2c20 2263 6865 636b 7375 6d33 3222  2", "checksum32"
-0000ec10: 2c20 4e6f 6e65 293a 2074 7970 6520 6f66  , None): type of
-0000ec20: 2076 616c 6964 6174 696f 6e20 746f 2069   validation to i
-0000ec30: 6e63 6c75 6465 2069 6e20 7468 6520 7361  nclude in the sa
-0000ec40: 7665 6420 6669 6c65 2e0a 2020 2020 2020  ved file..      
-0000ec50: 2020 2020 2020 2020 2020 7374 616e 6461            standa
-0000ec60: 7264 5f70 726f 7065 7274 6965 733a 2053  rd_properties: S
-0000ec70: 746f 7265 2073 7461 6e64 6172 6420 4f41  tore standard OA
-0000ec80: 5349 5320 7072 6f70 6572 7469 6573 2069  SIS properties i
-0000ec90: 6e20 7468 6520 6669 6c65 2e0a 0a20 2020  n the file...   
-0000eca0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000ecb0: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
-0000ecc0: 792e 7064 6b20 696d 706f 7274 2067 6574  y.pdk import get
-0000ecd0: 5f61 6374 6976 655f 7064 6b0a 0a20 2020  _active_pdk..   
-0000ece0: 2020 2020 2069 6620 6764 7370 6174 6820       if gdspath 
-0000ecf0: 616e 6420 6764 7364 6972 3a0a 2020 2020  and gdsdir:.    
-0000ed00: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-0000ed10: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
-0000ed20: 2020 2020 2020 2022 6764 7370 6174 6820         "gdspath 
-0000ed30: 616e 6420 6764 7364 6972 2068 6176 6520  and gdsdir have 
-0000ed40: 626f 7468 2062 6565 6e20 7370 6563 6966  both been specif
-0000ed50: 6965 642e 2067 6473 7061 7468 2077 696c  ied. gdspath wil
-0000ed60: 6c20 7461 6b65 2070 7265 6365 6465 6e63  l take precedenc
-0000ed70: 6520 616e 6420 6764 7364 6972 2077 696c  e and gdsdir wil
-0000ed80: 6c20 6265 2069 676e 6f72 6564 2e22 0a20  l be ignored.". 
-0000ed90: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000eda0: 2020 2020 2020 6465 6661 756c 745f 7365        default_se
-0000edb0: 7474 696e 6773 203d 2067 6574 5f61 6374  ttings = get_act
-0000edc0: 6976 655f 7064 6b28 292e 6764 735f 7772  ive_pdk().gds_wr
-0000edd0: 6974 655f 7365 7474 696e 6773 0a20 2020  ite_settings.   
-0000ede0: 2020 2020 2064 6566 6175 6c74 5f6f 6173       default_oas
-0000edf0: 6973 5f73 6574 7469 6e67 7320 3d20 6765  is_settings = ge
-0000ee00: 745f 6163 7469 7665 5f70 646b 2829 2e6f  t_active_pdk().o
-0000ee10: 6173 6973 5f73 6574 7469 6e67 730a 0a20  asis_settings.. 
-0000ee20: 2020 2020 2020 2065 7870 6c69 6369 745f         explicit_
-0000ee30: 6764 735f 7365 7474 696e 6773 203d 207b  gds_settings = {
-0000ee40: 0a20 2020 2020 2020 2020 2020 206b 3a20  .            k: 
-0000ee50: 760a 2020 2020 2020 2020 2020 2020 666f  v.            fo
-0000ee60: 7220 6b2c 2076 2069 6e20 6b77 6172 6773  r k, v in kwargs
-0000ee70: 2e69 7465 6d73 2829 0a20 2020 2020 2020  .items().       
-0000ee80: 2020 2020 2069 6620 7620 6973 206e 6f74       if v is not
-0000ee90: 204e 6f6e 6520 616e 6420 6b20 696e 2064   None and k in d
-0000eea0: 6566 6175 6c74 5f73 6574 7469 6e67 732e  efault_settings.
-0000eeb0: 6469 6374 2829 0a20 2020 2020 2020 207d  dict().        }
-0000eec0: 0a20 2020 2020 2020 2065 7870 6c69 6369  .        explici
-0000eed0: 745f 6f61 735f 7365 7474 696e 6773 203d  t_oas_settings =
-0000eee0: 207b 0a20 2020 2020 2020 2020 2020 206b   {.            k
-0000eef0: 3a20 760a 2020 2020 2020 2020 2020 2020  : v.            
-0000ef00: 666f 7220 6b2c 2076 2069 6e20 6b77 6172  for k, v in kwar
-0000ef10: 6773 2e69 7465 6d73 2829 0a20 2020 2020  gs.items().     
-0000ef20: 2020 2020 2020 2069 6620 7620 6973 206e         if v is n
-0000ef30: 6f74 204e 6f6e 6520 616e 6420 6b20 696e  ot None and k in
-0000ef40: 2064 6566 6175 6c74 5f6f 6173 6973 5f73   default_oasis_s
-0000ef50: 6574 7469 6e67 732e 6469 6374 2829 0a20  ettings.dict(). 
-0000ef60: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0000ef70: 2023 2075 7064 6174 6520 7468 6520 7772   # update the wr
-0000ef80: 6974 6520 7365 7474 696e 6773 2077 6974  ite settings wit
-0000ef90: 6820 616e 7920 7365 7474 696e 6773 2065  h any settings e
-0000efa0: 7870 6c69 6369 746c 7920 7061 7373 6564  xplicitly passed
-0000efb0: 0a20 2020 2020 2020 2077 7269 7465 5f73  .        write_s
-0000efc0: 6574 7469 6e67 7320 3d20 6465 6661 756c  ettings = defaul
-0000efd0: 745f 7365 7474 696e 6773 2e63 6f70 7928  t_settings.copy(
-0000efe0: 7570 6461 7465 3d65 7870 6c69 6369 745f  update=explicit_
-0000eff0: 6764 735f 7365 7474 696e 6773 290a 2020  gds_settings).  
-0000f000: 2020 2020 2020 6f61 7369 735f 7365 7474        oasis_sett
-0000f010: 696e 6773 203d 2064 6566 6175 6c74 5f6f  ings = default_o
-0000f020: 6173 6973 5f73 6574 7469 6e67 732e 636f  asis_settings.co
-0000f030: 7079 2875 7064 6174 653d 6578 706c 6963  py(update=explic
-0000f040: 6974 5f6f 6173 5f73 6574 7469 6e67 7329  it_oas_settings)
-0000f050: 0a0a 2020 2020 2020 2020 5f63 6865 636b  ..        _check
-0000f060: 5f75 6e63 6163 6865 645f 636f 6d70 6f6e  _uncached_compon
-0000f070: 656e 7473 280a 2020 2020 2020 2020 2020  ents(.          
-0000f080: 2020 636f 6d70 6f6e 656e 743d 7365 6c66    component=self
-0000f090: 2c20 6d6f 6465 3d77 7269 7465 5f73 6574  , mode=write_set
-0000f0a0: 7469 6e67 732e 6f6e 5f75 6e63 6163 6865  tings.on_uncache
-0000f0b0: 645f 636f 6d70 6f6e 656e 740a 2020 2020  d_component.    
-0000f0c0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-0000f0d0: 6620 7772 6974 655f 7365 7474 696e 6773  f write_settings
-0000f0e0: 2e66 6c61 7474 656e 5f69 6e76 616c 6964  .flatten_invalid
-0000f0f0: 5f72 6566 733a 0a20 2020 2020 2020 2020  _refs:.         
-0000f100: 2020 2074 6f70 5f63 656c 6c20 3d20 666c     top_cell = fl
-0000f110: 6174 7465 6e5f 696e 7661 6c69 645f 7265  atten_invalid_re
-0000f120: 6673 5f72 6563 7572 7369 7665 2873 656c  fs_recursive(sel
-0000f130: 6629 0a20 2020 2020 2020 2065 6c73 653a  f).        else:
-0000f140: 0a20 2020 2020 2020 2020 2020 2074 6f70  .            top
-0000f150: 5f63 656c 6c20 3d20 7365 6c66 0a0a 2020  _cell = self..  
-0000f160: 2020 2020 2020 6764 7364 6972 203d 2067        gdsdir = g
-0000f170: 6473 6469 7220 6f72 2047 4453 4449 525f  dsdir or GDSDIR_
-0000f180: 5445 4d50 0a20 2020 2020 2020 2067 6473  TEMP.        gds
-0000f190: 6469 7220 3d20 7061 7468 6c69 622e 5061  dir = pathlib.Pa
-0000f1a0: 7468 2867 6473 6469 7229 0a20 2020 2020  th(gdsdir).     
-0000f1b0: 2020 2069 6620 7769 7468 5f6f 6173 6973     if with_oasis
-0000f1c0: 3a0a 2020 2020 2020 2020 2020 2020 6764  :.            gd
-0000f1d0: 7370 6174 6820 3d20 6764 7370 6174 6820  spath = gdspath 
-0000f1e0: 6f72 2067 6473 6469 7220 2f20 6622 7b74  or gdsdir / f"{t
-0000f1f0: 6f70 5f63 656c 6c2e 6e61 6d65 7d2e 6f61  op_cell.name}.oa
-0000f200: 7322 0a20 2020 2020 2020 2065 6c73 653a  s".        else:
-0000f210: 0a20 2020 2020 2020 2020 2020 2067 6473  .            gds
-0000f220: 7061 7468 203d 2067 6473 7061 7468 206f  path = gdspath o
-0000f230: 7220 6764 7364 6972 202f 2066 227b 746f  r gdsdir / f"{to
-0000f240: 705f 6365 6c6c 2e6e 616d 657d 2e67 6473  p_cell.name}.gds
-0000f250: 220a 2020 2020 2020 2020 6764 7370 6174  ".        gdspat
-0000f260: 6820 3d20 7061 7468 6c69 622e 5061 7468  h = pathlib.Path
-0000f270: 2867 6473 7061 7468 290a 2020 2020 2020  (gdspath).      
-0000f280: 2020 6764 7364 6972 203d 2067 6473 7061    gdsdir = gdspa
-0000f290: 7468 2e70 6172 656e 740a 2020 2020 2020  th.parent.      
-0000f2a0: 2020 6764 7364 6972 2e6d 6b64 6972 2865    gdsdir.mkdir(e
-0000f2b0: 7869 7374 5f6f 6b3d 5472 7565 2c20 7061  xist_ok=True, pa
-0000f2c0: 7265 6e74 733d 5472 7565 290a 0a20 2020  rents=True)..   
-0000f2d0: 2020 2020 2063 656c 6c73 203d 2074 6f70       cells = top
-0000f2e0: 5f63 656c 6c2e 6765 745f 6465 7065 6e64  _cell.get_depend
-0000f2f0: 656e 6369 6573 2872 6563 7572 7369 7665  encies(recursive
-0000f300: 3d54 7275 6529 0a20 2020 2020 2020 2063  =True).        c
-0000f310: 656c 6c5f 6e61 6d65 7320 3d20 5b63 656c  ell_names = [cel
-0000f320: 6c2e 6e61 6d65 2066 6f72 2063 656c 6c20  l.name for cell 
-0000f330: 696e 206c 6973 7428 6365 6c6c 7329 5d0a  in list(cells)].
-0000f340: 2020 2020 2020 2020 6365 6c6c 5f6e 616d          cell_nam
-0000f350: 6573 5f75 6e69 7175 6520 3d20 7365 7428  es_unique = set(
-0000f360: 6365 6c6c 5f6e 616d 6573 290a 0a20 2020  cell_names)..   
-0000f370: 2020 2020 2069 6620 6c65 6e28 6365 6c6c       if len(cell
-0000f380: 5f6e 616d 6573 2920 213d 206c 656e 2873  _names) != len(s
-0000f390: 6574 2863 656c 6c5f 6e61 6d65 7329 293a  et(cell_names)):
-0000f3a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000f3b0: 2063 656c 6c5f 6e61 6d65 2069 6e20 6365   cell_name in ce
-0000f3c0: 6c6c 5f6e 616d 6573 5f75 6e69 7175 653a  ll_names_unique:
-0000f3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f3e0: 2063 656c 6c5f 6e61 6d65 732e 7265 6d6f   cell_names.remo
-0000f3f0: 7665 2863 656c 6c5f 6e61 6d65 290a 0a20  ve(cell_name).. 
-0000f400: 2020 2020 2020 2020 2020 2069 6620 7772             if wr
-0000f410: 6974 655f 7365 7474 696e 6773 2e6f 6e5f  ite_settings.on_
-0000f420: 6475 706c 6963 6174 655f 6365 6c6c 203d  duplicate_cell =
-0000f430: 3d20 2265 7272 6f72 223a 0a20 2020 2020  = "error":.     
-0000f440: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000f450: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-0000f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f470: 2066 2244 7570 6c69 6361 7465 6420 6365   f"Duplicated ce
-0000f480: 6c6c 206e 616d 6573 2069 6e20 7b74 6f70  ll names in {top
-0000f490: 5f63 656c 6c2e 6e61 6d65 2172 7d3a 207b  _cell.name!r}: {
-0000f4a0: 6365 6c6c 5f6e 616d 6573 2172 7d22 0a20  cell_names!r}". 
-0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000f4c0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0000f4d0: 6620 7772 6974 655f 7365 7474 696e 6773  f write_settings
-0000f4e0: 2e6f 6e5f 6475 706c 6963 6174 655f 6365  .on_duplicate_ce
-0000f4f0: 6c6c 2069 6e20 7b22 7761 726e 222c 2022  ll in {"warn", "
-0000f500: 6f76 6572 7772 6974 6522 7d3a 0a20 2020  overwrite"}:.   
-0000f510: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000f520: 7772 6974 655f 7365 7474 696e 6773 2e6f  write_settings.o
-0000f530: 6e5f 6475 706c 6963 6174 655f 6365 6c6c  n_duplicate_cell
-0000f540: 203d 3d20 2277 6172 6e22 3a0a 2020 2020   == "warn":.    
-0000f550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f560: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
-0000f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f580: 2020 2020 2020 2066 2244 7570 6c69 6361         f"Duplica
-0000f590: 7465 6420 6365 6c6c 206e 616d 6573 2069  ted cell names i
-0000f5a0: 6e20 7b74 6f70 5f63 656c 6c2e 6e61 6d65  n {top_cell.name
-0000f5b0: 2172 7d3a 2020 7b63 656c 6c5f 6e61 6d65  !r}:  {cell_name
-0000f5c0: 737d 222c 0a20 2020 2020 2020 2020 2020  s}",.           
-0000f5d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000f5e0: 2020 2020 2020 2020 2020 2063 656c 6c73             cells
-0000f5f0: 5f64 6963 7420 3d20 7b63 656c 6c2e 6e61  _dict = {cell.na
-0000f600: 6d65 3a20 6365 6c6c 2e5f 6365 6c6c 2066  me: cell._cell f
-0000f610: 6f72 2063 656c 6c20 696e 2063 656c 6c73  or cell in cells
-0000f620: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000f630: 2020 6365 6c6c 7320 3d20 6365 6c6c 735f    cells = cells_
-0000f640: 6469 6374 2e76 616c 7565 7328 290a 2020  dict.values().  
-0000f650: 2020 2020 2020 2020 2020 656c 6966 2077            elif w
-0000f660: 7269 7465 5f73 6574 7469 6e67 732e 6f6e  rite_settings.on
-0000f670: 5f64 7570 6c69 6361 7465 5f63 656c 6c20  _duplicate_cell 
-0000f680: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000f690: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000f6a0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6c0: 2020 2066 226f 6e5f 6475 706c 6963 6174     f"on_duplicat
-0000f6d0: 655f 6365 6c6c 3a20 7b77 7269 7465 5f73  e_cell: {write_s
-0000f6e0: 6574 7469 6e67 732e 6f6e 5f64 7570 6c69  ettings.on_dupli
-0000f6f0: 6361 7465 5f63 656c 6c21 727d 206e 6f74  cate_cell!r} not
-0000f700: 2069 6e20 284e 6f6e 652c 2077 6172 6e2c   in (None, warn,
-0000f710: 2065 7272 6f72 2c20 6f76 6572 7772 6974   error, overwrit
-0000f720: 6529 220a 2020 2020 2020 2020 2020 2020  e)".            
-0000f730: 2020 2020 290a 0a20 2020 2020 2020 2061      )..        a
-0000f740: 6c6c 5f63 656c 6c73 203d 205b 746f 705f  ll_cells = [top_
-0000f750: 6365 6c6c 2e5f 6365 6c6c 5d20 2b20 736f  cell._cell] + so
-0000f760: 7274 6564 2863 656c 6c73 2c20 6b65 793d  rted(cells, key=
-0000f770: 6c61 6d62 6461 2063 633a 2063 632e 6e61  lambda cc: cc.na
-0000f780: 6d65 290a 0a20 2020 2020 2020 206e 6f5f  me)..        no_
-0000f790: 6e61 6d65 5f63 656c 6c73 203d 205b 0a20  name_cells = [. 
-0000f7a0: 2020 2020 2020 2020 2020 2063 656c 6c2e             cell.
-0000f7b0: 6e61 6d65 2066 6f72 2063 656c 6c20 696e  name for cell in
-0000f7c0: 2061 6c6c 5f63 656c 6c73 2069 6620 6365   all_cells if ce
-0000f7d0: 6c6c 2e6e 616d 652e 7374 6172 7473 7769  ll.name.startswi
-0000f7e0: 7468 2822 556e 6e61 6d65 6422 290a 2020  th("Unnamed").  
-0000f7f0: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
-0000f800: 2069 6620 6e6f 5f6e 616d 655f 6365 6c6c   if no_name_cell
-0000f810: 733a 0a20 2020 2020 2020 2020 2020 2077  s:.            w
-0000f820: 6172 6e69 6e67 732e 7761 726e 280a 2020  arnings.warn(.  
-0000f830: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000f840: 436f 6d70 6f6e 656e 7420 7b74 6f70 5f63  Component {top_c
-0000f850: 656c 6c2e 6e61 6d65 2172 7d20 636f 6e74  ell.name!r} cont
-0000f860: 6169 6e73 207b 6c65 6e28 6e6f 5f6e 616d  ains {len(no_nam
-0000f870: 655f 6365 6c6c 7329 7d20 556e 6e61 6d65  e_cells)} Unname
-0000f880: 6420 6365 6c6c 7322 0a20 2020 2020 2020  d cells".       
-0000f890: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000f8a0: 2320 666f 7220 6365 6c6c 2069 6e20 616c  # for cell in al
-0000f8b0: 6c5f 6365 6c6c 733a 0a20 2020 2020 2020  l_cells:.       
-0000f8c0: 2023 2020 2020 2070 7269 6e74 2863 656c   #     print(cel
-0000f8d0: 6c2e 6e61 6d65 2c20 7479 7065 2863 656c  l.name, type(cel
-0000f8e0: 6c29 290a 0a20 2020 2020 2020 206c 6962  l))..        lib
-0000f8f0: 203d 2067 6473 746b 2e4c 6962 7261 7279   = gdstk.Library
-0000f900: 280a 2020 2020 2020 2020 2020 2020 756e  (.            un
-0000f910: 6974 3d77 7269 7465 5f73 6574 7469 6e67  it=write_setting
-0000f920: 732e 756e 6974 2c20 7072 6563 6973 696f  s.unit, precisio
-0000f930: 6e3d 7772 6974 655f 7365 7474 696e 6773  n=write_settings
-0000f940: 2e70 7265 6369 7369 6f6e 0a20 2020 2020  .precision.     
-0000f950: 2020 2029 0a20 2020 2020 2020 206c 6962     ).        lib
-0000f960: 2e61 6464 2874 6f70 5f63 656c 6c2e 5f63  .add(top_cell._c
-0000f970: 656c 6c29 0a20 2020 2020 2020 206c 6962  ell).        lib
-0000f980: 2e61 6464 282a 746f 705f 6365 6c6c 2e5f  .add(*top_cell._
-0000f990: 6365 6c6c 2e64 6570 656e 6465 6e63 6965  cell.dependencie
-0000f9a0: 7328 5472 7565 2929 0a0a 2020 2020 2020  s(True))..      
-0000f9b0: 2020 6966 2077 6974 685f 6f61 7369 733a    if with_oasis:
-0000f9c0: 0a20 2020 2020 2020 2020 2020 206c 6962  .            lib
-0000f9d0: 2e77 7269 7465 5f6f 6173 2867 6473 7061  .write_oas(gdspa
-0000f9e0: 7468 2c20 2a2a 6f61 7369 735f 7365 7474  th, **oasis_sett
-0000f9f0: 696e 6773 2e64 6963 7428 2929 0a20 2020  ings.dict()).   
-0000fa00: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000fa10: 2020 2020 2020 206c 6962 2e77 7269 7465         lib.write
-0000fa20: 5f67 6473 280a 2020 2020 2020 2020 2020  _gds(.          
-0000fa30: 2020 2020 2020 6764 7370 6174 682c 2074        gdspath, t
-0000fa40: 696d 6573 7461 6d70 3d74 696d 6573 7461  imestamp=timesta
-0000fa50: 6d70 2c20 6d61 785f 706f 696e 7473 3d77  mp, max_points=w
-0000fa60: 7269 7465 5f73 6574 7469 6e67 732e 6d61  rite_settings.ma
-0000fa70: 785f 706f 696e 7473 0a20 2020 2020 2020  x_points.       
-0000fa80: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-0000fa90: 6620 6c6f 6767 696e 673a 0a20 2020 2020  f logging:.     
-0000faa0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-0000fab0: 666f 2866 2257 726f 7465 2074 6f20 7b73  fo(f"Wrote to {s
-0000fac0: 7472 2867 6473 7061 7468 2921 727d 2229  tr(gdspath)!r}")
-0000fad0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000fae0: 6764 7370 6174 680a 0a20 2020 2064 6566  gdspath..    def
-0000faf0: 2077 7269 7465 5f67 6473 280a 2020 2020   write_gds(.    
-0000fb00: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000fb10: 2020 6764 7370 6174 683a 204f 7074 696f    gdspath: Optio
-0000fb20: 6e61 6c5b 5061 7468 5479 7065 5d20 3d20  nal[PathType] = 
-0000fb30: 4e6f 6e65 2c0a 2020 2020 2020 2020 6764  None,.        gd
-0000fb40: 7364 6972 3a20 4f70 7469 6f6e 616c 5b50  sdir: Optional[P
-0000fb50: 6174 6854 7970 655d 203d 204e 6f6e 652c  athType] = None,
-0000fb60: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
-0000fb70: 732c 0a20 2020 2029 202d 3e20 5061 7468  s,.    ) -> Path
-0000fb80: 3a0a 2020 2020 2020 2020 2222 2257 7269  :.        """Wri
-0000fb90: 7465 2063 6f6d 706f 6e65 6e74 2074 6f20  te component to 
-0000fba0: 4744 5320 616e 6420 7265 7475 726e 7320  GDS and returns 
-0000fbb0: 6764 7370 6174 682e 0a0a 2020 2020 2020  gdspath...      
-0000fbc0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000fbd0: 2020 2020 6764 7370 6174 683a 2047 4453      gdspath: GDS
-0000fbe0: 2066 696c 6520 7061 7468 2074 6f20 7772   file path to wr
-0000fbf0: 6974 6520 746f 2e0a 2020 2020 2020 2020  ite to..        
-0000fc00: 2020 2020 6764 7364 6972 3a20 6469 7265      gdsdir: dire
-0000fc10: 6374 6f72 7920 666f 7220 7468 6520 4744  ctory for the GD
-0000fc20: 5320 6669 6c65 2e20 4465 6661 756c 7473  S file. Defaults
-0000fc30: 2074 6f20 2f74 6d70 2f72 616e 646f 6d46   to /tmp/randomF
-0000fc40: 696c 652f 6764 7366 6163 746f 7279 2e0a  ile/gdsfactory..
-0000fc50: 0a20 2020 2020 2020 204b 6579 776f 7264  .        Keyword
-0000fc60: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0000fc70: 2020 2075 6e69 743a 2075 6e69 7420 7369     unit: unit si
-0000fc80: 7a65 2066 6f72 206f 626a 6563 7473 2069  ze for objects i
-0000fc90: 6e20 6c69 6272 6172 792e 2031 756d 2062  n library. 1um b
-0000fca0: 7920 6465 6661 756c 742e 0a20 2020 2020  y default..     
-0000fcb0: 2020 2020 2020 2070 7265 6369 7369 6f6e         precision
-0000fcc0: 3a20 666f 7220 6469 6d65 6e73 696f 6e73  : for dimensions
-0000fcd0: 2069 6e20 7468 6520 6c69 6272 6172 7920   in the library 
-0000fce0: 286d 292e 2031 6e6d 2062 7920 6465 6661  (m). 1nm by defa
-0000fcf0: 756c 742e 0a20 2020 2020 2020 2020 2020  ult..           
-0000fd00: 206c 6f67 6769 6e67 3a20 6469 7361 626c   logging: disabl
-0000fd10: 6520 4744 5320 7061 7468 206c 6f67 6769  e GDS path loggi
-0000fd20: 6e67 2c20 666f 7220 6578 616d 706c 6520  ng, for example 
-0000fd30: 666f 7220 7368 6f77 696e 6720 6974 2069  for showing it i
-0000fd40: 6e20 4b4c 6179 6f75 742e 0a20 2020 2020  n KLayout..     
-0000fd50: 2020 2020 2020 206f 6e5f 6475 706c 6963         on_duplic
-0000fd60: 6174 655f 6365 6c6c 3a20 7370 6563 6966  ate_cell: specif
-0000fd70: 7920 686f 7720 746f 2072 6573 6f6c 7665  y how to resolve
-0000fd80: 2064 7570 6c69 6361 7465 2d6e 616d 6564   duplicate-named
-0000fd90: 2063 656c 6c73 2e20 4368 6f6f 7365 206f   cells. Choose o
-0000fda0: 6e65 206f 6620 7468 6520 666f 6c6c 6f77  ne of the follow
-0000fdb0: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-0000fdc0: 2020 2020 2022 7761 726e 2220 2864 6566       "warn" (def
-0000fdd0: 6175 6c74 293a 206f 7665 7277 7269 7465  ault): overwrite
-0000fde0: 2061 6c6c 2064 7570 6c69 6361 7465 2063   all duplicate c
-0000fdf0: 656c 6c73 2077 6974 6820 6f6e 6520 6f66  ells with one of
-0000fe00: 2074 6865 2064 7570 6c69 6361 7465 7320   the duplicates 
-0000fe10: 2861 7262 6974 7261 7269 6c79 292e 0a20  (arbitrarily).. 
-0000fe20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000fe30: 6572 726f 7222 3a20 7468 726f 7720 6120  error": throw a 
-0000fe40: 5661 6c75 6545 7272 6f72 2077 6865 6e20  ValueError when 
-0000fe50: 6174 7465 6d70 7469 6e67 2074 6f20 7772  attempting to wr
-0000fe60: 6974 6520 6120 6764 7320 7769 7468 2064  ite a gds with d
-0000fe70: 7570 6c69 6361 7465 2063 656c 6c73 2e0a  uplicate cells..
-0000fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe90: 226f 7665 7277 7269 7465 223a 206f 7665  "overwrite": ove
-0000fea0: 7277 7269 7465 2061 6c6c 2064 7570 6c69  rwrite all dupli
-0000feb0: 6361 7465 2063 656c 6c73 2077 6974 6820  cate cells with 
-0000fec0: 6f6e 6520 6f66 2074 6865 2064 7570 6c69  one of the dupli
-0000fed0: 6361 7465 732c 2077 6974 686f 7574 2077  cates, without w
-0000fee0: 6172 6e69 6e67 2e0a 2020 2020 2020 2020  arning..        
-0000fef0: 2020 2020 6f6e 5f75 6e63 6163 6865 645f      on_uncached_
-0000ff00: 636f 6d70 6f6e 656e 743a 204c 6974 6572  component: Liter
-0000ff10: 616c 5b22 7761 726e 222c 2022 6572 726f  al["warn", "erro
-0000ff20: 7222 5d20 3d20 2277 6172 6e22 0a20 2020  r"] = "warn".   
-0000ff30: 2020 2020 2020 2020 2066 6c61 7474 656e           flatten
-0000ff40: 5f69 6e76 616c 6964 5f72 6566 733a 2066  _invalid_refs: f
-0000ff50: 6c61 7474 656e 7320 636f 6d70 6f6e 656e  lattens componen
-0000ff60: 7420 7265 6665 7265 6e63 6573 2077 6869  t references whi
-0000ff70: 6368 2068 6176 6520 696e 7661 6c69 6420  ch have invalid 
-0000ff80: 7472 616e 7366 6f72 6d61 7469 6f6e 732e  transformations.
-0000ff90: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-0000ffa0: 5f70 6f69 6e74 733a 204d 6178 696d 616c  _points: Maximal
-0000ffb0: 206e 756d 6265 7220 6f66 2076 6572 7469   number of verti
-0000ffc0: 6365 7320 7065 7220 706f 6c79 676f 6e2e  ces per polygon.
-0000ffd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ffe0: 2050 6f6c 7967 6f6e 7320 7769 7468 206d   Polygons with m
-0000fff0: 6f72 6520 7665 7274 6963 6573 2074 6861  ore vertices tha
-00010000: 7420 7468 6973 2061 7265 2061 7574 6f6d  t this are autom
-00010010: 6174 6963 616c 6c79 2066 7261 6374 7572  atically fractur
-00010020: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
-00010030: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010040: 7365 6c66 2e5f 7772 6974 655f 6c69 6272  self._write_libr
-00010050: 6172 7928 0a20 2020 2020 2020 2020 2020  ary(.           
-00010060: 2067 6473 7061 7468 3d67 6473 7061 7468   gdspath=gdspath
-00010070: 2c20 6764 7364 6972 3d67 6473 6469 722c  , gdsdir=gdsdir,
-00010080: 2077 6974 685f 6f61 7369 733d 4661 6c73   with_oasis=Fals
-00010090: 652c 202a 2a6b 7761 7267 730a 2020 2020  e, **kwargs.    
-000100a0: 2020 2020 290a 0a20 2020 2064 6566 2077      )..    def w
-000100b0: 7269 7465 5f6f 6173 280a 2020 2020 2020  rite_oas(.      
-000100c0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000100d0: 6764 7370 6174 683a 204f 7074 696f 6e61  gdspath: Optiona
-000100e0: 6c5b 5061 7468 5479 7065 5d20 3d20 4e6f  l[PathType] = No
-000100f0: 6e65 2c0a 2020 2020 2020 2020 6764 7364  ne,.        gdsd
-00010100: 6972 3a20 4f70 7469 6f6e 616c 5b50 6174  ir: Optional[Pat
-00010110: 6854 7970 655d 203d 204e 6f6e 652c 0a20  hType] = None,. 
-00010120: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
-00010130: 0a20 2020 2029 202d 3e20 5061 7468 3a0a  .    ) -> Path:.
-00010140: 2020 2020 2020 2020 2222 2257 7269 7465          """Write
-00010150: 2063 6f6d 706f 6e65 6e74 2074 6f20 4744   component to GD
-00010160: 5320 616e 6420 7265 7475 726e 7320 6764  S and returns gd
-00010170: 7370 6174 682e 0a0a 2020 2020 2020 2020  spath...        
-00010180: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00010190: 2020 6764 7370 6174 683a 2047 4453 2066    gdspath: GDS f
-000101a0: 696c 6520 7061 7468 2074 6f20 7772 6974  ile path to writ
-000101b0: 6520 746f 2e0a 2020 2020 2020 2020 2020  e to..          
-000101c0: 2020 6764 7364 6972 3a20 6469 7265 6374    gdsdir: direct
-000101d0: 6f72 7920 666f 7220 7468 6520 4744 5320  ory for the GDS 
-000101e0: 6669 6c65 2e20 4465 6661 756c 7473 2074  file. Defaults t
-000101f0: 6f20 2f74 6d70 2f72 616e 646f 6d46 696c  o /tmp/randomFil
-00010200: 652f 6764 7366 6163 746f 7279 2e0a 0a20  e/gdsfactory... 
-00010210: 2020 2020 2020 204b 6579 776f 7264 2041         Keyword A
-00010220: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00010230: 2075 6e69 743a 2075 6e69 7420 7369 7a65   unit: unit size
-00010240: 2066 6f72 206f 626a 6563 7473 2069 6e20   for objects in 
-00010250: 6c69 6272 6172 792e 2031 756d 2062 7920  library. 1um by 
-00010260: 6465 6661 756c 742e 0a20 2020 2020 2020  default..       
-00010270: 2020 2020 2070 7265 6369 7369 6f6e 3a20       precision: 
-00010280: 666f 7220 6469 6d65 6e73 696f 6e73 2069  for dimensions i
-00010290: 6e20 7468 6520 6c69 6272 6172 7920 286d  n the library (m
-000102a0: 292e 2031 6e6d 2062 7920 6465 6661 756c  ). 1nm by defaul
-000102b0: 742e 0a20 2020 2020 2020 2020 2020 206c  t..            l
-000102c0: 6f67 6769 6e67 3a20 6469 7361 626c 6520  ogging: disable 
-000102d0: 4744 5320 7061 7468 206c 6f67 6769 6e67  GDS path logging
-000102e0: 2c20 666f 7220 6578 616d 706c 6520 666f  , for example fo
-000102f0: 7220 7368 6f77 696e 6720 6974 2069 6e20  r showing it in 
-00010300: 4b4c 6179 6f75 742e 0a20 2020 2020 2020  KLayout..       
-00010310: 2020 2020 206f 6e5f 6475 706c 6963 6174       on_duplicat
-00010320: 655f 6365 6c6c 3a20 7370 6563 6966 7920  e_cell: specify 
-00010330: 686f 7720 746f 2072 6573 6f6c 7665 2064  how to resolve d
-00010340: 7570 6c69 6361 7465 2d6e 616d 6564 2063  uplicate-named c
-00010350: 656c 6c73 2e20 4368 6f6f 7365 206f 6e65  ells. Choose one
-00010360: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-00010370: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-00010380: 2020 2022 7761 726e 2220 2864 6566 6175     "warn" (defau
-00010390: 6c74 293a 206f 7665 7277 7269 7465 2061  lt): overwrite a
-000103a0: 6c6c 2064 7570 6c69 6361 7465 2063 656c  ll duplicate cel
-000103b0: 6c73 2077 6974 6820 6f6e 6520 6f66 2074  ls with one of t
-000103c0: 6865 2064 7570 6c69 6361 7465 7320 2861  he duplicates (a
-000103d0: 7262 6974 7261 7269 6c79 292e 0a20 2020  rbitrarily)..   
-000103e0: 2020 2020 2020 2020 2020 2020 2022 6572               "er
-000103f0: 726f 7222 3a20 7468 726f 7720 6120 5661  ror": throw a Va
-00010400: 6c75 6545 7272 6f72 2077 6865 6e20 6174  lueError when at
-00010410: 7465 6d70 7469 6e67 2074 6f20 7772 6974  tempting to writ
-00010420: 6520 6120 6764 7320 7769 7468 2064 7570  e a gds with dup
-00010430: 6c69 6361 7465 2063 656c 6c73 2e0a 2020  licate cells..  
-00010440: 2020 2020 2020 2020 2020 2020 2020 226f                "o
-00010450: 7665 7277 7269 7465 223a 206f 7665 7277  verwrite": overw
-00010460: 7269 7465 2061 6c6c 2064 7570 6c69 6361  rite all duplica
-00010470: 7465 2063 656c 6c73 2077 6974 6820 6f6e  te cells with on
-00010480: 6520 6f66 2074 6865 2064 7570 6c69 6361  e of the duplica
-00010490: 7465 732c 2077 6974 686f 7574 2077 6172  tes, without war
-000104a0: 6e69 6e67 2e0a 2020 2020 2020 2020 2020  ning..          
-000104b0: 2020 2020 2020 4e6f 6e65 3a20 646f 206e        None: do n
-000104c0: 6f74 2074 7279 2074 6f20 7265 736f 6c76  ot try to resolv
-000104d0: 6520 2861 7420 796f 7572 206f 776e 2072  e (at your own r
-000104e0: 6973 6b21 290a 2020 2020 2020 2020 2020  isk!).          
-000104f0: 2020 6f6e 5f75 6e63 6163 6865 645f 636f    on_uncached_co
-00010500: 6d70 6f6e 656e 743a 204c 6974 6572 616c  mponent: Literal
-00010510: 5b22 7761 726e 222c 2022 6572 726f 7222  ["warn", "error"
-00010520: 5d20 3d20 2277 6172 6e22 0a20 2020 2020  ] = "warn".     
-00010530: 2020 2020 2020 2066 6c61 7474 656e 5f69         flatten_i
-00010540: 6e76 616c 6964 5f72 6566 733a 2066 6c61  nvalid_refs: fla
-00010550: 7474 656e 7320 636f 6d70 6f6e 656e 7420  ttens component 
-00010560: 7265 6665 7265 6e63 6573 2077 6869 6368  references which
-00010570: 2068 6176 6520 696e 7661 6c69 6420 7472   have invalid tr
-00010580: 616e 7366 6f72 6d61 7469 6f6e 732e 0a20  ansformations.. 
-00010590: 2020 2020 2020 2020 2020 2063 6f6d 7072             compr
-000105a0: 6573 7369 6f6e 5f6c 6576 656c 3a20 4c65  ession_level: Le
-000105b0: 7665 6c20 6f66 2063 6f6d 7072 6573 7369  vel of compressi
-000105c0: 6f6e 2066 6f72 2063 656c 6c73 2028 6265  on for cells (be
-000105d0: 7477 6565 6e20 3020 616e 6420 3929 2e0a  tween 0 and 9)..
-000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105f0: 5365 7474 696e 6720 746f 2030 2077 696c  Setting to 0 wil
-00010600: 6c20 6469 7361 626c 6520 6365 6c6c 2063  l disable cell c
-00010610: 6f6d 7072 6573 7369 6f6e 2c20 3120 6769  ompression, 1 gi
-00010620: 7665 7320 7468 6520 6265 7374 2073 7065  ves the best spe
-00010630: 6564 2061 6e64 2039 2c20 7468 6520 6265  ed and 9, the be
-00010640: 7374 2063 6f6d 7072 6573 7369 6f6e 2e0a  st compression..
-00010650: 2020 2020 2020 2020 2020 2020 6465 7465              dete
-00010660: 6374 5f72 6563 7461 6e67 6c65 733a 2053  ct_rectangles: S
-00010670: 746f 7265 2072 6563 7461 6e67 6c65 7320  tore rectangles 
-00010680: 696e 2063 6f6d 7072 6573 7365 6420 666f  in compressed fo
-00010690: 726d 6174 2e0a 2020 2020 2020 2020 2020  rmat..          
-000106a0: 2020 6465 7465 6374 5f74 7261 7065 7a6f    detect_trapezo
-000106b0: 6964 733a 2053 746f 7265 2074 7261 7065  ids: Store trape
-000106c0: 7a6f 6964 7320 696e 2063 6f6d 7072 6573  zoids in compres
-000106d0: 7365 6420 666f 726d 6174 2e0a 2020 2020  sed format..    
-000106e0: 2020 2020 2020 2020 6369 7263 6c65 5f74          circle_t
-000106f0: 6f6c 6572 616e 6365 3a20 546f 6c65 7261  olerance: Tolera
-00010700: 6e63 6520 666f 7220 6465 7465 6374 696e  nce for detectin
-00010710: 6720 6369 7263 6c65 732e 2049 6620 6c65  g circles. If le
-00010720: 7373 206f 7220 6571 7561 6c20 746f 2030  ss or equal to 0
-00010730: 2c20 6e6f 2064 6574 6563 7469 6f6e 2069  , no detection i
-00010740: 7320 7065 7266 6f72 6d65 642e 0a20 2020  s performed..   
-00010750: 2020 2020 2020 2020 2020 2020 2043 6972               Cir
-00010760: 636c 6573 2061 7265 2073 746f 7265 6420  cles are stored 
-00010770: 696e 2063 6f6d 7072 6573 7365 6420 666f  in compressed fo
-00010780: 726d 6174 2e0a 2020 2020 2020 2020 2020  rmat..          
-00010790: 2020 7661 6c69 6461 7469 6f6e 2028 2263    validation ("c
-000107a0: 7263 3332 222c 2022 6368 6563 6b73 756d  rc32", "checksum
-000107b0: 3332 222c 204e 6f6e 6529 20e2 8093 2074  32", None) ... t
-000107c0: 7970 6520 6f66 2076 616c 6964 6174 696f  ype of validatio
-000107d0: 6e20 746f 2069 6e63 6c75 6465 2069 6e20  n to include in 
-000107e0: 7468 6520 7361 7665 6420 6669 6c65 2e0a  the saved file..
-000107f0: 2020 2020 2020 2020 2020 2020 7374 616e              stan
-00010800: 6461 7264 5f70 726f 7065 7274 6965 733a  dard_properties:
-00010810: 2053 746f 7265 2073 7461 6e64 6172 6420   Store standard 
-00010820: 4f41 5349 5320 7072 6f70 6572 7469 6573  OASIS properties
-00010830: 2069 6e20 7468 6520 6669 6c65 2e0a 2020   in the file..  
-00010840: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010850: 2020 7265 7475 726e 2073 656c 662e 5f77    return self._w
-00010860: 7269 7465 5f6c 6962 7261 7279 280a 2020  rite_library(.  
-00010870: 2020 2020 2020 2020 2020 6764 7370 6174            gdspat
-00010880: 683d 6764 7370 6174 682c 0a20 2020 2020  h=gdspath,.     
-00010890: 2020 2020 2020 2067 6473 6469 723d 6764         gdsdir=gd
-000108a0: 7364 6972 2c0a 2020 2020 2020 2020 2020  sdir,.          
-000108b0: 2020 7769 7468 5f6f 6173 6973 3d54 7275    with_oasis=Tru
-000108c0: 652c 0a20 2020 2020 2020 2020 2020 202a  e,.            *
-000108d0: 2a6b 7761 7267 732c 0a20 2020 2020 2020  *kwargs,.       
-000108e0: 2029 0a0a 2020 2020 6465 6620 7772 6974   )..    def writ
-000108f0: 655f 6764 735f 7769 7468 5f6d 6574 6164  e_gds_with_metad
-00010900: 6174 6128 7365 6c66 2c20 2a61 7267 732c  ata(self, *args,
-00010910: 202a 2a6b 7761 7267 7329 202d 3e20 5061   **kwargs) -> Pa
-00010920: 7468 3a0a 2020 2020 2020 2020 2222 2257  th:.        """W
-00010930: 7269 7465 2063 6f6d 706f 6e65 6e74 2069  rite component i
-00010940: 6e20 4744 5320 616e 6420 6d65 7461 6461  n GDS and metada
-00010950: 7461 2028 636f 6d70 6f6e 656e 7420 7365  ta (component se
-00010960: 7474 696e 6773 2920 696e 2059 414d 4c2e  ttings) in YAML.
-00010970: 2222 220a 2020 2020 2020 2020 6764 7370  """.        gdsp
-00010980: 6174 6820 3d20 7365 6c66 2e77 7269 7465  ath = self.write
-00010990: 5f67 6473 282a 6172 6773 2c20 2a2a 6b77  _gds(*args, **kw
-000109a0: 6172 6773 290a 2020 2020 2020 2020 6d65  args).        me
-000109b0: 7461 6461 7461 203d 2067 6473 7061 7468  tadata = gdspath
-000109c0: 2e77 6974 685f 7375 6666 6978 2822 2e79  .with_suffix(".y
-000109d0: 6d6c 2229 0a20 2020 2020 2020 206d 6574  ml").        met
-000109e0: 6164 6174 612e 7772 6974 655f 7465 7874  adata.write_text
-000109f0: 2873 656c 662e 746f 5f79 616d 6c28 7769  (self.to_yaml(wi
-00010a00: 7468 5f63 656c 6c73 3d54 7275 652c 2077  th_cells=True, w
-00010a10: 6974 685f 706f 7274 733d 5472 7565 2929  ith_ports=True))
-00010a20: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00010a30: 696e 666f 2866 2257 7269 7465 2059 414d  info(f"Write YAM
-00010a40: 4c20 6d65 7461 6461 7461 2074 6f20 7b73  L metadata to {s
-00010a50: 7472 286d 6574 6164 6174 6129 2172 7d22  tr(metadata)!r}"
-00010a60: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00010a70: 2067 6473 7061 7468 0a0a 2020 2020 6465   gdspath..    de
-00010a80: 6620 746f 5f64 6963 7428 0a20 2020 2020  f to_dict(.     
-00010a90: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00010aa0: 2069 676e 6f72 655f 636f 6d70 6f6e 656e   ignore_componen
-00010ab0: 7473 5f70 7265 6669 783a 204f 7074 696f  ts_prefix: Optio
-00010ac0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 203d  nal[List[str]] =
-00010ad0: 204e 6f6e 652c 0a20 2020 2020 2020 2069   None,.        i
-00010ae0: 676e 6f72 655f 6675 6e63 7469 6f6e 735f  gnore_functions_
-00010af0: 7072 6566 6978 3a20 4f70 7469 6f6e 616c  prefix: Optional
-00010b00: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
-00010b10: 6e65 2c0a 2020 2020 2020 2020 7769 7468  ne,.        with
-00010b20: 5f63 656c 6c73 3a20 626f 6f6c 203d 2046  _cells: bool = F
-00010b30: 616c 7365 2c0a 2020 2020 2020 2020 7769  alse,.        wi
-00010b40: 7468 5f70 6f72 7473 3a20 626f 6f6c 203d  th_ports: bool =
-00010b50: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
-00010b60: 4469 6374 5b73 7472 2c20 416e 795d 3a0a  Dict[str, Any]:.
-00010b70: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00010b80: 6e73 2044 6963 7420 7265 7072 6573 656e  ns Dict represen
-00010b90: 7461 7469 6f6e 206f 6620 6120 636f 6d70  tation of a comp
-00010ba0: 6f6e 656e 742e 0a0a 2020 2020 2020 2020  onent...        
-00010bb0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00010bc0: 2020 6967 6e6f 7265 5f63 6f6d 706f 6e65    ignore_compone
-00010bd0: 6e74 735f 7072 6566 6978 3a20 666f 7220  nts_prefix: for 
-00010be0: 636f 6d70 6f6e 656e 7473 2074 6f20 6967  components to ig
-00010bf0: 6e6f 7265 2077 6865 6e20 6578 706f 7274  nore when export
-00010c00: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
-00010c10: 2069 676e 6f72 655f 6675 6e63 7469 6f6e   ignore_function
-00010c20: 735f 7072 6566 6978 3a20 666f 7220 6675  s_prefix: for fu
-00010c30: 6e63 7469 6f6e 7320 746f 2069 676e 6f72  nctions to ignor
-00010c40: 6520 7768 656e 2065 7870 6f72 7469 6e67  e when exporting
-00010c50: 2e0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00010c60: 7468 5f63 656c 6c73 3a20 7772 6974 6520  th_cells: write 
-00010c70: 6365 6c6c 7320 7265 6375 7273 6976 656c  cells recursivel
-00010c80: 792e 0a20 2020 2020 2020 2020 2020 2077  y..            w
-00010c90: 6974 685f 706f 7274 733a 2077 7269 7465  ith_ports: write
-00010ca0: 2070 6f72 7420 696e 666f 726d 6174 696f   port informatio
-00010cb0: 6e20 6469 6374 2e0a 2020 2020 2020 2020  n dict..        
-00010cc0: 2222 220a 2020 2020 2020 2020 6420 3d20  """.        d = 
-00010cd0: 7b7d 0a20 2020 2020 2020 2069 6620 7769  {}.        if wi
-00010ce0: 7468 5f70 6f72 7473 3a0a 2020 2020 2020  th_ports:.      
-00010cf0: 2020 2020 2020 706f 7274 7320 3d20 7b70        ports = {p
-00010d00: 6f72 742e 6e61 6d65 3a20 706f 7274 2e74  ort.name: port.t
-00010d10: 6f5f 6469 6374 2829 2066 6f72 2070 6f72  o_dict() for por
-00010d20: 7420 696e 2073 656c 662e 6765 745f 706f  t in self.get_po
-00010d30: 7274 735f 6c69 7374 2829 7d0a 2020 2020  rts_list()}.    
-00010d40: 2020 2020 2020 2020 645b 2270 6f72 7473          d["ports
-00010d50: 225d 203d 2070 6f72 7473 0a0a 2020 2020  "] = ports..    
-00010d60: 2020 2020 6966 2077 6974 685f 6365 6c6c      if with_cell
-00010d70: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-00010d80: 656c 6c73 203d 2072 6563 7572 7365 5f73  ells = recurse_s
-00010d90: 7472 7563 7475 7265 7328 0a20 2020 2020  tructures(.     
-00010da0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00010db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010dc0: 2069 676e 6f72 655f 6675 6e63 7469 6f6e   ignore_function
-00010dd0: 735f 7072 6566 6978 3d69 676e 6f72 655f  s_prefix=ignore_
-00010de0: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
-00010df0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010e00: 2020 6967 6e6f 7265 5f63 6f6d 706f 6e65    ignore_compone
-00010e10: 6e74 735f 7072 6566 6978 3d69 676e 6f72  nts_prefix=ignor
-00010e20: 655f 636f 6d70 6f6e 656e 7473 5f70 7265  e_components_pre
-00010e30: 6669 782c 0a20 2020 2020 2020 2020 2020  fix,.           
-00010e40: 2029 0a20 2020 2020 2020 2020 2020 2064   ).            d
-00010e50: 5b22 6365 6c6c 7322 5d20 3d20 636c 6561  ["cells"] = clea
-00010e60: 6e5f 6469 6374 2863 656c 6c73 290a 0a20  n_dict(cells).. 
-00010e70: 2020 2020 2020 2064 5b22 6e61 6d65 225d         d["name"]
-00010e80: 203d 2073 656c 662e 6e61 6d65 0a20 2020   = self.name.   
-00010e90: 2020 2020 2064 5b22 7365 7474 696e 6773       d["settings
-00010ea0: 225d 203d 2063 6c65 616e 5f64 6963 7428  "] = clean_dict(
-00010eb0: 6469 6374 2873 656c 662e 7365 7474 696e  dict(self.settin
-00010ec0: 6773 2929 0a20 2020 2020 2020 2072 6574  gs)).        ret
-00010ed0: 7572 6e20 640a 0a20 2020 2064 6566 2074  urn d..    def t
-00010ee0: 6f5f 7961 6d6c 2873 656c 662c 202a 2a6b  o_yaml(self, **k
-00010ef0: 7761 7267 7329 202d 3e20 7374 723a 0a20  wargs) -> str:. 
-00010f00: 2020 2020 2020 2022 2222 5772 6974 6520         """Write 
-00010f10: 4469 6374 2072 6570 7265 7365 6e74 6174  Dict representat
-00010f20: 696f 6e20 6f66 2061 2063 6f6d 706f 6e65  ion of a compone
-00010f30: 6e74 2069 6e20 5941 4d4c 2066 6f72 6d61  nt in YAML forma
-00010f40: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
-00010f50: 3a0a 2020 2020 2020 2020 2020 2020 6967  :.            ig
-00010f60: 6e6f 7265 5f63 6f6d 706f 6e65 6e74 735f  nore_components_
-00010f70: 7072 6566 6978 3a20 666f 7220 636f 6d70  prefix: for comp
-00010f80: 6f6e 656e 7473 2074 6f20 6967 6e6f 7265  onents to ignore
-00010f90: 2077 6865 6e20 6578 706f 7274 696e 672e   when exporting.
-00010fa0: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
-00010fb0: 6f72 655f 6675 6e63 7469 6f6e 735f 7072  ore_functions_pr
-00010fc0: 6566 6978 3a20 666f 7220 6675 6e63 7469  efix: for functi
-00010fd0: 6f6e 7320 746f 2069 676e 6f72 6520 7768  ons to ignore wh
-00010fe0: 656e 2065 7870 6f72 7469 6e67 2e0a 2020  en exporting..  
-00010ff0: 2020 2020 2020 2020 2020 7769 7468 5f63            with_c
-00011000: 656c 6c73 3a20 7772 6974 6520 6365 6c6c  ells: write cell
-00011010: 7320 7265 6375 7273 6976 656c 792e 0a20  s recursively.. 
-00011020: 2020 2020 2020 2020 2020 2077 6974 685f             with_
-00011030: 706f 7274 733a 2077 7269 7465 2070 6f72  ports: write por
-00011040: 7420 696e 666f 726d 6174 696f 6e2e 0a20  t information.. 
-00011050: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011060: 2020 2072 6574 7572 6e20 4f6d 6567 6143     return OmegaC
-00011070: 6f6e 662e 746f 5f79 616d 6c28 636c 6561  onf.to_yaml(clea
-00011080: 6e5f 6469 6374 2873 656c 662e 746f 5f64  n_dict(self.to_d
-00011090: 6963 7428 2a2a 6b77 6172 6773 2929 290a  ict(**kwargs))).
-000110a0: 0a20 2020 2064 6566 2074 6f5f 6469 6374  .    def to_dict
-000110b0: 5f70 6f6c 7967 6f6e 7328 7365 6c66 2920  _polygons(self) 
-000110c0: 2d3e 2044 6963 745b 7374 722c 2041 6e79  -> Dict[str, Any
-000110d0: 5d3a 0a20 2020 2020 2020 2022 2222 5265  ]:.        """Re
-000110e0: 7475 726e 7320 6120 6469 6374 2072 6570  turns a dict rep
-000110f0: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
-00011100: 6865 2066 6c61 7474 656e 6564 2063 6f6d  he flattened com
-00011110: 706f 6e65 6e74 2e22 2222 0a20 2020 2020  ponent.""".     
-00011120: 2020 2064 203d 207b 7d0a 2020 2020 2020     d = {}.      
-00011130: 2020 706f 6c79 676f 6e73 203d 207b 7d0a    polygons = {}.
-00011140: 2020 2020 2020 2020 6c61 7965 725f 746f          layer_to
-00011150: 5f70 6f6c 7967 6f6e 7320 3d20 7365 6c66  _polygons = self
-00011160: 2e67 6574 5f70 6f6c 7967 6f6e 7328 6279  .get_polygons(by
-00011170: 5f73 7065 633d 5472 7565 290a 0a20 2020  _spec=True)..   
-00011180: 2020 2020 2066 6f72 206c 6179 6572 2c20       for layer, 
-00011190: 706f 6c79 676f 6e73 5f6c 6179 6572 2069  polygons_layer i
-000111a0: 6e20 6c61 7965 725f 746f 5f70 6f6c 7967  n layer_to_polyg
-000111b0: 6f6e 732e 6974 656d 7328 293a 0a20 2020  ons.items():.   
-000111c0: 2020 2020 2020 2020 206c 6179 6572 5f6e           layer_n
-000111d0: 616d 6520 3d20 6622 7b6c 6179 6572 5b30  ame = f"{layer[0
-000111e0: 5d7d 5f7b 6c61 7965 725b 315d 7d22 0a20  ]}_{layer[1]}". 
-000111f0: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
-00011200: 6f6c 7967 6f6e 2069 6e20 706f 6c79 676f  olygon in polygo
-00011210: 6e73 5f6c 6179 6572 3a0a 2020 2020 2020  ns_layer:.      
-00011220: 2020 2020 2020 2020 2020 706f 6c79 676f            polygo
-00011230: 6e73 5b6c 6179 6572 5f6e 616d 655d 203d  ns[layer_name] =
-00011240: 205b 7475 706c 6528 736e 6170 5f74 6f5f   [tuple(snap_to_
-00011250: 6772 6964 2876 2929 2066 6f72 2076 2069  grid(v)) for v i
-00011260: 6e20 706f 6c79 676f 6e5d 0a0a 2020 2020  n polygon]..    
-00011270: 2020 2020 706f 7274 7320 3d20 7b70 6f72      ports = {por
-00011280: 742e 6e61 6d65 3a20 706f 7274 2e73 6574  t.name: port.set
-00011290: 7469 6e67 7320 666f 7220 706f 7274 2069  tings for port i
-000112a0: 6e20 7365 6c66 2e67 6574 5f70 6f72 7473  n self.get_ports
-000112b0: 5f6c 6973 7428 297d 0a20 2020 2020 2020  _list()}.       
-000112c0: 2063 6c65 616e 5f64 6963 7428 706f 7274   clean_dict(port
-000112d0: 7329 0a20 2020 2020 2020 2063 6c65 616e  s).        clean
-000112e0: 5f64 6963 7428 706f 6c79 676f 6e73 290a  _dict(polygons).
-000112f0: 2020 2020 2020 2020 642e 696e 666f 203d          d.info =
-00011300: 2073 656c 662e 696e 666f 0a20 2020 2020   self.info.     
-00011310: 2020 2064 2e70 6f6c 7967 6f6e 7320 3d20     d.polygons = 
-00011320: 706f 6c79 676f 6e73 0a20 2020 2020 2020  polygons.       
-00011330: 2064 2e70 6f72 7473 203d 2070 6f72 7473   d.ports = ports
-00011340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011350: 640a 0a20 2020 2064 6566 2061 7574 6f5f  d..    def auto_
-00011360: 7265 6e61 6d65 5f70 6f72 7473 2873 656c  rename_ports(sel
-00011370: 662c 202a 2a6b 7761 7267 7329 202d 3e20  f, **kwargs) -> 
-00011380: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00011390: 2252 656e 616d 6520 706f 7274 7320 6279  "Rename ports by
-000113a0: 206f 7269 656e 7461 7469 6f6e 204e 5345   orientation NSE
-000113b0: 5720 286e 6f72 7468 2c20 736f 7574 682c  W (north, south,
-000113c0: 2065 6173 742c 2077 6573 7429 2e0a 0a20   east, west)... 
-000113d0: 2020 2020 2020 204b 6579 776f 7264 2041         Keyword A
-000113e0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-000113f0: 2066 756e 6374 696f 6e3a 2074 6f20 7265   function: to re
-00011400: 6e61 6d65 2070 6f72 7473 2e0a 2020 2020  name ports..    
-00011410: 2020 2020 2020 2020 7365 6c65 6374 5f70          select_p
-00011420: 6f72 7473 5f6f 7074 6963 616c 3a20 746f  orts_optical: to
-00011430: 2073 656c 6563 7420 6f70 7469 6361 6c20   select optical 
-00011440: 706f 7274 732e 0a20 2020 2020 2020 2020  ports..         
-00011450: 2020 2073 656c 6563 745f 706f 7274 735f     select_ports_
-00011460: 656c 6563 7472 6963 616c 3a20 746f 2073  electrical: to s
-00011470: 656c 6563 7420 656c 6563 7472 6963 616c  elect electrical
-00011480: 2070 6f72 7473 2e0a 2020 2020 2020 2020   ports..        
-00011490: 2020 2020 7072 6566 6978 5f6f 7074 6963      prefix_optic
-000114a0: 616c 3a20 7072 6566 6978 2e0a 2020 2020  al: prefix..    
-000114b0: 2020 2020 2020 2020 7072 6566 6978 5f65          prefix_e
-000114c0: 6c65 6374 7269 6361 6c3a 2070 7265 6669  lectrical: prefi
-000114d0: 782e 0a0a 2020 2020 2020 2020 2e2e 2063  x...        .. c
-000114e0: 6f64 653a 3a0a 0a20 2020 2020 2020 2020  ode::..         
-000114f0: 2020 2020 2020 2020 2033 2020 340a 2020           3  4.  
-00011500: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-00011510: 7c5f 5f7c 5f0a 2020 2020 2020 2020 2020  |__|_.          
-00011520: 2020 2032 202d 7c20 2020 2020 207c 2d20     2 -|      |- 
-00011530: 350a 2020 2020 2020 2020 2020 2020 2020  5.              
-00011540: 2020 7c20 2020 2020 207c 0a20 2020 2020    |      |.     
-00011550: 2020 2020 2020 2020 3120 2d7c 5f5f 5f5f          1 -|____
-00011560: 5f5f 7c2d 2036 0a20 2020 2020 2020 2020  __|- 6.         
-00011570: 2020 2020 2020 2020 207c 2020 7c0a 2020           |  |.  
-00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011590: 3820 2037 0a20 2020 2020 2020 2022 2222  8  7.        """
-000115a0: 0a20 2020 2020 2020 2073 656c 662e 6973  .        self.is
-000115b0: 5f75 6e6c 6f63 6b65 6428 290a 2020 2020  _unlocked().    
-000115c0: 2020 2020 6175 746f 5f72 656e 616d 655f      auto_rename_
-000115d0: 706f 7274 7328 7365 6c66 2c20 2a2a 6b77  ports(self, **kw
-000115e0: 6172 6773 290a 0a20 2020 2064 6566 2061  args)..    def a
-000115f0: 7574 6f5f 7265 6e61 6d65 5f70 6f72 7473  uto_rename_ports
-00011600: 5f63 6f75 6e74 6572 5f63 6c6f 636b 7769  _counter_clockwi
-00011610: 7365 2873 656c 662c 202a 2a6b 7761 7267  se(self, **kwarg
-00011620: 7329 202d 3e20 4e6f 6e65 3a0a 2020 2020  s) -> None:.    
-00011630: 2020 2020 7365 6c66 2e69 735f 756e 6c6f      self.is_unlo
-00011640: 636b 6564 2829 0a20 2020 2020 2020 2061  cked().        a
-00011650: 7574 6f5f 7265 6e61 6d65 5f70 6f72 7473  uto_rename_ports
-00011660: 5f63 6f75 6e74 6572 5f63 6c6f 636b 7769  _counter_clockwi
-00011670: 7365 2873 656c 662c 202a 2a6b 7761 7267  se(self, **kwarg
-00011680: 7329 0a0a 2020 2020 6465 6620 6175 746f  s)..    def auto
-00011690: 5f72 656e 616d 655f 706f 7274 735f 6c61  _rename_ports_la
-000116a0: 7965 725f 6f72 6965 6e74 6174 696f 6e28  yer_orientation(
-000116b0: 7365 6c66 2c20 2a2a 6b77 6172 6773 2920  self, **kwargs) 
-000116c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000116d0: 2073 656c 662e 6973 5f75 6e6c 6f63 6b65   self.is_unlocke
-000116e0: 6428 290a 2020 2020 2020 2020 6175 746f  d().        auto
-000116f0: 5f72 656e 616d 655f 706f 7274 735f 6c61  _rename_ports_la
-00011700: 7965 725f 6f72 6965 6e74 6174 696f 6e28  yer_orientation(
-00011710: 7365 6c66 2c20 2a2a 6b77 6172 6773 290a  self, **kwargs).
-00011720: 0a20 2020 2064 6566 2061 7574 6f5f 7265  .    def auto_re
-00011730: 6e61 6d65 5f70 6f72 7473 5f6f 7269 656e  name_ports_orien
-00011740: 7461 7469 6f6e 2873 656c 662c 202a 2a6b  tation(self, **k
-00011750: 7761 7267 7329 202d 3e20 4e6f 6e65 3a0a  wargs) -> None:.
-00011760: 2020 2020 2020 2020 2222 2252 656e 616d          """Renam
-00011770: 6520 706f 7274 7320 6279 206f 7269 656e  e ports by orien
-00011780: 7461 7469 6f6e 204e 5345 5720 286e 6f72  tation NSEW (nor
-00011790: 7468 2c20 736f 7574 682c 2065 6173 742c  th, south, east,
-000117a0: 2077 6573 7429 2e0a 0a20 2020 2020 2020   west)...       
-000117b0: 204b 6579 776f 7264 2041 7267 733a 0a20   Keyword Args:. 
-000117c0: 2020 2020 2020 2020 2020 2066 756e 6374             funct
-000117d0: 696f 6e3a 2074 6f20 7265 6e61 6d65 2070  ion: to rename p
-000117e0: 6f72 7473 2e0a 2020 2020 2020 2020 2020  orts..          
-000117f0: 2020 7365 6c65 6374 5f70 6f72 7473 5f6f    select_ports_o
-00011800: 7074 6963 616c 3a20 746f 2073 656c 6563  ptical: to selec
-00011810: 7420 706f 7274 732e 0a20 2020 2020 2020  t ports..       
-00011820: 2020 2020 2073 656c 6563 745f 706f 7274       select_port
-00011830: 735f 656c 6563 7472 6963 616c 3a0a 2020  s_electrical:.  
-00011840: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-00011850: 5f6f 7074 6963 616c 3a0a 2020 2020 2020  _optical:.      
-00011860: 2020 2020 2020 7072 6566 6978 5f65 6c65        prefix_ele
-00011870: 6374 7269 6361 6c3a 0a0a 2020 2020 2020  ctrical:..      
-00011880: 2020 2e2e 2063 6f64 653a 3a0a 0a20 2020    .. code::..   
-00011890: 2020 2020 2020 2020 2020 2020 2020 4e30                N0
-000118a0: 2020 4e31 0a20 2020 2020 2020 2020 2020    N1.           
-000118b0: 2020 2020 2020 7c5f 5f5f 7c5f 0a20 2020        |___|_.   
-000118c0: 2020 2020 2020 2020 2057 3120 2d7c 2020           W1 -|  
-000118d0: 2020 2020 7c2d 2045 310a 2020 2020 2020      |- E1.      
-000118e0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000118f0: 207c 0a20 2020 2020 2020 2020 2020 2057   |.            W
-00011900: 3020 2d7c 5f5f 5f5f 5f5f 7c2d 2045 300a  0 -|______|- E0.
-00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011920: 207c 2020 207c 0a20 2020 2020 2020 2020   |   |.         
-00011930: 2020 2020 2020 2053 3020 2020 5331 0a20         S0   S1. 
-00011940: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011950: 2020 2073 656c 662e 6973 5f75 6e6c 6f63     self.is_unloc
-00011960: 6b65 6428 290a 2020 2020 2020 2020 6175  ked().        au
-00011970: 746f 5f72 656e 616d 655f 706f 7274 735f  to_rename_ports_
-00011980: 6f72 6965 6e74 6174 696f 6e28 7365 6c66  orientation(self
-00011990: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
-000119a0: 2064 6566 206d 6f76 6528 0a20 2020 2020   def move(.     
-000119b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000119c0: 206f 7269 6769 6e3a 2046 6c6f 6174 3220   origin: Float2 
-000119d0: 3d20 2830 2c20 3029 2c0a 2020 2020 2020  = (0, 0),.      
-000119e0: 2020 6465 7374 696e 6174 696f 6e3a 204f    destination: O
-000119f0: 7074 696f 6e61 6c5b 466c 6f61 7432 5d20  ptional[Float2] 
-00011a00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00011a10: 6178 6973 3a20 4f70 7469 6f6e 616c 5b41  axis: Optional[A
-00011a20: 7869 735d 203d 204e 6f6e 652c 0a20 2020  xis] = None,.   
-00011a30: 2029 202d 3e20 436f 6d70 6f6e 656e 743a   ) -> Component:
-00011a40: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00011a50: 726e 7320 6e65 7720 436f 6d70 6f6e 656e  rns new Componen
-00011a60: 7420 7769 7468 2061 206d 6f76 6564 2072  t with a moved r
-00011a70: 6566 6572 656e 6365 2074 6f20 7468 6520  eference to the 
-00011a80: 6f72 6967 696e 616c 2e0a 0a20 2020 2020  original...     
-00011a90: 2020 2063 6f6d 706f 6e65 6e74 2e0a 0a20     component... 
-00011aa0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00011ab0: 2020 2020 2020 2020 206f 7269 6769 6e3a           origin:
-00011ac0: 206f 6620 636f 6d70 6f6e 656e 742e 0a20   of component.. 
-00011ad0: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00011ae0: 6e61 7469 6f6e 3a20 782c 2079 2e0a 2020  nation: x, y..  
-00011af0: 2020 2020 2020 2020 2020 6178 6973 3a20            axis: 
-00011b00: 7820 6f72 2079 2e0a 2020 2020 2020 2020  x or y..        
-00011b10: 2222 220a 2020 2020 2020 2020 7261 6973  """.        rais
-00011b20: 6520 5661 6c75 6545 7272 6f72 286d 6f76  e ValueError(mov
-00011b30: 655f 6572 726f 725f 6d65 7373 6167 6529  e_error_message)
-00011b40: 0a0a 2020 2020 6465 6620 6d69 7272 6f72  ..    def mirror
-00011b50: 2873 656c 662c 2070 313a 2046 6c6f 6174  (self, p1: Float
-00011b60: 3220 3d20 2830 2c20 3129 2c20 7032 3a20  2 = (0, 1), p2: 
-00011b70: 466c 6f61 7432 203d 2028 302c 2030 292c  Float2 = (0, 0),
-00011b80: 202a 2a6b 7761 7267 7329 202d 3e20 436f   **kwargs) -> Co
-00011b90: 6d70 6f6e 656e 743a 0a20 2020 2020 2020  mponent:.       
-00011ba0: 2022 2222 5265 7475 726e 7320 6e65 7720   """Returns new 
-00011bb0: 436f 6d70 6f6e 656e 7420 7769 7468 2061  Component with a
-00011bc0: 206d 6972 726f 7265 6420 7265 6665 7265   mirrored refere
-00011bd0: 6e63 652e 0a0a 2020 2020 2020 2020 4172  nce...        Ar
-00011be0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00011bf0: 7031 3a20 6669 7273 7420 706f 696e 7420  p1: first point 
-00011c00: 746f 2064 6566 696e 6520 6d69 7272 6f72  to define mirror
-00011c10: 2061 7869 732e 0a20 2020 2020 2020 2020   axis..         
-00011c20: 2020 2070 323a 2073 6563 6f6e 6420 706f     p2: second po
-00011c30: 696e 7420 746f 2064 6566 696e 6520 6d69  int to define mi
-00011c40: 7272 6f72 2061 7869 732e 0a20 2020 2020  rror axis..     
-00011c50: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
-00011c60: 726f 6d20 6764 7366 6163 746f 7279 2e66  rom gdsfactory.f
-00011c70: 756e 6374 696f 6e73 2069 6d70 6f72 7420  unctions import 
-00011c80: 6d69 7272 6f72 0a0a 2020 2020 2020 2020  mirror..        
-00011c90: 7265 7475 726e 206d 6972 726f 7228 636f  return mirror(co
-00011ca0: 6d70 6f6e 656e 743d 7365 6c66 2c20 7031  mponent=self, p1
-00011cb0: 3d70 312c 2070 323d 7032 2c20 2a2a 6b77  =p1, p2=p2, **kw
-00011cc0: 6172 6773 290a 0a20 2020 2064 6566 2072  args)..    def r
-00011cd0: 6f74 6174 6528 7365 6c66 2c20 616e 676c  otate(self, angl
-00011ce0: 653a 2066 6c6f 6174 203d 2039 302c 202a  e: float = 90, *
-00011cf0: 2a6b 7761 7267 7329 202d 3e20 436f 6d70  *kwargs) -> Comp
-00011d00: 6f6e 656e 743a 0a20 2020 2020 2020 2022  onent:.        "
-00011d10: 2222 5265 7475 726e 7320 6e65 7720 636f  ""Returns new co
-00011d20: 6d70 6f6e 656e 7420 7769 7468 2061 2072  mponent with a r
-00011d30: 6f74 6174 6564 2072 6566 6572 656e 6365  otated reference
-00011d40: 2074 6f20 7468 6520 6f72 6967 696e 616c   to the original
-00011d50: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00011d60: 0a20 2020 2020 2020 2020 2020 2061 6e67  .            ang
-00011d70: 6c65 3a20 696e 2064 6567 7265 6573 2e0a  le: in degrees..
-00011d80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011d90: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
-00011da0: 6f72 792e 6675 6e63 7469 6f6e 7320 696d  ory.functions im
-00011db0: 706f 7274 2072 6f74 6174 650a 0a20 2020  port rotate..   
-00011dc0: 2020 2020 2072 6574 7572 6e20 726f 7461       return rota
-00011dd0: 7465 2863 6f6d 706f 6e65 6e74 3d73 656c  te(component=sel
-00011de0: 662c 2061 6e67 6c65 3d61 6e67 6c65 2c20  f, angle=angle, 
-00011df0: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
-00011e00: 6566 2061 6464 5f70 6164 6469 6e67 2873  ef add_padding(s
-00011e10: 656c 662c 202a 2a6b 7761 7267 7329 202d  elf, **kwargs) -
-00011e20: 3e20 436f 6d70 6f6e 656e 743a 0a20 2020  > Component:.   
-00011e30: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
-00011e40: 7361 6d65 2063 6f6d 706f 6e65 6e74 2077  same component w
-00011e50: 6974 6820 7061 6464 696e 672e 0a0a 2020  ith padding...  
-00011e60: 2020 2020 2020 4b65 7977 6f72 6420 4172        Keyword Ar
-00011e70: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00011e80: 636f 6d70 6f6e 656e 743a 2066 6f72 2070  component: for p
-00011e90: 6164 6469 6e67 2e0a 2020 2020 2020 2020  adding..        
-00011ea0: 2020 2020 6c61 7965 7273 3a20 6c69 7374      layers: list
-00011eb0: 206f 6620 6c61 7965 7273 2e0a 2020 2020   of layers..    
-00011ec0: 2020 2020 2020 2020 7375 6666 6978 2066          suffix f
-00011ed0: 6f72 206e 616d 652e 0a20 2020 2020 2020  or name..       
-00011ee0: 2020 2020 2064 6566 6175 6c74 3a20 6465       default: de
-00011ef0: 6661 756c 7420 7061 6464 696e 6720 2835  fault padding (5
-00011f00: 3075 6d29 2e0a 2020 2020 2020 2020 2020  0um)..          
-00011f10: 2020 746f 703a 206e 6f72 7468 2070 6164    top: north pad
-00011f20: 6469 6e67 2e0a 2020 2020 2020 2020 2020  ding..          
-00011f30: 2020 626f 7474 6f6d 3a20 736f 7574 6820    bottom: south 
-00011f40: 7061 6464 696e 672e 0a20 2020 2020 2020  padding..       
-00011f50: 2020 2020 2072 6967 6874 3a20 6561 7374       right: east
-00011f60: 2070 6164 6469 6e67 2e0a 2020 2020 2020   padding..      
-00011f70: 2020 2020 2020 6c65 6674 3a20 7765 7374        left: west
-00011f80: 2070 6164 6469 6e67 2e0a 2020 2020 2020   padding..      
-00011f90: 2020 2222 220a 2020 2020 2020 2020 6672    """.        fr
-00011fa0: 6f6d 2067 6473 6661 6374 6f72 792e 6164  om gdsfactory.ad
-00011fb0: 645f 7061 6464 696e 6720 696d 706f 7274  d_padding import
-00011fc0: 2061 6464 5f70 6164 6469 6e67 0a0a 2020   add_padding..  
-00011fd0: 2020 2020 2020 7265 7475 726e 2061 6464        return add
-00011fe0: 5f70 6164 6469 6e67 2863 6f6d 706f 6e65  _padding(compone
-00011ff0: 6e74 3d73 656c 662c 202a 2a6b 7761 7267  nt=self, **kwarg
-00012000: 7329 0a0a 2020 2020 6465 6620 6162 736f  s)..    def abso
-00012010: 7262 2873 656c 662c 2072 6566 6572 656e  rb(self, referen
-00012020: 6365 2920 2d3e 2043 6f6d 706f 6e65 6e74  ce) -> Component
-00012030: 3a0a 2020 2020 2020 2020 2222 2241 6273  :.        """Abs
-00012040: 6f72 6273 2070 6f6c 7967 6f6e 7320 6672  orbs polygons fr
-00012050: 6f6d 2043 6f6d 706f 6e65 6e74 5265 6665  om ComponentRefe
-00012060: 7265 6e63 6520 696e 746f 2043 6f6d 706f  rence into Compo
-00012070: 6e65 6e74 2e0a 0a20 2020 2020 2020 2044  nent...        D
-00012080: 6573 7472 6f79 7320 7468 6520 7265 6665  estroys the refe
-00012090: 7265 6e63 6520 696e 2074 6865 2070 726f  rence in the pro
-000120a0: 6365 7373 2062 7574 206b 6565 7069 6e67  cess but keeping
-000120b0: 2074 6865 2070 6f6c 7967 6f6e 2067 656f   the polygon geo
-000120c0: 6d65 7472 792e 0a0a 2020 2020 2020 2020  metry...        
-000120d0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-000120e0: 2020 7265 6665 7265 6e63 653a 2043 6f6d    reference: Com
-000120f0: 706f 6e65 6e74 5265 6665 7265 6e63 6520  ponentReference 
-00012100: 746f 2062 6520 6162 736f 7262 6564 2069  to be absorbed i
-00012110: 6e74 6f20 7468 6520 436f 6d70 6f6e 656e  nto the Componen
-00012120: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
-00012130: 2020 2020 2020 2069 6620 7265 6665 7265         if refere
-00012140: 6e63 6520 6e6f 7420 696e 2073 656c 662e  nce not in self.
-00012150: 7265 6665 7265 6e63 6573 3a0a 2020 2020  references:.    
-00012160: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00012170: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-00012180: 2020 2020 2020 2020 2020 2254 6865 2072            "The r
-00012190: 6566 6572 656e 6365 2079 6f75 2061 736b  eference you ask
-000121a0: 6564 2074 6f20 6162 736f 7262 2064 6f65  ed to absorb doe
-000121b0: 7320 6e6f 7420 6578 6973 7420 696e 2074  s not exist in t
-000121c0: 6869 7320 436f 6d70 6f6e 656e 742e 220a  his Component.".
-000121d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000121e0: 2020 2020 2020 7265 665f 706f 6c79 676f        ref_polygo
-000121f0: 6e73 203d 2072 6566 6572 656e 6365 2e67  ns = reference.g
-00012200: 6574 5f70 6f6c 7967 6f6e 7328 0a20 2020  et_polygons(.   
-00012210: 2020 2020 2020 2020 2062 795f 7370 6563           by_spec
-00012220: 3d46 616c 7365 2c20 696e 636c 7564 655f  =False, include_
-00012230: 7061 7468 733d 4661 6c73 652c 2061 735f  paths=False, as_
-00012240: 6172 7261 793d 4661 6c73 650a 2020 2020  array=False.    
-00012250: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00012260: 6c66 2e5f 6164 645f 706f 6c79 676f 6e73  lf._add_polygons
-00012270: 282a 7265 665f 706f 6c79 676f 6e73 290a  (*ref_polygons).
-00012280: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-00012290: 6428 7265 6665 7265 6e63 652e 6765 745f  d(reference.get_
-000122a0: 6c61 6265 6c73 2829 290a 2020 2020 2020  labels()).      
-000122b0: 2020 7365 6c66 2e61 6464 2872 6566 6572    self.add(refer
-000122c0: 656e 6365 2e67 6574 5f70 6174 6873 2829  ence.get_paths()
-000122d0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-000122e0: 656d 6f76 6528 7265 6665 7265 6e63 6529  emove(reference)
-000122f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012300: 7365 6c66 0a0a 2020 2020 6465 6620 7265  self..    def re
-00012310: 6d6f 7665 2873 656c 662c 2069 7465 6d73  move(self, items
-00012320: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-00012330: 6d6f 7665 7320 6974 656d 7320 6672 6f6d  moves items from
-00012340: 2061 2043 6f6d 706f 6e65 6e74 2c20 7768   a Component, wh
-00012350: 6963 6820 6361 6e20 696e 636c 7564 6520  ich can include 
-00012360: 506f 7274 732c 2050 6f6c 7967 6f6e 5365  Ports, PolygonSe
-00012370: 7473 205c 0a20 2020 2020 2020 2043 656c  ts \.        Cel
-00012380: 6c52 6566 6572 656e 6365 732c 2043 6f6d  lReferences, Com
-00012390: 706f 6e65 6e74 5265 6665 7265 6e63 6573  ponentReferences
-000123a0: 2061 6e64 204c 6162 656c 732e 0a0a 2020   and Labels...  
-000123b0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-000123c0: 2020 2020 2020 2020 6974 656d 733a 206c          items: l
-000123d0: 6973 7420 6f66 2049 7465 6d73 2074 6f20  ist of Items to 
-000123e0: 6265 2072 656d 6f76 6564 2066 726f 6d20  be removed from 
-000123f0: 7468 6520 436f 6d70 6f6e 656e 742e 0a20  the Component.. 
-00012400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012410: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
-00012420: 7228 6974 656d 732c 2022 5f5f 6974 6572  r(items, "__iter
-00012430: 5f5f 2229 3a0a 2020 2020 2020 2020 2020  __"):.          
-00012440: 2020 6974 656d 7320 3d20 5b69 7465 6d73    items = [items
-00012450: 5d0a 2020 2020 2020 2020 666f 7220 6974  ].        for it
-00012460: 656d 2069 6e20 6974 656d 733a 0a20 2020  em in items:.   
-00012470: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00012480: 7374 616e 6365 2869 7465 6d2c 2050 6f72  stance(item, Por
-00012490: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-000124a0: 2020 2020 7365 6c66 2e70 6f72 7473 203d      self.ports =
-000124b0: 207b 6b3a 2076 2066 6f72 206b 2c20 7620   {k: v for k, v 
-000124c0: 696e 2073 656c 662e 706f 7274 732e 6974  in self.ports.it
-000124d0: 656d 7328 2920 6966 2076 2021 3d20 6974  ems() if v != it
-000124e0: 656d 7d0a 2020 2020 2020 2020 2020 2020  em}.            
-000124f0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00012500: 6974 656d 2c20 6764 7374 6b2e 5265 6665  item, gdstk.Refe
-00012510: 7265 6e63 6529 3a0a 2020 2020 2020 2020  rence):.        
-00012520: 2020 2020 2020 2020 7365 6c66 2e5f 6365          self._ce
-00012530: 6c6c 2e72 656d 6f76 6528 6974 656d 290a  ll.remove(item).
-00012540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012550: 6974 656d 2e6f 776e 6572 203d 204e 6f6e  item.owner = Non
-00012560: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
-00012570: 6966 2069 7369 6e73 7461 6e63 6528 6974  if isinstance(it
-00012580: 656d 2c20 436f 6d70 6f6e 656e 7452 6566  em, ComponentRef
-00012590: 6572 656e 6365 293a 0a20 2020 2020 2020  erence):.       
-000125a0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000125b0: 6665 7265 6e63 6573 2e72 656d 6f76 6528  ferences.remove(
-000125c0: 6974 656d 290a 2020 2020 2020 2020 2020  item).          
-000125d0: 2020 2020 2020 7365 6c66 2e5f 6365 6c6c        self._cell
-000125e0: 2e72 656d 6f76 6528 6974 656d 2e5f 7265  .remove(item._re
-000125f0: 6665 7265 6e63 6529 0a20 2020 2020 2020  ference).       
-00012600: 2020 2020 2020 2020 2069 7465 6d2e 6f77           item.ow
-00012610: 6e65 7220 3d20 4e6f 6e65 0a20 2020 2020  ner = None.     
-00012620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012630: 5f6e 616d 6564 5f72 6566 6572 656e 6365  _named_reference
-00012640: 732e 706f 7028 6974 656d 2e6e 616d 6529  s.pop(item.name)
-00012650: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00012660: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00012670: 2020 2073 656c 662e 5f63 656c 6c2e 7265     self._cell.re
-00012680: 6d6f 7665 2869 7465 6d29 0a0a 2020 2020  move(item)..    
-00012690: 2020 2020 7365 6c66 2e5f 6262 5f76 616c      self._bb_val
-000126a0: 6964 203d 2046 616c 7365 0a20 2020 2020  id = False.     
-000126b0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-000126c0: 2020 2020 6465 6620 6861 7368 5f67 656f      def hash_geo
-000126d0: 6d65 7472 7928 7365 6c66 2c20 7072 6563  metry(self, prec
-000126e0: 6973 696f 6e3a 2066 6c6f 6174 203d 2031  ision: float = 1
-000126f0: 652d 3429 202d 3e20 7374 723a 0a20 2020  e-4) -> str:.   
-00012700: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
-00012710: 616e 2053 4841 3120 6861 7368 206f 6620  an SHA1 hash of 
-00012720: 7468 6520 6765 6f6d 6574 7279 2069 6e20  the geometry in 
-00012730: 7468 6520 436f 6d70 6f6e 656e 742e 0a0a  the Component...
-00012740: 2020 2020 2020 2020 466f 7220 6561 6368          For each
-00012750: 206c 6179 6572 2c20 6561 6368 2070 6f6c   layer, each pol
-00012760: 7967 6f6e 2069 7320 696e 6469 7669 6475  ygon is individu
-00012770: 616c 6c79 2068 6173 6865 6420 616e 6420  ally hashed and 
-00012780: 7468 656e 2074 6865 2070 6f6c 7967 6f6e  then the polygon
-00012790: 2068 6173 6865 730a 2020 2020 2020 2020   hashes.        
-000127a0: 6172 6520 736f 7274 6564 2c20 746f 2065  are sorted, to e
-000127b0: 6e73 7572 6520 7468 6520 6861 7368 2073  nsure the hash s
-000127c0: 7461 7973 2063 6f6e 7374 616e 7420 7265  tays constant re
-000127d0: 6761 7264 6c65 7373 206f 6620 7468 6520  gardless of the 
-000127e0: 6f72 6465 7269 6e67 0a20 2020 2020 2020  ordering.       
-000127f0: 2074 6865 2070 6f6c 7967 6f6e 732e 2020   the polygons.  
-00012800: 5369 6d69 6c61 726c 792c 2074 6865 206c  Similarly, the l
-00012810: 6179 6572 7320 6172 6520 736f 7274 6564  ayers are sorted
-00012820: 2062 7920 286c 6179 6572 2c20 6461 7461   by (layer, data
-00012830: 7479 7065 292e 0a0a 2020 2020 2020 2020  type)...        
-00012840: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00012850: 2020 7072 6563 6973 696f 6e3a 2052 6f75    precision: Rou
-00012860: 6e64 696e 6720 7072 6563 6973 696f 6e20  nding precision 
-00012870: 666f 7220 7468 6520 7468 6520 6f62 6a65  for the the obje
-00012880: 6374 7320 696e 2074 6865 2043 6f6d 706f  cts in the Compo
-00012890: 6e65 6e74 2e0a 2020 2020 2020 2020 2020  nent..          
-000128a0: 2020 2020 2020 466f 7220 696e 7374 616e        For instan
-000128b0: 6365 2c20 6120 7072 6563 6973 696f 6e20  ce, a precision 
-000128c0: 6f66 2031 652d 3220 7769 6c6c 2072 6f75  of 1e-2 will rou
-000128d0: 6e64 2061 2070 6f69 6e74 2061 740a 2020  nd a point at.  
-000128e0: 2020 2020 2020 2020 2020 2020 2020 2830                (0
-000128f0: 2e31 3234 2c20 312e 3734 3829 2074 6f20  .124, 1.748) to 
-00012900: 2830 2e31 322c 2031 2e37 3529 2e0a 0a20  (0.12, 1.75)... 
-00012910: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012920: 2020 2070 6f6c 7967 6f6e 735f 6279 5f73     polygons_by_s
-00012930: 7065 6320 3d20 7365 6c66 2e67 6574 5f70  pec = self.get_p
-00012940: 6f6c 7967 6f6e 7328 6279 5f73 7065 633d  olygons(by_spec=
-00012950: 5472 7565 2c20 6173 5f61 7272 6179 3d46  True, as_array=F
-00012960: 616c 7365 290a 2020 2020 2020 2020 6c61  alse).        la
-00012970: 7965 7273 203d 206e 702e 6172 7261 7928  yers = np.array(
-00012980: 6c69 7374 2870 6f6c 7967 6f6e 735f 6279  list(polygons_by
-00012990: 5f73 7065 632e 6b65 7973 2829 2929 0a20  _spec.keys())). 
-000129a0: 2020 2020 2020 2073 6f72 7465 645f 6c61         sorted_la
-000129b0: 7965 7273 203d 206c 6179 6572 735b 6e70  yers = layers[np
-000129c0: 2e6c 6578 736f 7274 2828 6c61 7965 7273  .lexsort((layers
-000129d0: 5b3a 2c20 305d 2c20 6c61 7965 7273 5b3a  [:, 0], layers[:
-000129e0: 2c20 315d 2929 5d0a 0a20 2020 2020 2020  , 1]))]..       
-000129f0: 2066 696e 616c 5f68 6173 6820 3d20 6861   final_hash = ha
-00012a00: 7368 6c69 622e 7368 6131 2829 0a20 2020  shlib.sha1().   
-00012a10: 2020 2020 2066 6f72 206c 6179 6572 2069       for layer i
-00012a20: 6e20 736f 7274 6564 5f6c 6179 6572 733a  n sorted_layers:
-00012a30: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-00012a40: 6572 5f68 6173 6820 3d20 6861 7368 6c69  er_hash = hashli
-00012a50: 622e 7368 6131 286c 6179 6572 2e61 7374  b.sha1(layer.ast
-00012a60: 7970 6528 6e70 2e69 6e74 3634 2929 2e64  ype(np.int64)).d
-00012a70: 6967 6573 7428 290a 2020 2020 2020 2020  igest().        
-00012a80: 2020 2020 706f 6c79 676f 6e73 203d 2070      polygons = p
-00012a90: 6f6c 7967 6f6e 735f 6279 5f73 7065 635b  olygons_by_spec[
-00012aa0: 7475 706c 6528 6c61 7965 7229 5d0a 2020  tuple(layer)].  
-00012ab0: 2020 2020 2020 2020 2020 706f 6c79 676f            polygo
-00012ac0: 6e73 203d 205b 5f72 6e64 2870 2e70 6f69  ns = [_rnd(p.poi
-00012ad0: 6e74 732c 2070 7265 6369 7369 6f6e 2920  nts, precision) 
-00012ae0: 666f 7220 7020 696e 2070 6f6c 7967 6f6e  for p in polygon
-00012af0: 735d 0a20 2020 2020 2020 2020 2020 2070  s].            p
-00012b00: 6f6c 7967 6f6e 5f68 6173 6865 7320 3d20  olygon_hashes = 
-00012b10: 6e70 2e73 6f72 7428 5b68 6173 686c 6962  np.sort([hashlib
-00012b20: 2e73 6861 3128 7029 2e64 6967 6573 7428  .sha1(p).digest(
-00012b30: 2920 666f 7220 7020 696e 2070 6f6c 7967  ) for p in polyg
-00012b40: 6f6e 735d 290a 2020 2020 2020 2020 2020  ons]).          
-00012b50: 2020 6669 6e61 6c5f 6861 7368 2e75 7064    final_hash.upd
-00012b60: 6174 6528 6c61 7965 725f 6861 7368 290a  ate(layer_hash).
-00012b70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00012b80: 7068 2069 6e20 706f 6c79 676f 6e5f 6861  ph in polygon_ha
-00012b90: 7368 6573 3a0a 2020 2020 2020 2020 2020  shes:.          
-00012ba0: 2020 2020 2020 6669 6e61 6c5f 6861 7368        final_hash
-00012bb0: 2e75 7064 6174 6528 7068 290a 0a20 2020  .update(ph)..   
-00012bc0: 2020 2020 2072 6574 7572 6e20 6669 6e61       return fina
-00012bd0: 6c5f 6861 7368 2e68 6578 6469 6765 7374  l_hash.hexdigest
-00012be0: 2829 0a0a 2020 2020 6465 6620 6765 745f  ()..    def get_
-00012bf0: 6c61 6265 6c73 280a 2020 2020 2020 2020  labels(.        
-00012c00: 7365 6c66 2c20 6170 706c 795f 7265 7065  self, apply_repe
-00012c10: 7469 7469 6f6e 733d 5472 7565 2c20 6465  titions=True, de
-00012c20: 7074 683a 204f 7074 696f 6e61 6c5b 696e  pth: Optional[in
-00012c30: 745d 203d 204e 6f6e 652c 206c 6179 6572  t] = None, layer
-00012c40: 3d4e 6f6e 650a 2020 2020 2920 2d3e 204c  =None.    ) -> L
-00012c50: 6973 745b 4c61 6265 6c5d 3a0a 2020 2020  ist[Label]:.    
-00012c60: 2020 2020 2222 2252 6574 7572 6e20 6c61      """Return la
-00012c70: 6265 6c73 2e0a 0a20 2020 2020 2020 2041  bels...        A
-00012c80: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00012c90: 2061 7070 6c79 5f72 6570 6574 6974 696f   apply_repetitio
-00012ca0: 6e73 3a2e 0a20 2020 2020 2020 2020 2020  ns:..           
-00012cb0: 2064 6570 7468 3a20 4e6f 6e65 2072 6574   depth: None ret
-00012cc0: 7572 6e73 2061 6c6c 206c 6162 656c 7320  urns all labels 
-00012cd0: 616e 6420 3020 746f 7020 6c65 7665 6c2e  and 0 top level.
-00012ce0: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-00012cf0: 6572 3a20 6c61 7965 7273 7065 632e 0a20  er: layerspec.. 
-00012d00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012d10: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
-00012d20: 7279 2e70 646b 2069 6d70 6f72 7420 6765  ry.pdk import ge
-00012d30: 745f 6c61 7965 720a 0a20 2020 2020 2020  t_layer..       
-00012d40: 2069 6620 6c61 7965 723a 0a20 2020 2020   if layer:.     
-00012d50: 2020 2020 2020 206c 6179 6572 2c20 7465         layer, te
-00012d60: 7874 7479 7065 203d 2067 6574 5f6c 6179  xttype = get_lay
-00012d70: 6572 286c 6179 6572 290a 2020 2020 2020  er(layer).      
-00012d80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00012d90: 2020 2020 7465 7874 7479 7065 203d 204e      texttype = N
-00012da0: 6f6e 650a 2020 2020 2020 2020 7265 7475  one.        retu
-00012db0: 726e 2073 656c 662e 5f63 656c 6c2e 6765  rn self._cell.ge
-00012dc0: 745f 6c61 6265 6c73 280a 2020 2020 2020  t_labels(.      
-00012dd0: 2020 2020 2020 6170 706c 795f 7265 7065        apply_repe
-00012de0: 7469 7469 6f6e 733d 6170 706c 795f 7265  titions=apply_re
-00012df0: 7065 7469 7469 6f6e 732c 0a20 2020 2020  petitions,.     
-00012e00: 2020 2020 2020 2064 6570 7468 3d64 6570         depth=dep
-00012e10: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-00012e20: 6c61 7965 723d 6c61 7965 722c 0a20 2020  layer=layer,.   
-00012e30: 2020 2020 2020 2020 2074 6578 7474 7970           texttyp
-00012e40: 653d 7465 7874 7479 7065 2c0a 2020 2020  e=texttype,.    
-00012e50: 2020 2020 290a 0a20 2020 2064 6566 2072      )..    def r
-00012e60: 656d 6f76 655f 6c61 6265 6c73 2873 656c  emove_labels(sel
-00012e70: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00012e80: 2020 2020 2222 2252 656d 6f76 6520 6c61      """Remove la
-00012e90: 6265 6c73 2e22 2222 0a20 2020 2020 2020  bels.""".       
-00012ea0: 2073 656c 662e 5f63 656c 6c2e 7265 6d6f   self._cell.remo
-00012eb0: 7665 282a 7365 6c66 2e6c 6162 656c 7329  ve(*self.labels)
-00012ec0: 0a0a 2020 2020 2320 4465 7072 6563 6174  ..    # Deprecat
-00012ed0: 6564 0a20 2020 2064 6566 2067 6574 5f69  ed.    def get_i
-00012ee0: 6e66 6f28 7365 6c66 293a 0a20 2020 2020  nfo(self):.     
-00012ef0: 2020 2022 2222 4761 7468 6572 7320 7468     """Gathers th
-00012f00: 6520 2e69 6e66 6f20 6469 6374 696f 6e61  e .info dictiona
-00012f10: 7269 6573 2066 726f 6d20 6576 6572 7920  ries from every 
-00012f20: 7375 622d 436f 6d70 6f6e 656e 7420 616e  sub-Component an
-00012f30: 6420 7265 7475 726e 7320 7468 656d 2069  d returns them i
-00012f40: 6e20 6120 6c69 7374 2e0a 0a20 2020 2020  n a list...     
-00012f50: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00012f60: 2020 2020 2064 6570 7468 3a20 696e 7420       depth: int 
-00012f70: 6f72 204e 6f6e 650a 2020 2020 2020 2020  or None.        
-00012f80: 2020 2020 2020 2020 4966 206e 6f74 204e          If not N
-00012f90: 6f6e 652c 2064 6566 696e 6573 2066 726f  one, defines fro
-00012fa0: 6d20 686f 7720 6d61 6e79 2072 6566 6572  m how many refer
-00012fb0: 656e 6365 206c 6576 656c 7320 746f 0a20  ence levels to. 
-00012fc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012fd0: 6574 7269 6576 6520 506f 7274 7320 6672  etrieve Ports fr
-00012fe0: 6f6d 2e0a 0a20 2020 2020 2020 2052 6574  om...        Ret
-00012ff0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00013000: 2020 6c69 7374 206f 6620 6469 6374 696f    list of dictio
-00013010: 6e61 7269 6573 0a20 2020 2020 2020 2020  naries.         
-00013020: 2020 2020 2020 204c 6973 7420 6f66 2074         List of t
-00013030: 6865 2022 2e69 6e66 6f22 2070 726f 7065  he ".info" prope
-00013040: 7274 7920 6469 6374 696f 6e61 7269 6573  rty dictionaries
-00013050: 2066 726f 6d20 616c 6c20 7375 622d 436f   from all sub-Co
-00013060: 6d70 6f6e 656e 7473 0a20 2020 2020 2020  mponents.       
-00013070: 2022 2222 0a20 2020 2020 2020 2044 5f6c   """.        D_l
-00013080: 6973 7420 3d20 7365 6c66 2e67 6574 5f64  ist = self.get_d
-00013090: 6570 656e 6465 6e63 6965 7328 7265 6375  ependencies(recu
-000130a0: 7273 6976 653d 5472 7565 290a 2020 2020  rsive=True).    
-000130b0: 2020 2020 7265 7475 726e 205b 442e 696e      return [D.in
-000130c0: 666f 2e63 6f70 7928 2920 666f 7220 4420  fo.copy() for D 
-000130d0: 696e 2044 5f6c 6973 745d 0a0a 2020 2020  in D_list]..    
-000130e0: 6465 6620 7265 6d61 705f 6c61 7965 7273  def remap_layers
-000130f0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00013100: 6c61 7965 726d 6170 2c20 696e 636c 7564  layermap, includ
-00013110: 655f 6c61 6265 6c73 3a20 626f 6f6c 203d  e_labels: bool =
-00013120: 2054 7275 652c 2069 6e63 6c75 6465 5f70   True, include_p
-00013130: 6174 6873 3a20 626f 6f6c 203d 2054 7275  aths: bool = Tru
-00013140: 650a 2020 2020 2920 2d3e 2043 6f6d 706f  e.    ) -> Compo
-00013150: 6e65 6e74 3a0a 2020 2020 2020 2020 2222  nent:.        ""
-00013160: 2252 6574 7572 6e73 2061 2063 6f70 7920  "Returns a copy 
-00013170: 6f66 2074 6865 2063 6f6d 706f 6e65 6e74  of the component
-00013180: 2077 6974 6820 7265 6d61 7070 6564 206c   with remapped l
-00013190: 6179 6572 732e 0a0a 2020 2020 2020 2020  ayers...        
-000131a0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-000131b0: 2020 6c61 7965 726d 6170 3a20 4469 6374    layermap: Dict
-000131c0: 696f 6e61 7279 206f 6620 7661 6c75 6573  ionary of values
-000131d0: 2069 6e20 666f 726d 6174 207b 6c61 7965   in format {laye
-000131e0: 725f 6672 6f6d 203a 206c 6179 6572 5f74  r_from : layer_t
-000131f0: 6f7d 2e0a 2020 2020 2020 2020 2020 2020  o}..            
-00013200: 696e 636c 7564 655f 6c61 6265 6c73 3a20  include_labels: 
-00013210: 5365 6c65 6374 7320 7768 6574 6865 7220  Selects whether 
-00013220: 746f 206d 6f76 6520 4c61 6265 6c73 2061  to move Labels a
-00013230: 6c6f 6e67 2077 6974 6820 706f 6c79 676f  long with polygo
-00013240: 6e73 2e0a 2020 2020 2020 2020 2020 2020  ns..            
-00013250: 696e 636c 7564 655f 7061 7468 733a 2053  include_paths: S
-00013260: 656c 6563 7473 2077 6865 7468 6572 2074  elects whether t
-00013270: 6f20 6d6f 7665 2050 6174 6873 2061 6c6f  o move Paths alo
-00013280: 6e67 2077 6974 6820 706f 6c79 676f 6e73  ng with polygons
-00013290: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000132a0: 2020 2020 2020 636f 6d70 6f6e 656e 7420        component 
-000132b0: 3d20 7365 6c66 2e63 6f70 7928 290a 2020  = self.copy().  
-000132c0: 2020 2020 2020 6c61 7965 726d 6170 203d        layermap =
-000132d0: 207b 5f70 6172 7365 5f6c 6179 6572 286b   {_parse_layer(k
-000132e0: 293a 205f 7061 7273 655f 6c61 7965 7228  ): _parse_layer(
-000132f0: 7629 2066 6f72 206b 2c20 7620 696e 206c  v) for k, v in l
-00013300: 6179 6572 6d61 702e 6974 656d 7328 297d  ayermap.items()}
-00013310: 0a0a 2020 2020 2020 2020 616c 6c5f 4420  ..        all_D 
-00013320: 3d20 6c69 7374 2863 6f6d 706f 6e65 6e74  = list(component
-00013330: 2e67 6574 5f64 6570 656e 6465 6e63 6965  .get_dependencie
-00013340: 7328 5472 7565 2929 0a20 2020 2020 2020  s(True)).       
-00013350: 2061 6c6c 5f44 2e61 7070 656e 6428 636f   all_D.append(co
-00013360: 6d70 6f6e 656e 7429 0a20 2020 2020 2020  mponent).       
-00013370: 2066 6f72 2044 2069 6e20 616c 6c5f 443a   for D in all_D:
-00013380: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00013390: 2070 2069 6e20 442e 706f 6c79 676f 6e73   p in D.polygons
-000133a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000133b0: 2020 6c61 7965 7220 3d20 2870 2e6c 6179    layer = (p.lay
-000133c0: 6572 2c20 702e 6461 7461 7479 7065 290a  er, p.datatype).
-000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 6966 206c 6179 6572 2069 6e20 6c61 7965  if layer in laye
-000133f0: 726d 6170 3a0a 2020 2020 2020 2020 2020  rmap:.          
-00013400: 2020 2020 2020 2020 2020 6e65 775f 6c61            new_la
-00013410: 7965 7220 3d20 6c61 7965 726d 6170 5b6c  yer = layermap[l
-00013420: 6179 6572 5d0a 2020 2020 2020 2020 2020  ayer].          
-00013430: 2020 2020 2020 2020 2020 702e 6c61 7965            p.laye
-00013440: 7220 3d20 6e65 775f 6c61 7965 725b 305d  r = new_layer[0]
-00013450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013460: 2020 2020 2070 2e64 6174 6174 7970 6520       p.datatype 
-00013470: 3d20 6e65 775f 6c61 7965 725b 315d 0a20  = new_layer[1]. 
-00013480: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-00013490: 636c 7564 655f 6c61 6265 6c73 3a0a 2020  clude_labels:.  
-000134a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000134b0: 7220 6c61 6265 6c20 696e 2044 2e6c 6162  r label in D.lab
-000134c0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
-000134d0: 2020 2020 2020 2020 206f 7269 6769 6e61           origina
-000134e0: 6c5f 6c61 7965 7220 3d20 286c 6162 656c  l_layer = (label
-000134f0: 2e6c 6179 6572 2c20 6c61 6265 6c2e 7465  .layer, label.te
-00013500: 7874 7479 7065 290a 2020 2020 2020 2020  xttype).        
-00013510: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-00013520: 696e 616c 5f6c 6179 6572 203d 205f 7061  inal_layer = _pa
-00013530: 7273 655f 6c61 7965 7228 6f72 6967 696e  rse_layer(origin
-00013540: 616c 5f6c 6179 6572 290a 2020 2020 2020  al_layer).      
-00013550: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00013560: 206f 7269 6769 6e61 6c5f 6c61 7965 7220   original_layer 
-00013570: 696e 206c 6179 6572 6d61 703a 0a20 2020  in layermap:.   
-00013580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013590: 2020 2020 206e 6577 5f6c 6179 6572 203d       new_layer =
-000135a0: 206c 6179 6572 6d61 705b 6f72 6967 696e   layermap[origin
-000135b0: 616c 5f6c 6179 6572 5d0a 2020 2020 2020  al_layer].      
-000135c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135d0: 2020 6c61 6265 6c2e 6c61 7965 7220 3d20    label.layer = 
-000135e0: 6e65 775f 6c61 7965 725b 305d 0a20 2020  new_layer[0].   
-000135f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013600: 2020 2020 206c 6162 656c 2e74 6578 7474       label.textt
-00013610: 7970 6520 3d20 6e65 775f 6c61 7965 725b  ype = new_layer[
-00013620: 315d 0a0a 2020 2020 2020 2020 2020 2020  1]..            
-00013630: 6966 2069 6e63 6c75 6465 5f70 6174 6873  if include_paths
-00013640: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013650: 2020 666f 7220 7061 7468 2069 6e20 442e    for path in D.
-00013660: 7061 7468 733a 0a20 2020 2020 2020 2020  paths:.         
-00013670: 2020 2020 2020 2020 2020 206e 6577 5f6c             new_l
-00013680: 6179 6572 7320 3d20 6c69 7374 2870 6174  ayers = list(pat
-00013690: 682e 6c61 7965 7273 290a 2020 2020 2020  h.layers).      
-000136a0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-000136b0: 775f 6461 7461 7479 7065 7320 3d20 6c69  w_datatypes = li
-000136c0: 7374 2870 6174 682e 6461 7461 7479 7065  st(path.datatype
-000136d0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-000136e0: 2020 2020 2020 2066 6f72 206c 6179 6572         for layer
-000136f0: 5f6e 756d 6265 7220 696e 2072 616e 6765  _number in range
-00013700: 286c 656e 286e 6577 5f6c 6179 6572 7329  (len(new_layers)
-00013710: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00013720: 2020 2020 2020 2020 2020 206f 7269 6769             origi
-00013730: 6e61 6c5f 6c61 7965 7220 3d20 5f70 6172  nal_layer = _par
-00013740: 7365 5f6c 6179 6572 280a 2020 2020 2020  se_layer(.      
-00013750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013760: 2020 2020 2020 286e 6577 5f6c 6179 6572        (new_layer
-00013770: 735b 6c61 7965 725f 6e75 6d62 6572 5d2c  s[layer_number],
-00013780: 206e 6577 5f64 6174 6174 7970 6573 5b6c   new_datatypes[l
-00013790: 6179 6572 5f6e 756d 6265 725d 290a 2020  ayer_number]).  
-000137a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000137c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137d0: 6966 206f 7269 6769 6e61 6c5f 6c61 7965  if original_laye
-000137e0: 7220 696e 206c 6179 6572 6d61 703a 0a20  r in layermap:. 
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 2020 2020 2020 2020 2020 206e 6577 5f6c             new_l
-00013810: 6179 6572 203d 206c 6179 6572 6d61 705b  ayer = layermap[
-00013820: 6f72 6967 696e 616c 5f6c 6179 6572 5d0a  original_layer].
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00013850: 6c61 7965 7273 5b6c 6179 6572 5f6e 756d  layers[layer_num
-00013860: 6265 725d 203d 206e 6577 5f6c 6179 6572  ber] = new_layer
-00013870: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00013880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013890: 6e65 775f 6461 7461 7479 7065 735b 6c61  new_datatypes[la
-000138a0: 7965 725f 6e75 6d62 6572 5d20 3d20 6e65  yer_number] = ne
-000138b0: 775f 6c61 7965 725b 315d 0a20 2020 2020  w_layer[1].     
-000138c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000138d0: 6174 682e 7365 745f 6c61 7965 7273 282a  ath.set_layers(*
-000138e0: 6e65 775f 6c61 7965 7273 290a 2020 2020  new_layers).    
-000138f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013900: 7061 7468 2e73 6574 5f64 6174 6174 7970  path.set_datatyp
-00013910: 6573 282a 6e65 775f 6461 7461 7479 7065  es(*new_datatype
-00013920: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
-00013930: 6e20 636f 6d70 6f6e 656e 740a 0a20 2020  n component..   
-00013940: 2064 6566 2074 6f5f 3364 280a 2020 2020   def to_3d(.    
-00013950: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00013960: 2020 6c61 7965 725f 7669 6577 733a 204f    layer_views: O
-00013970: 7074 696f 6e61 6c5b 4c61 7965 7256 6965  ptional[LayerVie
-00013980: 7773 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ws] = None,.    
-00013990: 2020 2020 6c61 7965 725f 7374 6163 6b3a      layer_stack:
-000139a0: 204f 7074 696f 6e61 6c5b 4c61 7965 7253   Optional[LayerS
-000139b0: 7461 636b 5d20 3d20 4e6f 6e65 2c0a 2020  tack] = None,.  
-000139c0: 2020 2020 2020 6578 636c 7564 655f 6c61        exclude_la
-000139d0: 7965 7273 3a20 4f70 7469 6f6e 616c 5b54  yers: Optional[T
-000139e0: 7570 6c65 5b4c 6179 6572 2c20 2e2e 2e5d  uple[Layer, ...]
-000139f0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
-00013a00: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00013a10: 726e 2043 6f6d 706f 6e65 6e74 2033 4420  rn Component 3D 
-00013a20: 7472 696d 6573 6820 5363 656e 652e 0a0a  trimesh Scene...
-00013a30: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00013a40: 2020 2020 2020 2020 2020 636f 6d70 6f6e            compon
-00013a50: 656e 743a 2074 6f20 6578 7472 7564 6520  ent: to extrude 
-00013a60: 696e 2033 442e 0a20 2020 2020 2020 2020  in 3D..         
-00013a70: 2020 206c 6179 6572 5f76 6965 7773 3a20     layer_views: 
-00013a80: 6c61 7965 7220 636f 6c6f 7273 2066 726f  layer colors fro
-00013a90: 6d20 4b6c 6179 6f75 7420 4c61 7965 7220  m Klayout Layer 
-00013aa0: 5072 6f70 6572 7469 6573 2066 696c 652e  Properties file.
-00013ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ac0: 2044 6566 6175 6c74 7320 746f 2061 6374   Defaults to act
-00013ad0: 6976 6520 5044 4b2e 6c61 7965 725f 7669  ive PDK.layer_vi
-00013ae0: 6577 732e 0a20 2020 2020 2020 2020 2020  ews..           
-00013af0: 206c 6179 6572 5f73 7461 636b 3a20 636f   layer_stack: co
-00013b00: 6e74 6169 6e73 2074 6869 636b 6e65 7373  ntains thickness
-00013b10: 2061 6e64 207a 6d69 6e20 666f 7220 6561   and zmin for ea
-00013b20: 6368 206c 6179 6572 2e0a 2020 2020 2020  ch layer..      
-00013b30: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00013b40: 7473 2074 6f20 6163 7469 7665 2050 444b  ts to active PDK
-00013b50: 2e6c 6179 6572 5f73 7461 636b 2e0a 2020  .layer_stack..  
-00013b60: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
-00013b70: 655f 6c61 7965 7273 3a20 6c61 7965 7273  e_layers: layers
-00013b80: 2074 6f20 6578 636c 7564 652e 0a0a 2020   to exclude...  
-00013b90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013ba0: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
-00013bb0: 792e 6578 706f 7274 2e74 6f5f 3364 2069  y.export.to_3d i
-00013bc0: 6d70 6f72 7420 746f 5f33 640a 0a20 2020  mport to_3d..   
-00013bd0: 2020 2020 2072 6574 7572 6e20 746f 5f33       return to_3
-00013be0: 6428 0a20 2020 2020 2020 2020 2020 2073  d(.            s
-00013bf0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-00013c00: 206c 6179 6572 5f76 6965 7773 3d6c 6179   layer_views=lay
-00013c10: 6572 5f76 6965 7773 2c0a 2020 2020 2020  er_views,.      
-00013c20: 2020 2020 2020 6c61 7965 725f 7374 6163        layer_stac
-00013c30: 6b3d 6c61 7965 725f 7374 6163 6b2c 0a20  k=layer_stack,. 
-00013c40: 2020 2020 2020 2020 2020 2065 7863 6c75             exclu
-00013c50: 6465 5f6c 6179 6572 733d 6578 636c 7564  de_layers=exclud
-00013c60: 655f 6c61 7965 7273 2c0a 2020 2020 2020  e_layers,.      
-00013c70: 2020 290a 0a20 2020 2064 6566 2074 6f5f    )..    def to_
-00013c80: 6e70 280a 2020 2020 2020 2020 7365 6c66  np(.        self
-00013c90: 2c0a 2020 2020 2020 2020 6e6d 5f70 6572  ,.        nm_per
-00013ca0: 5f70 6978 656c 3a20 696e 7420 3d20 3230  _pixel: int = 20
-00013cb0: 2c0a 2020 2020 2020 2020 6c61 7965 7273  ,.        layers
-00013cc0: 3a20 4c61 7965 7273 203d 2028 2831 2c20  : Layers = ((1, 
-00013cd0: 3029 2c29 2c0a 2020 2020 2020 2020 7661  0),),.        va
-00013ce0: 6c75 6573 3a20 4f70 7469 6f6e 616c 5b54  lues: Optional[T
-00013cf0: 7570 6c65 5b66 6c6f 6174 2c20 2e2e 2e5d  uple[float, ...]
-00013d00: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00013d10: 2020 7061 645f 7769 6474 683a 2069 6e74    pad_width: int
-00013d20: 203d 2031 2c0a 2020 2020 2920 2d3e 206e   = 1,.    ) -> n
-00013d30: 702e 6e64 6172 7261 793a 0a20 2020 2020  p.ndarray:.     
-00013d40: 2020 2022 2222 5265 7475 726e 7320 6120     """Returns a 
-00013d50: 7069 7865 6c61 7465 6420 6e75 6d70 7920  pixelated numpy 
-00013d60: 6172 7261 7920 6672 6f6d 2043 6f6d 706f  array from Compo
-00013d70: 6e65 6e74 2070 6f6c 7967 6f6e 732e 0a0a  nent polygons...
-00013d80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00013d90: 2020 2020 2020 2020 2020 636f 6d70 6f6e            compon
-00013da0: 656e 743a 2043 6f6d 706f 6e65 6e74 2e0a  ent: Component..
-00013db0: 2020 2020 2020 2020 2020 2020 6e6d 5f70              nm_p
-00013dc0: 6572 5f70 6978 656c 3a20 796f 7520 6361  er_pixel: you ca
-00013dd0: 6e20 676f 2066 726f 6d20 3230 2028 636f  n go from 20 (co
-00013de0: 6172 7365 2920 746f 2034 2028 6669 6e65  arse) to 4 (fine
-00013df0: 292e 0a20 2020 2020 2020 2020 2020 206c  )..            l
-00013e00: 6179 6572 733a 2074 6f20 636f 6e76 6572  ayers: to conver
-00013e10: 742e 204f 7264 6572 206d 6174 7465 7273  t. Order matters
-00013e20: 2028 6c61 7474 6572 206f 7665 7277 7269   (latter overwri
-00013e30: 7465 2066 6f72 6d65 7229 2e0a 2020 2020  te former)..    
-00013e40: 2020 2020 2020 2020 7661 6c75 6573 3a20          values: 
-00013e50: 6173 736f 6369 6174 6564 2074 6f20 6561  associated to ea
-00013e60: 6368 206c 6179 6572 2028 6465 6661 756c  ch layer (defaul
-00013e70: 7473 2074 6f20 3129 2e0a 2020 2020 2020  ts to 1)..      
-00013e80: 2020 2020 2020 7061 645f 7769 6474 683a        pad_width:
-00013e90: 2070 6164 6469 6e67 2070 6978 656c 7320   padding pixels 
-00013ea0: 6172 6f75 6e64 2074 6865 2069 6d61 6765  around the image
-00013eb0: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-00013ec0: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
-00013ed0: 6163 746f 7279 2e65 7870 6f72 742e 746f  actory.export.to
-00013ee0: 5f6e 7020 696d 706f 7274 2074 6f5f 6e70  _np import to_np
-00013ef0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00013f00: 2074 6f5f 6e70 280a 2020 2020 2020 2020   to_np(.        
-00013f10: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00013f20: 2020 2020 2020 6e6d 5f70 6572 5f70 6978        nm_per_pix
-00013f30: 656c 3d6e 6d5f 7065 725f 7069 7865 6c2c  el=nm_per_pixel,
-00013f40: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-00013f50: 6572 733d 6c61 7965 7273 2c0a 2020 2020  ers=layers,.    
-00013f60: 2020 2020 2020 2020 7661 6c75 6573 3d76          values=v
-00013f70: 616c 7565 732c 0a20 2020 2020 2020 2020  alues,.         
-00013f80: 2020 2070 6164 5f77 6964 7468 3d70 6164     pad_width=pad
-00013f90: 5f77 6964 7468 2c0a 2020 2020 2020 2020  _width,.        
-00013fa0: 290a 0a20 2020 2064 6566 2077 7269 7465  )..    def write
-00013fb0: 5f73 746c 280a 2020 2020 2020 2020 7365  _stl(.        se
-00013fc0: 6c66 2c0a 2020 2020 2020 2020 6669 6c65  lf,.        file
-00013fd0: 7061 7468 3a20 7374 722c 0a20 2020 2020  path: str,.     
-00013fe0: 2020 206c 6179 6572 5f73 7461 636b 3a20     layer_stack: 
-00013ff0: 4f70 7469 6f6e 616c 5b4c 6179 6572 5374  Optional[LayerSt
-00014000: 6163 6b5d 203d 204e 6f6e 652c 0a20 2020  ack] = None,.   
-00014010: 2020 2020 2065 7863 6c75 6465 5f6c 6179       exclude_lay
-00014020: 6572 733a 204f 7074 696f 6e61 6c5b 5475  ers: Optional[Tu
-00014030: 706c 655b 4c61 7965 722c 202e 2e2e 5d5d  ple[Layer, ...]]
-00014040: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
-00014050: 3e20 6e70 2e6e 6461 7272 6179 3a0a 2020  > np.ndarray:.  
-00014060: 2020 2020 2020 2222 2257 7269 7465 2061        """Write a
-00014070: 2043 6f6d 706f 6e65 6e74 2074 6f20 5354   Component to ST
-00014080: 4c20 666f 7220 3344 2070 7269 6e74 696e  L for 3D printin
-00014090: 672e 0a0a 2020 2020 2020 2020 4172 6773  g...        Args
-000140a0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-000140b0: 6c65 7061 7468 3a20 746f 2077 7269 7465  lepath: to write
-000140c0: 2053 544c 2074 6f2e 0a20 2020 2020 2020   STL to..       
-000140d0: 2020 2020 206c 6179 6572 5f73 7461 636b       layer_stack
-000140e0: 3a20 636f 6e74 6169 6e73 2074 6869 636b  : contains thick
-000140f0: 6e65 7373 2061 6e64 207a 6d69 6e20 666f  ness and zmin fo
-00014100: 7220 6561 6368 206c 6179 6572 2e0a 2020  r each layer..  
-00014110: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
-00014120: 655f 6c61 7965 7273 3a20 6c61 7965 7273  e_layers: layers
-00014130: 2074 6f20 6578 636c 7564 652e 0a20 2020   to exclude..   
-00014140: 2020 2020 2020 2020 2075 7365 5f6c 6179           use_lay
-00014150: 6572 5f6e 616d 653a 2049 6620 5472 7565  er_name: If True
-00014160: 2c20 7573 6573 204c 6179 6572 4c65 7665  , uses LayerLeve
-00014170: 6c20 6e61 6d65 7320 696e 206f 7574 7075  l names in outpu
-00014180: 7420 6669 6c65 6e61 6d65 7320 7261 7468  t filenames rath
-00014190: 6572 2074 6861 6e20 6764 735f 6c61 7965  er than gds_laye
-000141a0: 7220 616e 6420 6764 735f 6461 7461 7479  r and gds_dataty
-000141b0: 7065 2e0a 2020 2020 2020 2020 2020 2020  pe..            
-000141c0: 6875 6c6c 5f69 6e76 616c 6964 5f70 6f6c  hull_invalid_pol
-000141d0: 7967 6f6e 733a 2049 6620 5472 7565 2c20  ygons: If True, 
-000141e0: 7265 706c 6163 6573 2069 6e76 616c 6964  replaces invalid
-000141f0: 2070 6f6c 7967 6f6e 7320 2864 6574 6572   polygons (deter
-00014200: 6d69 6e65 6420 6279 2073 6861 7065 6c79  mined by shapely
-00014210: 2e50 6f6c 7967 6f6e 2e69 735f 7661 6c69  .Polygon.is_vali
-00014220: 6429 2077 6974 6820 6974 7320 636f 6e76  d) with its conv
-00014230: 6578 2068 756c 6c2e 0a20 2020 2020 2020  ex hull..       
-00014240: 2020 2020 2073 6361 6c65 3a20 4f70 7469       scale: Opti
-00014250: 6f6e 616c 2066 6163 746f 7220 6279 2077  onal factor by w
-00014260: 6869 6368 2074 6f20 7363 616c 6520 6d65  hich to scale me
-00014270: 7368 6573 2062 6566 6f72 6520 7772 6974  shes before writ
-00014280: 696e 672e 0a0a 2020 2020 2020 2020 2222  ing...        ""
-00014290: 220a 2020 2020 2020 2020 6672 6f6d 2067  ".        from g
-000142a0: 6473 6661 6374 6f72 792e 6578 706f 7274  dsfactory.export
-000142b0: 2e74 6f5f 7374 6c20 696d 706f 7274 2074  .to_stl import t
-000142c0: 6f5f 7374 6c0a 0a20 2020 2020 2020 2072  o_stl..        r
-000142d0: 6574 7572 6e20 746f 5f73 746c 280a 2020  eturn to_stl(.  
-000142e0: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
-000142f0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00014300: 7061 7468 3d66 696c 6570 6174 682c 0a20  path=filepath,. 
-00014310: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-00014320: 5f73 7461 636b 3d6c 6179 6572 5f73 7461  _stack=layer_sta
-00014330: 636b 2c0a 2020 2020 2020 2020 2020 2020  ck,.            
-00014340: 6578 636c 7564 655f 6c61 7965 7273 3d65  exclude_layers=e
-00014350: 7863 6c75 6465 5f6c 6179 6572 732c 0a20  xclude_layers,. 
-00014360: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00014370: 6620 746f 5f67 6d73 6828 0a20 2020 2020  f to_gmsh(.     
-00014380: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00014390: 2074 7970 652c 0a20 2020 2020 2020 207a   type,.        z
-000143a0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2078  =None,.        x
-000143b0: 7365 6374 696f 6e5f 626f 756e 6473 3d4e  section_bounds=N
-000143c0: 6f6e 652c 0a20 2020 2020 2020 206c 6179  one,.        lay
-000143d0: 6572 5f73 7461 636b 3d4e 6f6e 652c 0a20  er_stack=None,. 
-000143e0: 2020 2020 2020 2077 6166 6572 5f70 6164         wafer_pad
-000143f0: 6469 6e67 3d30 2e30 2c0a 2020 2020 2020  ding=0.0,.      
-00014400: 2020 7761 6665 725f 6c61 7965 723d 4c41    wafer_layer=LA
-00014410: 5945 522e 5741 4645 522c 0a20 2020 2020  YER.WAFER,.     
-00014420: 2020 202a 6172 6773 2c0a 2020 2020 2020     *args,.      
-00014430: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
-00014440: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-00014450: 7475 726e 7320 6120 676d 7368 206d 7368  turns a gmsh msh
-00014460: 206f 6620 7468 6520 636f 6d70 6f6e 656e   of the componen
-00014470: 7420 666f 7220 6669 6e69 7465 2065 6c65  t for finite ele
-00014480: 6d65 6e74 2073 696d 756c 6174 696f 6e2e  ment simulation.
-00014490: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
-000144a0: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
-000144b0: 2074 7970 653a 206f 6e65 206f 6620 2278   type: one of "x
-000144c0: 7922 2c20 2275 7a22 2c20 6f72 2022 3344  y", "uz", or "3D
-000144d0: 222e 2044 6574 6572 6d69 6e65 7320 7468  ". Determines th
-000144e0: 6520 7479 7065 206f 6620 6d65 7368 2074  e type of mesh t
-000144f0: 6f20 7265 7475 726e 2e0a 2020 2020 2020  o return..      
-00014500: 2020 2020 2020 7a3a 2075 7365 6420 746f        z: used to
-00014510: 2064 6566 696e 6520 7a2d 736c 6963 6520   define z-slice 
-00014520: 666f 7220 7879 206d 6573 6869 6e67 0a20  for xy meshing. 
-00014530: 2020 2020 2020 2020 2020 2078 7365 6374             xsect
-00014540: 696f 6e5f 626f 756e 6473 3a20 7573 6564  ion_bounds: used
-00014550: 2074 6f20 6465 6669 6e65 2069 6e2d 706c   to define in-pl
-00014560: 616e 6520 6c69 6e65 2066 6f72 2075 7a20  ane line for uz 
-00014570: 6d65 7368 696e 670a 2020 2020 2020 2020  meshing.        
-00014580: 2020 2020 7761 6665 725f 7061 6464 696e      wafer_paddin
-00014590: 673a 2070 6164 6469 6e67 2062 6579 6f6e  g: padding beyon
-000145a0: 6420 6262 6f78 2074 6f20 6164 6420 746f  d bbox to add to
-000145b0: 2057 4146 4552 206c 6179 6572 732e 0a0a   WAFER layers...
-000145c0: 2020 2020 2020 2020 4b65 7977 6f72 6420          Keyword 
-000145d0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-000145e0: 2020 4172 6775 6d65 6e74 7320 666f 7220    Arguments for 
-000145f0: 7468 6520 7461 7267 6574 206d 6573 6869  the target meshi
-00014600: 6e67 2066 756e 6374 696f 6e20 696e 2067  ng function in g
-00014610: 6473 6661 6374 6f72 792e 7369 6d75 6c61  dsfactory.simula
-00014620: 7469 6f6e 2e67 6d73 680a 2020 2020 2020  tion.gmsh.      
-00014630: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-00014640: 4164 6420 5741 4645 5220 6c61 7965 723a  Add WAFER layer:
-00014650: 0a20 2020 2020 2020 2070 6164 6465 645f  .        padded_
-00014660: 636f 6d70 6f6e 656e 7420 3d20 436f 6d70  component = Comp
-00014670: 6f6e 656e 7428 290a 2020 2020 2020 2020  onent().        
-00014680: 7061 6464 6564 5f63 6f6d 706f 6e65 6e74  padded_component
-00014690: 203c 3c20 7365 6c66 0a20 2020 2020 2020   << self.       
-000146a0: 2028 786d 696e 2c20 796d 696e 292c 2028   (xmin, ymin), (
-000146b0: 786d 6178 2c20 796d 6178 2920 3d20 7365  xmax, ymax) = se
-000146c0: 6c66 2e62 626f 780a 2020 2020 2020 2020  lf.bbox.        
-000146d0: 706f 696e 7473 203d 205b 0a20 2020 2020  points = [.     
-000146e0: 2020 2020 2020 205b 786d 696e 202d 2077         [xmin - w
-000146f0: 6166 6572 5f70 6164 6469 6e67 2c20 796d  afer_padding, ym
-00014700: 696e 202d 2077 6166 6572 5f70 6164 6469  in - wafer_paddi
-00014710: 6e67 5d2c 0a20 2020 2020 2020 2020 2020  ng],.           
-00014720: 205b 786d 6178 202b 2077 6166 6572 5f70   [xmax + wafer_p
-00014730: 6164 6469 6e67 2c20 796d 696e 202d 2077  adding, ymin - w
-00014740: 6166 6572 5f70 6164 6469 6e67 5d2c 0a20  afer_padding],. 
-00014750: 2020 2020 2020 2020 2020 205b 786d 6178             [xmax
-00014760: 202b 2077 6166 6572 5f70 6164 6469 6e67   + wafer_padding
-00014770: 2c20 796d 6178 202b 2077 6166 6572 5f70  , ymax + wafer_p
-00014780: 6164 6469 6e67 5d2c 0a20 2020 2020 2020  adding],.       
-00014790: 2020 2020 205b 786d 696e 202d 2077 6166       [xmin - waf
-000147a0: 6572 5f70 6164 6469 6e67 2c20 796d 6178  er_padding, ymax
-000147b0: 202b 2077 6166 6572 5f70 6164 6469 6e67   + wafer_padding
-000147c0: 5d2c 0a20 2020 2020 2020 205d 0a20 2020  ],.        ].   
-000147d0: 2020 2020 2070 6164 6465 645f 636f 6d70       padded_comp
-000147e0: 6f6e 656e 742e 6164 645f 706f 6c79 676f  onent.add_polygo
-000147f0: 6e28 706f 696e 7473 2c20 6c61 7965 723d  n(points, layer=
-00014800: 7761 6665 725f 6c61 7965 7229 0a0a 2020  wafer_layer)..  
-00014810: 2020 2020 2020 6966 206c 6179 6572 5f73        if layer_s
-00014820: 7461 636b 2069 7320 4e6f 6e65 3a0a 2020  tack is None:.  
-00014830: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00014840: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00014850: 2020 2020 2020 2020 2020 2020 2741 204c              'A L
-00014860: 6179 6572 5374 6163 6b20 6d75 7374 2062  ayerStack must b
-00014870: 6520 7072 6f76 6964 6564 2074 6872 6f75  e provided throu
-00014880: 6768 2061 7267 756d 656e 7420 226c 6179  gh argument "lay
-00014890: 6572 5f73 7461 636b 222e 270a 2020 2020  er_stack".'.    
-000148a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000148b0: 2020 6966 2074 7970 6520 3d3d 2022 7879    if type == "xy
-000148c0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
-000148d0: 6620 7a20 6973 204e 6f6e 653a 0a20 2020  f z is None:.   
-000148e0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-000148f0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014910: 2020 2027 466f 7220 7879 2d6d 6573 6869     'For xy-meshi
-00014920: 6e67 2c20 6120 7a2d 7661 6c75 6520 6d75  ng, a z-value mu
-00014930: 7374 2062 6520 7072 6f76 6964 6564 2076  st be provided v
-00014940: 6961 2074 6865 2066 6c6f 6174 2061 7267  ia the float arg
-00014950: 756d 656e 7420 227a 222e 270a 2020 2020  ument "z".'.    
-00014960: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00014970: 2020 2020 2020 2020 2020 6672 6f6d 2067            from g
-00014980: 6473 6661 6374 6f72 792e 7369 6d75 6c61  dsfactory.simula
-00014990: 7469 6f6e 2e67 6d73 682e 7879 5f78 7365  tion.gmsh.xy_xse
-000149a0: 6374 696f 6e5f 6d65 7368 2069 6d70 6f72  ction_mesh impor
-000149b0: 7420 7879 5f78 7365 6374 696f 6e5f 6d65  t xy_xsection_me
-000149c0: 7368 0a0a 2020 2020 2020 2020 2020 2020  sh..            
-000149d0: 7265 7475 726e 2078 795f 7873 6563 7469  return xy_xsecti
-000149e0: 6f6e 5f6d 6573 6828 7061 6464 6564 5f63  on_mesh(padded_c
-000149f0: 6f6d 706f 6e65 6e74 2c20 7a2c 206c 6179  omponent, z, lay
-00014a00: 6572 5f73 7461 636b 2c20 2a2a 6b77 6172  er_stack, **kwar
-00014a10: 6773 290a 2020 2020 2020 2020 656c 6966  gs).        elif
-00014a20: 2074 7970 6520 3d3d 2022 757a 223a 0a20   type == "uz":. 
-00014a30: 2020 2020 2020 2020 2020 2069 6620 7873             if xs
-00014a40: 6563 7469 6f6e 5f62 6f75 6e64 7320 6973  ection_bounds is
-00014a50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00014a60: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00014a70: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-00014a80: 2020 2020 2020 2020 2020 2020 2022 466f               "Fo
-00014a90: 7220 757a 2d6d 6573 6869 6e67 2c20 796f  r uz-meshing, yo
-00014aa0: 7520 6d75 7374 2070 726f 7669 6465 2061  u must provide a
-00014ab0: 206c 696e 6520 696e 2074 6865 2078 792d   line in the xy-
-00014ac0: 706c 616e 6520 220a 2020 2020 2020 2020  plane ".        
-00014ad0: 2020 2020 2020 2020 2020 2020 2276 6961              "via
-00014ae0: 2074 6865 2054 7570 6c65 2061 7267 756d   the Tuple argum
-00014af0: 656e 7420 5b5b 7831 2c79 315d 2c20 5b78  ent [[x1,y1], [x
-00014b00: 322c 7932 5d5d 2078 7365 6374 696f 6e5f  2,y2]] xsection_
-00014b10: 626f 756e 6473 2e22 0a20 2020 2020 2020  bounds.".       
-00014b20: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00014b30: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
-00014b40: 6163 746f 7279 2e73 696d 756c 6174 696f  actory.simulatio
-00014b50: 6e2e 676d 7368 2e75 7a5f 7873 6563 7469  n.gmsh.uz_xsecti
-00014b60: 6f6e 5f6d 6573 6820 696d 706f 7274 2075  on_mesh import u
-00014b70: 7a5f 7873 6563 7469 6f6e 5f6d 6573 680a  z_xsection_mesh.
-00014b80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00014b90: 7572 6e20 757a 5f78 7365 6374 696f 6e5f  urn uz_xsection_
-00014ba0: 6d65 7368 280a 2020 2020 2020 2020 2020  mesh(.          
-00014bb0: 2020 2020 2020 7061 6464 6564 5f63 6f6d        padded_com
-00014bc0: 706f 6e65 6e74 2c20 7873 6563 7469 6f6e  ponent, xsection
-00014bd0: 5f62 6f75 6e64 732c 206c 6179 6572 5f73  _bounds, layer_s
-00014be0: 7461 636b 2c20 2a2a 6b77 6172 6773 0a20  tack, **kwargs. 
-00014bf0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00014c00: 2020 2020 2065 6c69 6620 7479 7065 203d       elif type =
-00014c10: 3d20 2233 4422 3a0a 2020 2020 2020 2020  = "3D":.        
-00014c20: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
-00014c30: 6f72 792e 7369 6d75 6c61 7469 6f6e 2e67  ory.simulation.g
-00014c40: 6d73 682e 7879 7a5f 6d65 7368 2069 6d70  msh.xyz_mesh imp
-00014c50: 6f72 7420 7879 7a5f 6d65 7368 0a0a 2020  ort xyz_mesh..  
-00014c60: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014c70: 2078 797a 5f6d 6573 6828 7061 6464 6564   xyz_mesh(padded
-00014c80: 5f63 6f6d 706f 6e65 6e74 2c20 6c61 7965  _component, laye
-00014c90: 725f 7374 6163 6b2c 202a 2a6b 7761 7267  r_stack, **kwarg
-00014ca0: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
-00014cb0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00014cc0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-00014cd0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00014ce0: 5265 7175 6972 6564 2061 7267 756d 656e  Required argumen
-00014cf0: 7420 2274 7970 6522 206d 7573 7420 6265  t "type" must be
-00014d00: 206f 6e65 206f 6620 2278 7922 2c20 2275   one of "xy", "u
-00014d10: 7a22 2c20 6f72 2022 3344 222e 270a 2020  z", or "3D".'.  
-00014d20: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00014d30: 2064 6566 206f 6666 7365 7428 0a20 2020   def offset(.   
-00014d40: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00014d50: 2020 2064 6973 7461 6e63 653a 2066 6c6f     distance: flo
-00014d60: 6174 203d 2030 2e31 2c0a 2020 2020 2020  at = 0.1,.      
-00014d70: 2020 706f 6c79 676f 6e73 3d4e 6f6e 652c    polygons=None,
-00014d80: 0a20 2020 2020 2020 2075 7365 5f75 6e69  .        use_uni
-00014d90: 6f6e 3a20 626f 6f6c 203d 2054 7275 652c  on: bool = True,
-00014da0: 0a20 2020 2020 2020 2070 7265 6369 7369  .        precisi
-00014db0: 6f6e 3a20 666c 6f61 7420 3d20 3165 2d34  on: float = 1e-4
-00014dc0: 2c0a 2020 2020 2020 2020 6a6f 696e 3a20  ,.        join: 
-00014dd0: 7374 7220 3d20 226d 6974 6572 222c 0a20  str = "miter",. 
-00014de0: 2020 2020 2020 2074 6f6c 6572 616e 6365         tolerance
-00014df0: 3a20 696e 7420 3d20 322c 0a20 2020 2020  : int = 2,.     
-00014e00: 2020 206c 6179 6572 3a20 4c61 7965 7253     layer: LayerS
-00014e10: 7065 6320 3d20 2257 4722 2c0a 2020 2020  pec = "WG",.    
-00014e20: 2920 2d3e 2043 6f6d 706f 6e65 6e74 3a0a  ) -> Component:.
-00014e30: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00014e40: 6e73 206e 6577 2043 6f6d 706f 6e65 6e74  ns new Component
-00014e50: 2077 6974 6820 706f 6c79 676f 6e73 2065   with polygons e
-00014e60: 726f 6465 6420 6f72 2064 696c 6174 6564  roded or dilated
-00014e70: 2062 7920 616e 206f 6666 7365 742e 0a0a   by an offset...
-00014e80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00014e90: 2020 2020 2020 2020 2020 6469 7374 616e            distan
-00014ea0: 6365 3a20 4469 7374 616e 6365 2074 6f20  ce: Distance to 
-00014eb0: 6f66 6673 6574 2070 6f6c 7967 6f6e 732e  offset polygons.
-00014ec0: 2050 6f73 6974 6976 6520 7661 6c75 6573   Positive values
-00014ed0: 2065 7870 616e 642c 206e 6567 6174 6976   expand, negativ
-00014ee0: 6520 7368 7269 6e6b 2e0a 2020 2020 2020  e shrink..      
-00014ef0: 2020 2020 2020 7072 6563 6973 696f 6e3a        precision:
-00014f00: 2044 6573 6972 6564 2070 7265 6369 7369   Desired precisi
-00014f10: 6f6e 2066 6f72 2072 6f75 6e64 696e 6720  on for rounding 
-00014f20: 7665 7274 6578 2063 6f6f 7264 696e 6174  vertex coordinat
-00014f30: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-00014f40: 6a6f 696e 3a20 7b27 6d69 7465 7227 2c20  join: {'miter', 
-00014f50: 2762 6576 656c 272c 2027 726f 756e 6427  'bevel', 'round'
-00014f60: 7d20 5479 7065 206f 6620 6a6f 696e 2075  } Type of join u
-00014f70: 7365 6420 746f 2063 7265 6174 6520 706f  sed to create po
-00014f80: 6c79 676f 6e20 6f66 6673 6574 0a20 2020  lygon offset.   
-00014f90: 2020 2020 2020 2020 2074 6f6c 6572 616e           toleran
-00014fa0: 6365 3a20 466f 7220 6d69 7465 7220 6a6f  ce: For miter jo
-00014fb0: 696e 7473 2c20 7468 6973 206e 756d 6265  ints, this numbe
-00014fc0: 7220 6d75 7374 2062 6520 6174 206c 6561  r must be at lea
-00014fd0: 7374 2032 2072 6570 7265 7365 6e74 7320  st 2 represents 
-00014fe0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00014ff0: 2020 6d61 7869 6d61 6c20 6469 7374 616e    maximal distan
-00015000: 6365 2069 6e20 6d75 6c74 6970 6c65 7320  ce in multiples 
-00015010: 6f66 206f 6666 7365 7420 6265 7477 6565  of offset betwee
-00015020: 6e20 6e65 7720 7665 7274 6963 6573 2061  n new vertices a
-00015030: 6e64 2074 6865 6972 0a20 2020 2020 2020  nd their.       
-00015040: 2020 2020 2020 206f 7269 6769 6e61 6c20         original 
-00015050: 706f 7369 7469 6f6e 2062 6566 6f72 6520  position before 
-00015060: 6265 7665 6c69 6e67 2074 6f20 6176 6f69  beveling to avoi
-00015070: 6420 7370 696b 6573 2061 7420 6163 7574  d spikes at acut
-00015080: 6520 6a6f 696e 7473 2e20 466f 720a 2020  e joints. For.  
-00015090: 2020 2020 2020 2020 2020 2020 726f 756e              roun
-000150a0: 6420 6a6f 696e 7473 2c20 6974 2069 6e64  d joints, it ind
-000150b0: 6963 6174 6573 2074 6865 2063 7572 7661  icates the curva
-000150c0: 7475 7265 2072 6573 6f6c 7574 696f 6e20  ture resolution 
-000150d0: 696e 206e 756d 6265 7220 6f66 0a20 2020  in number of.   
-000150e0: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
-000150f0: 7320 7065 7220 6675 6c6c 2063 6972 636c  s per full circl
-00015100: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
-00015110: 6179 6572 3a20 5370 6563 6966 6963 206c  ayer: Specific l
-00015120: 6179 6572 2066 6f72 206e 6577 2070 6f6c  ayer for new pol
-00015130: 7967 6f6e 732e 0a0a 2020 2020 2020 2020  ygons...        
-00015140: 2222 220a 2020 2020 2020 2020 696d 706f  """.        impo
-00015150: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
-00015160: 2067 660a 0a20 2020 2020 2020 2067 6473   gf..        gds
-00015170: 5f6c 6179 6572 2c20 6764 735f 6461 7461  _layer, gds_data
-00015180: 7479 7065 203d 2067 662e 6765 745f 6c61  type = gf.get_la
-00015190: 7965 7228 6c61 7965 7229 0a20 2020 2020  yer(layer).     
-000151a0: 2020 2070 203d 2067 6473 746b 2e6f 6666     p = gdstk.off
-000151b0: 7365 7428 0a20 2020 2020 2020 2020 2020  set(.           
-000151c0: 2070 6f6c 7967 6f6e 7320 6f72 2073 656c   polygons or sel
-000151d0: 662e 6765 745f 706f 6c79 676f 6e73 2829  f.get_polygons()
-000151e0: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
-000151f0: 7374 616e 6365 3d64 6973 7461 6e63 652c  stance=distance,
-00015200: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
-00015210: 6e3d 6a6f 696e 2c0a 2020 2020 2020 2020  n=join,.        
-00015220: 2020 2020 746f 6c65 7261 6e63 653d 746f      tolerance=to
-00015230: 6c65 7261 6e63 652c 0a20 2020 2020 2020  lerance,.       
-00015240: 2020 2020 2070 7265 6369 7369 6f6e 3d70       precision=p
-00015250: 7265 6369 7369 6f6e 2c0a 2020 2020 2020  recision,.      
-00015260: 2020 2020 2020 7573 655f 756e 696f 6e3d        use_union=
-00015270: 7573 655f 756e 696f 6e2c 0a20 2020 2020  use_union,.     
-00015280: 2020 2020 2020 206c 6179 6572 3d67 6473         layer=gds
-00015290: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
-000152a0: 2020 2020 6461 7461 7479 7065 3d67 6473      datatype=gds
-000152b0: 5f64 6174 6174 7970 652c 0a20 2020 2020  _datatype,.     
-000152c0: 2020 2029 0a0a 2020 2020 2020 2020 636f     )..        co
-000152d0: 6d70 6f6e 656e 7420 3d20 6766 2e43 6f6d  mponent = gf.Com
-000152e0: 706f 6e65 6e74 2829 0a20 2020 2020 2020  ponent().       
-000152f0: 2063 6f6d 706f 6e65 6e74 2e61 6464 5f70   component.add_p
-00015300: 6f6c 7967 6f6e 2870 2c20 6c61 7965 723d  olygon(p, layer=
-00015310: 6c61 7965 7229 0a20 2020 2020 2020 2072  layer).        r
-00015320: 6574 7572 6e20 636f 6d70 6f6e 656e 740a  eturn component.
-00015330: 0a0a 6465 6620 636f 7079 280a 2020 2020  ..def copy(.    
-00015340: 443a 2043 6f6d 706f 6e65 6e74 2c0a 2020  D: Component,.  
-00015350: 2020 7265 6665 7265 6e63 6573 3d4e 6f6e    references=Non
-00015360: 652c 0a20 2020 2070 6f72 7473 3d4e 6f6e  e,.    ports=Non
-00015370: 652c 0a20 2020 2070 6f6c 7967 6f6e 733d  e,.    polygons=
-00015380: 4e6f 6e65 2c0a 2020 2020 7061 7468 733d  None,.    paths=
-00015390: 4e6f 6e65 2c0a 2020 2020 6e61 6d65 3d4e  None,.    name=N
-000153a0: 6f6e 652c 0a20 2020 206c 6162 656c 733d  one,.    labels=
-000153b0: 4e6f 6e65 2c0a 2920 2d3e 2043 6f6d 706f  None,.) -> Compo
-000153c0: 6e65 6e74 3a0a 2020 2020 2222 2252 6574  nent:.    """Ret
-000153d0: 7572 6e73 2061 2043 6f6d 706f 6e65 6e74  urns a Component
-000153e0: 2063 6f70 792e 0a0a 2020 2020 4172 6773   copy...    Args
-000153f0: 3a0a 2020 2020 2020 2020 443a 2063 6f6d  :.        D: com
-00015400: 706f 6e65 6e74 2074 6f20 636f 7079 2e0a  ponent to copy..
-00015410: 2020 2020 2222 220a 2020 2020 445f 636f      """.    D_co
-00015420: 7079 203d 2043 6f6d 706f 6e65 6e74 2829  py = Component()
-00015430: 0a20 2020 2044 5f63 6f70 792e 696e 666f  .    D_copy.info
-00015440: 203d 2044 2e69 6e66 6f0a 2020 2020 2320   = D.info.    # 
-00015450: 445f 636f 7079 2e5f 6365 6c6c 203d 2044  D_copy._cell = D
-00015460: 2e5f 6365 6c6c 2e63 6f70 7928 6e61 6d65  ._cell.copy(name
-00015470: 3d44 5f63 6f70 792e 6e61 6d65 290a 0a20  =D_copy.name).. 
-00015480: 2020 2066 6f72 2072 6566 2069 6e20 7265     for ref in re
-00015490: 6665 7265 6e63 6573 2069 6620 7265 6665  ferences if refe
-000154a0: 7265 6e63 6573 2069 7320 6e6f 7420 4e6f  rences is not No
-000154b0: 6e65 2065 6c73 6520 442e 7265 6665 7265  ne else D.refere
-000154c0: 6e63 6573 3a0a 2020 2020 2020 2020 445f  nces:.        D_
-000154d0: 636f 7079 2e61 6464 2863 6f70 795f 7265  copy.add(copy_re
-000154e0: 6665 7265 6e63 6528 7265 6629 290a 2020  ference(ref)).  
-000154f0: 2020 666f 7220 706f 7274 2069 6e20 2870    for port in (p
-00015500: 6f72 7473 2069 6620 706f 7274 7320 6973  orts if ports is
-00015510: 206e 6f74 204e 6f6e 6520 656c 7365 2044   not None else D
-00015520: 2e70 6f72 7473 292e 7661 6c75 6573 2829  .ports).values()
-00015530: 3a0a 2020 2020 2020 2020 445f 636f 7079  :.        D_copy
-00015540: 2e61 6464 5f70 6f72 7428 706f 7274 3d70  .add_port(port=p
-00015550: 6f72 7429 0a20 2020 2066 6f72 2070 6f6c  ort).    for pol
-00015560: 7920 696e 2070 6f6c 7967 6f6e 7320 6966  y in polygons if
-00015570: 2070 6f6c 7967 6f6e 7320 6973 206e 6f74   polygons is not
-00015580: 204e 6f6e 6520 656c 7365 2044 2e70 6f6c   None else D.pol
-00015590: 7967 6f6e 733a 0a20 2020 2020 2020 2044  ygons:.        D
-000155a0: 5f63 6f70 792e 6164 645f 706f 6c79 676f  _copy.add_polygo
-000155b0: 6e28 706f 6c79 290a 2020 2020 666f 7220  n(poly).    for 
-000155c0: 7061 7468 2069 6e20 7061 7468 7320 6966  path in paths if
-000155d0: 2070 6174 6873 2069 7320 6e6f 7420 4e6f   paths is not No
-000155e0: 6e65 2065 6c73 6520 442e 7061 7468 733a  ne else D.paths:
-000155f0: 0a20 2020 2020 2020 2044 5f63 6f70 792e  .        D_copy.
-00015600: 6164 6428 7061 7468 290a 2020 2020 666f  add(path).    fo
-00015610: 7220 6c61 6265 6c20 696e 206c 6162 656c  r label in label
-00015620: 7320 6966 206c 6162 656c 7320 6973 206e  s if labels is n
-00015630: 6f74 204e 6f6e 6520 656c 7365 2044 2e6c  ot None else D.l
-00015640: 6162 656c 733a 0a20 2020 2020 2020 2044  abels:.        D
-00015650: 5f63 6f70 792e 6164 645f 6c61 6265 6c28  _copy.add_label(
-00015660: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-00015670: 743d 6c61 6265 6c2e 7465 7874 2c0a 2020  t=label.text,.  
-00015680: 2020 2020 2020 2020 2020 706f 7369 7469            positi
-00015690: 6f6e 3d6c 6162 656c 2e6f 7269 6769 6e2c  on=label.origin,
-000156a0: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-000156b0: 6572 3d28 6c61 6265 6c2e 6c61 7965 722c  er=(label.layer,
-000156c0: 206c 6162 656c 2e74 6578 7474 7970 6529   label.texttype)
-000156d0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-000156e0: 2069 6620 6e61 6d65 2069 7320 6e6f 7420   if name is not 
-000156f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 445f  None:.        D_
-00015700: 636f 7079 2e6e 616d 6520 3d20 6e61 6d65  copy.name = name
-00015710: 0a0a 2020 2020 7265 7475 726e 2044 5f63  ..    return D_c
-00015720: 6f70 790a 0a0a 6465 6620 636f 7079 5f72  opy...def copy_r
-00015730: 6566 6572 656e 6365 280a 2020 2020 7265  eference(.    re
-00015740: 662c 0a20 2020 2070 6172 656e 743d 4e6f  f,.    parent=No
-00015750: 6e65 2c0a 2020 2020 636f 6c75 6d6e 733d  ne,.    columns=
-00015760: 4e6f 6e65 2c0a 2020 2020 726f 7773 3d4e  None,.    rows=N
-00015770: 6f6e 652c 0a20 2020 2073 7061 6369 6e67  one,.    spacing
-00015780: 3d4e 6f6e 652c 0a20 2020 206f 7269 6769  =None,.    origi
-00015790: 6e3d 4e6f 6e65 2c0a 2020 2020 726f 7461  n=None,.    rota
-000157a0: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 206d  tion=None,.    m
-000157b0: 6167 6e69 6669 6361 7469 6f6e 3d4e 6f6e  agnification=Non
-000157c0: 652c 0a20 2020 2078 5f72 6566 6c65 6374  e,.    x_reflect
-000157d0: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 6e61  ion=None,.    na
-000157e0: 6d65 3d4e 6f6e 652c 0a20 2020 2076 313d  me=None,.    v1=
-000157f0: 4e6f 6e65 2c0a 2020 2020 7632 3d4e 6f6e  None,.    v2=Non
-00015800: 652c 0a29 202d 3e20 436f 6d70 6f6e 656e  e,.) -> Componen
-00015810: 7452 6566 6572 656e 6365 3a0a 2020 2020  tReference:.    
-00015820: 7265 7475 726e 2043 6f6d 706f 6e65 6e74  return Component
-00015830: 5265 6665 7265 6e63 6528 0a20 2020 2020  Reference(.     
-00015840: 2020 2063 6f6d 706f 6e65 6e74 3d70 6172     component=par
-00015850: 656e 7420 6f72 2072 6566 2e70 6172 656e  ent or ref.paren
-00015860: 742c 0a20 2020 2020 2020 2063 6f6c 756d  t,.        colum
-00015870: 6e73 3d63 6f6c 756d 6e73 206f 7220 7265  ns=columns or re
-00015880: 662e 636f 6c75 6d6e 732c 0a20 2020 2020  f.columns,.     
-00015890: 2020 2072 6f77 733d 726f 7773 206f 7220     rows=rows or 
-000158a0: 7265 662e 726f 7773 2c0a 2020 2020 2020  ref.rows,.      
-000158b0: 2020 7370 6163 696e 673d 7370 6163 696e    spacing=spacin
-000158c0: 6720 6f72 2072 6566 2e73 7061 6369 6e67  g or ref.spacing
-000158d0: 2c0a 2020 2020 2020 2020 6f72 6967 696e  ,.        origin
-000158e0: 3d6f 7269 6769 6e20 6f72 2072 6566 2e6f  =origin or ref.o
-000158f0: 7269 6769 6e2c 0a20 2020 2020 2020 2072  rigin,.        r
-00015900: 6f74 6174 696f 6e3d 726f 7461 7469 6f6e  otation=rotation
-00015910: 206f 7220 7265 662e 726f 7461 7469 6f6e   or ref.rotation
-00015920: 2c0a 2020 2020 2020 2020 6d61 676e 6966  ,.        magnif
-00015930: 6963 6174 696f 6e3d 6d61 676e 6966 6963  ication=magnific
-00015940: 6174 696f 6e20 6f72 2072 6566 2e6d 6167  ation or ref.mag
-00015950: 6e69 6669 6361 7469 6f6e 2c0a 2020 2020  nification,.    
-00015960: 2020 2020 785f 7265 666c 6563 7469 6f6e      x_reflection
-00015970: 3d78 5f72 6566 6c65 6374 696f 6e20 6f72  =x_reflection or
-00015980: 2072 6566 2e78 5f72 6566 6c65 6374 696f   ref.x_reflectio
-00015990: 6e2c 0a20 2020 2020 2020 206e 616d 653d  n,.        name=
-000159a0: 6e61 6d65 206f 7220 7265 662e 6e61 6d65  name or ref.name
-000159b0: 2c0a 2020 2020 2020 2020 7631 3d76 3120  ,.        v1=v1 
-000159c0: 6f72 2072 6566 2e76 312c 0a20 2020 2020  or ref.v1,.     
-000159d0: 2020 2076 323d 7632 206f 7220 7265 662e     v2=v2 or ref.
-000159e0: 7632 2c0a 2020 2020 290a 0a0a 6465 6620  v2,.    )...def 
-000159f0: 7465 7374 5f67 6574 5f6c 6179 6572 7328  test_get_layers(
-00015a00: 2920 2d3e 2043 6f6d 706f 6e65 6e74 3a0a  ) -> Component:.
-00015a10: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
-00015a20: 6374 6f72 7920 6173 2067 660a 0a20 2020  ctory as gf..   
-00015a30: 2063 3120 3d20 6766 2e63 6f6d 706f 6e65   c1 = gf.compone
-00015a40: 6e74 732e 7374 7261 6967 6874 280a 2020  nts.straight(.  
-00015a50: 2020 2020 2020 6c65 6e67 7468 3d31 302c        length=10,
-00015a60: 0a20 2020 2020 2020 2077 6964 7468 3d30  .        width=0
-00015a70: 2e35 2c0a 2020 2020 2020 2020 6c61 7965  .5,.        laye
-00015a80: 723d 2832 2c20 3029 2c0a 2020 2020 2020  r=(2, 0),.      
-00015a90: 2020 6262 6f78 5f6c 6179 6572 733d 5b28    bbox_layers=[(
-00015aa0: 3131 312c 2030 295d 2c0a 2020 2020 2020  111, 0)],.      
-00015ab0: 2020 6262 6f78 5f6f 6666 7365 7473 3d5b    bbox_offsets=[
-00015ac0: 335d 2c0a 2020 2020 2020 2020 7769 7468  3],.        with
-00015ad0: 5f62 626f 783d 5472 7565 2c0a 2020 2020  _bbox=True,.    
-00015ae0: 2020 2020 636c 6164 6469 6e67 5f6c 6179      cladding_lay
-00015af0: 6572 733d 4e6f 6e65 2c0a 2020 2020 2020  ers=None,.      
-00015b00: 2020 6164 645f 7069 6e73 3d4e 6f6e 652c    add_pins=None,
-00015b10: 0a20 2020 2020 2020 2061 6464 5f62 626f  .        add_bbo
-00015b20: 783d 4e6f 6e65 2c0a 2020 2020 290a 2020  x=None,.    ).  
-00015b30: 2020 6173 7365 7274 2063 312e 6765 745f    assert c1.get_
-00015b40: 6c61 7965 7273 2829 203d 3d20 7b28 322c  layers() == {(2,
-00015b50: 2030 292c 2028 3131 312c 2030 297d 2c20   0), (111, 0)}, 
-00015b60: 6331 2e67 6574 5f6c 6179 6572 7328 290a  c1.get_layers().
-00015b70: 2020 2020 2320 7265 7475 726e 2063 310a      # return c1.
-00015b80: 2020 2020 6332 203d 2063 312e 7265 6d6f      c2 = c1.remo
-00015b90: 7665 5f6c 6179 6572 7328 5b28 3131 312c  ve_layers([(111,
-00015ba0: 2030 295d 290a 2020 2020 6173 7365 7274   0)]).    assert
-00015bb0: 2063 322e 6765 745f 6c61 7965 7273 2829   c2.get_layers()
-00015bc0: 203d 3d20 7b28 322c 2030 297d 2c20 6332   == {(2, 0)}, c2
-00015bd0: 2e67 6574 5f6c 6179 6572 7328 290a 2020  .get_layers().  
-00015be0: 2020 7265 7475 726e 2063 320a 0a0a 6465    return c2...de
-00015bf0: 6620 5f66 696c 7465 725f 706f 6c79 7328  f _filter_polys(
-00015c00: 706f 6c79 676f 6e73 2c20 6c61 7965 7273  polygons, layers
-00015c10: 5f65 7863 6c29 3a0a 2020 2020 7265 7475  _excl):.    retu
-00015c20: 726e 205b 0a20 2020 2020 2020 2070 6f6c  rn [.        pol
-00015c30: 7967 6f6e 0a20 2020 2020 2020 2066 6f72  ygon.        for
-00015c40: 2070 6f6c 7967 6f6e 2c20 6c61 7965 722c   polygon, layer,
-00015c50: 2064 6174 6174 7970 6520 696e 207a 6970   datatype in zip
-00015c60: 280a 2020 2020 2020 2020 2020 2020 706f  (.            po
-00015c70: 6c79 676f 6e73 2e70 6f6c 7967 6f6e 732c  lygons.polygons,
-00015c80: 2070 6f6c 7967 6f6e 732e 6c61 7965 7273   polygons.layers
-00015c90: 2c20 706f 6c79 676f 6e73 2e64 6174 6174  , polygons.datat
-00015ca0: 7970 6573 0a20 2020 2020 2020 2029 0a20  ypes.        ). 
-00015cb0: 2020 2020 2020 2069 6620 286c 6179 6572         if (layer
-00015cc0: 2c20 6461 7461 7479 7065 2920 6e6f 7420  , datatype) not 
-00015cd0: 696e 206c 6179 6572 735f 6578 636c 0a20  in layers_excl. 
-00015ce0: 2020 205d 0a0a 0a64 6566 2072 6563 7572     ]...def recur
-00015cf0: 7365 5f73 7472 7563 7475 7265 7328 0a20  se_structures(. 
-00015d00: 2020 2063 6f6d 706f 6e65 6e74 3a20 436f     component: Co
-00015d10: 6d70 6f6e 656e 742c 0a20 2020 2069 676e  mponent,.    ign
-00015d20: 6f72 655f 636f 6d70 6f6e 656e 7473 5f70  ore_components_p
-00015d30: 7265 6669 783a 204f 7074 696f 6e61 6c5b  refix: Optional[
-00015d40: 4c69 7374 5b73 7472 5d5d 203d 204e 6f6e  List[str]] = Non
-00015d50: 652c 0a20 2020 2069 676e 6f72 655f 6675  e,.    ignore_fu
-00015d60: 6e63 7469 6f6e 735f 7072 6566 6978 3a20  nctions_prefix: 
-00015d70: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-00015d80: 725d 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  r]] = None,.) ->
-00015d90: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
-00015da0: 0a20 2020 2022 2222 5265 6375 7273 6520  .    """Recurse 
-00015db0: 636f 6d70 6f6e 656e 7420 616e 6420 636f  component and co
-00015dc0: 6d70 6f6e 656e 7473 2072 6566 6572 656e  mponents referen
-00015dd0: 6365 7320 7265 6375 7273 6976 656c 792e  ces recursively.
-00015de0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00015df0: 2020 2020 636f 6d70 6f6e 656e 743a 2063      component: c
-00015e00: 6f6d 706f 6e65 6e74 2074 6f20 7265 6375  omponent to recu
-00015e10: 7273 652e 0a20 2020 2020 2020 2069 676e  rse..        ign
-00015e20: 6f72 655f 636f 6d70 6f6e 656e 7473 5f70  ore_components_p
-00015e30: 7265 6669 783a 206c 6973 7420 6f66 2070  refix: list of p
-00015e40: 7265 6669 7820 746f 2069 676e 6f72 652e  refix to ignore.
-00015e50: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
-00015e60: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
-00015e70: 3a20 6c69 7374 206f 6620 7072 6566 6978  : list of prefix
-00015e80: 2074 6f20 6967 6e6f 7265 2e0a 2020 2020   to ignore..    
-00015e90: 2222 220a 2020 2020 6967 6e6f 7265 5f66  """.    ignore_f
-00015ea0: 756e 6374 696f 6e73 5f70 7265 6669 7820  unctions_prefix 
-00015eb0: 3d20 6967 6e6f 7265 5f66 756e 6374 696f  = ignore_functio
-00015ec0: 6e73 5f70 7265 6669 7820 6f72 205b 5d0a  ns_prefix or [].
-00015ed0: 2020 2020 6967 6e6f 7265 5f63 6f6d 706f      ignore_compo
-00015ee0: 6e65 6e74 735f 7072 6566 6978 203d 2069  nents_prefix = i
-00015ef0: 676e 6f72 655f 636f 6d70 6f6e 656e 7473  gnore_components
-00015f00: 5f70 7265 6669 7820 6f72 205b 5d0a 0a20  _prefix or [].. 
-00015f10: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-00015f20: 6861 7361 7474 7228 636f 6d70 6f6e 656e  hasattr(componen
-00015f30: 742c 2022 6675 6e63 7469 6f6e 5f6e 616d  t, "function_nam
-00015f40: 6522 290a 2020 2020 2020 2020 616e 6420  e").        and 
-00015f50: 636f 6d70 6f6e 656e 742e 6675 6e63 7469  component.functi
-00015f60: 6f6e 5f6e 616d 6520 696e 2069 676e 6f72  on_name in ignor
-00015f70: 655f 6675 6e63 7469 6f6e 735f 7072 6566  e_functions_pref
-00015f80: 6978 0a20 2020 2029 3a0a 2020 2020 2020  ix.    ):.      
-00015f90: 2020 7265 7475 726e 207b 7d0a 0a20 2020    return {}..   
-00015fa0: 2069 6620 6861 7361 7474 7228 636f 6d70   if hasattr(comp
-00015fb0: 6f6e 656e 742c 2022 6e61 6d65 2229 2061  onent, "name") a
-00015fc0: 6e64 2061 6e79 280a 2020 2020 2020 2020  nd any(.        
-00015fd0: 636f 6d70 6f6e 656e 742e 6e61 6d65 2e73  component.name.s
-00015fe0: 7461 7274 7377 6974 6828 6929 2066 6f72  tartswith(i) for
-00015ff0: 2069 2069 6e20 6967 6e6f 7265 5f63 6f6d   i in ignore_com
-00016000: 706f 6e65 6e74 735f 7072 6566 6978 0a20  ponents_prefix. 
-00016010: 2020 2029 3a0a 2020 2020 2020 2020 7265     ):.        re
-00016020: 7475 726e 207b 7d0a 0a20 2020 206f 7574  turn {}..    out
-00016030: 7075 7420 3d20 7b63 6f6d 706f 6e65 6e74  put = {component
-00016040: 2e6e 616d 653a 2064 6963 7428 636f 6d70  .name: dict(comp
-00016050: 6f6e 656e 742e 7365 7474 696e 6773 297d  onent.settings)}
-00016060: 0a20 2020 2066 6f72 2072 6566 6572 656e  .    for referen
-00016070: 6365 2069 6e20 636f 6d70 6f6e 656e 742e  ce in component.
-00016080: 7265 6665 7265 6e63 6573 3a0a 2020 2020  references:.    
-00016090: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-000160a0: 2020 2020 2069 7369 6e73 7461 6e63 6528       isinstance(
-000160b0: 7265 6665 7265 6e63 652c 2043 6f6d 706f  reference, Compo
-000160c0: 6e65 6e74 5265 6665 7265 6e63 6529 0a20  nentReference). 
-000160d0: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
-000160e0: 6566 6572 656e 6365 2e72 6566 5f63 656c  eference.ref_cel
-000160f0: 6c2e 6e61 6d65 206e 6f74 2069 6e20 6f75  l.name not in ou
-00016100: 7470 7574 0a20 2020 2020 2020 2029 3a0a  tput.        ):.
-00016110: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00016120: 7574 2e75 7064 6174 6528 7265 6375 7273  ut.update(recurs
-00016130: 655f 7374 7275 6374 7572 6573 2872 6566  e_structures(ref
-00016140: 6572 656e 6365 2e72 6566 5f63 656c 6c29  erence.ref_cell)
-00016150: 290a 0a20 2020 2072 6574 7572 6e20 6f75  )..    return ou
-00016160: 7470 7574 0a0a 0a64 6566 2066 6c61 7474  tput...def flatt
-00016170: 656e 5f69 6e76 616c 6964 5f72 6566 735f  en_invalid_refs_
-00016180: 7265 6375 7273 6976 6528 0a20 2020 2063  recursive(.    c
-00016190: 6f6d 706f 6e65 6e74 3a20 436f 6d70 6f6e  omponent: Compon
-000161a0: 656e 742c 0a20 2020 2067 7269 645f 7369  ent,.    grid_si
-000161b0: 7a65 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ze: Optional[flo
-000161c0: 6174 5d20 3d20 4e6f 6e65 2c0a 2020 2020  at] = None,.    
-000161d0: 7570 6461 7465 645f 636f 6d70 6f6e 656e  updated_componen
-000161e0: 7473 3d4e 6f6e 652c 0a20 2020 2074 7261  ts=None,.    tra
-000161f0: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
-00016200: 733d 4e6f 6e65 2c0a 293a 0a20 2020 2022  s=None,.):.    "
-00016210: 2222 5265 6375 7273 6976 656c 7920 666c  ""Recursively fl
-00016220: 6174 7465 6e73 2063 6f6d 706f 6e65 6e74  attens component
-00016230: 2072 6566 6572 656e 6365 7320 7768 6963   references whic
-00016240: 6820 6861 7665 2069 6e76 616c 6964 2074  h have invalid t
-00016250: 7261 6e73 666f 726d 6174 696f 6e73 2028  ransformations (
-00016260: 692e 652e 206e 6f6e 2d39 3020 6465 6720  i.e. non-90 deg 
-00016270: 726f 7461 7469 6f6e 7320 6f72 2073 7562  rotations or sub
-00016280: 2d67 7269 6420 7472 616e 736c 6174 696f  -grid translatio
-00016290: 6e73 2920 616e 6420 7265 7475 726e 7320  ns) and returns 
-000162a0: 6120 636f 7079 2069 6620 616e 7920 7375  a copy if any su
-000162b0: 6263 656c 6c73 2068 6176 6520 6265 656e  bcells have been
-000162c0: 206d 6f64 6966 6965 642e 0a0a 2020 2020   modified...    
-000162d0: 5741 524e 494e 473a 2074 6869 7320 6675  WARNING: this fu
-000162e0: 6e63 7469 6f6e 2077 696c 6c20 7072 6f64  nction will prod
-000162f0: 7563 6520 7361 6d65 2d6e 616d 6520 636f  uce same-name co
-00016300: 7069 6573 206f 6620 6365 6c6c 732e 2049  pies of cells. I
-00016310: 7420 6973 2073 7472 6963 746c 7920 6d65  t is strictly me
-00016320: 616e 7420 746f 2062 6520 7573 6564 206f  ant to be used o
-00016330: 6e20 7772 6974 6520 6f66 2074 6865 2047  n write of the G
-00016340: 4453 2066 696c 6520 616e 640a 2020 2020  DS file and.    
-00016350: 7368 6f75 6c64 206e 6f74 2062 6520 6d69  should not be mi
-00016360: 7865 6420 7769 7468 206f 7468 6572 2063  xed with other c
-00016370: 656c 6c73 2c20 6f72 2079 6f75 2077 696c  ells, or you wil
-00016380: 6c20 6c69 6b65 6c79 2065 7870 6572 6965  l likely experie
-00016390: 6e63 6520 6973 7375 6573 2077 6974 6820  nce issues with 
-000163a0: 6475 706c 6963 6174 6520 6365 6c6c 730a  duplicate cells.
-000163b0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-000163c0: 2020 2063 6f6d 706f 6e65 6e74 3a20 7468     component: th
-000163d0: 6520 636f 6d70 6f6e 656e 7420 746f 2066  e component to f
-000163e0: 6978 2028 696e 2070 6c61 6365 292e 0a20  ix (in place).. 
-000163f0: 2020 2020 2020 2067 7269 645f 7369 7a65         grid_size
-00016400: 3a20 7468 6520 4744 5320 6772 6964 2073  : the GDS grid s
-00016410: 697a 652c 2069 6e20 756d 2c20 6465 6661  ize, in um, defa
-00016420: 756c 7473 2074 6f20 6163 7469 7665 2050  ults to active P
-00016430: 444b 2e67 6574 5f67 7269 645f 7369 7a65  DK.get_grid_size
-00016440: 2829 0a20 2020 2020 2020 2020 2020 2061  ().            a
-00016450: 6e79 2074 7261 6e73 6c61 7469 6f6e 7320  ny translations 
-00016460: 7769 7468 2068 6967 6865 7220 7265 736f  with higher reso
-00016470: 6c75 7469 6f6e 2074 6861 6e20 7468 6973  lution than this
-00016480: 2061 7265 2063 6f6e 7369 6465 7265 6420   are considered 
-00016490: 696e 7661 6c69 642e 0a20 2020 2020 2020  invalid..       
-000164a0: 2075 7064 6174 6564 5f63 6f6d 706f 6e65   updated_compone
-000164b0: 6e74 733a 2074 6865 2072 756e 6e69 6e67  nts: the running
-000164c0: 2064 6963 7469 6f6e 6172 7920 6f66 2063   dictionary of c
-000164d0: 6f6d 706f 6e65 6e74 7320 7768 6963 6820  omponents which 
-000164e0: 6861 7665 2062 6565 6e20 6d6f 6469 6669  have been modifi
-000164f0: 6564 2062 7920 7468 6973 2074 7261 6e73  ed by this trans
-00016500: 666f 726d 6174 696f 6e2e 2053 686f 756c  formation. Shoul
-00016510: 6420 616c 7761 7973 2062 6520 4e6f 6e65  d always be None
-00016520: 2c20 6578 6365 7074 2066 6f72 2072 6563  , except for rec
-00016530: 7572 7369 7665 2069 6e76 6f63 6174 696f  ursive invocatio
-00016540: 6e73 2e0a 2020 2020 2020 2020 7472 6176  ns..        trav
-00016550: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
-00016560: 3a20 7468 6520 7365 7420 6f66 2063 6f6d  : the set of com
-00016570: 706f 6e65 6e74 206e 616d 6573 2077 6869  ponent names whi
-00016580: 6368 2068 6176 6520 6265 656e 2074 7261  ch have been tra
-00016590: 7665 7273 6564 2e20 5368 6f75 6c64 2061  versed. Should a
-000165a0: 6c77 6179 7320 6265 204e 6f6e 652c 2065  lways be None, e
-000165b0: 7863 6570 7420 666f 7220 7265 6375 7273  xcept for recurs
-000165c0: 6976 6520 696e 766f 6361 7469 6f6e 732e  ive invocations.
-000165d0: 0a20 2020 2022 2222 0a20 2020 2066 726f  .    """.    fro
-000165e0: 6d20 6764 7366 6163 746f 7279 2e64 6563  m gdsfactory.dec
-000165f0: 6f72 6174 6f72 7320 696d 706f 7274 2069  orators import i
-00016600: 735f 696e 7661 6c69 645f 7265 660a 0a20  s_invalid_ref.. 
-00016610: 2020 2069 6e76 616c 6964 5f72 6566 7320     invalid_refs 
-00016620: 3d20 5b5d 0a20 2020 2072 6566 7320 3d20  = [].    refs = 
-00016630: 636f 6d70 6f6e 656e 742e 7265 6665 7265  component.refere
-00016640: 6e63 6573 0a20 2020 2073 7562 6365 6c6c  nces.    subcell
-00016650: 5f6d 6f64 6966 6965 6420 3d20 4661 6c73  _modified = Fals
-00016660: 650a 2020 2020 6966 2075 7064 6174 6564  e.    if updated
-00016670: 5f63 6f6d 706f 6e65 6e74 7320 6973 204e  _components is N
-00016680: 6f6e 653a 0a20 2020 2020 2020 2075 7064  one:.        upd
-00016690: 6174 6564 5f63 6f6d 706f 6e65 6e74 7320  ated_components 
-000166a0: 3d20 7b7d 0a20 2020 2069 6620 7472 6176  = {}.    if trav
-000166b0: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
-000166c0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000166d0: 2020 7472 6176 6572 7365 645f 636f 6d70    traversed_comp
-000166e0: 6f6e 656e 7473 203d 2073 6574 2829 0a20  onents = set(). 
-000166f0: 2020 2066 6f72 2072 6566 2069 6e20 7265     for ref in re
-00016700: 6673 3a0a 2020 2020 2020 2020 2320 6d61  fs:.        # ma
-00016710: 726b 2061 6e79 2069 6e76 616c 6964 2072  rk any invalid r
-00016720: 6566 7320 666f 7220 666c 6174 7465 6e69  efs for flatteni
-00016730: 6e67 0a20 2020 2020 2020 2023 206f 7468  ng.        # oth
-00016740: 6572 7769 7365 2c20 6368 6563 6b20 6966  erwise, check if
-00016750: 2074 6865 7265 2061 7265 2061 6e79 206d   there are any m
-00016760: 6f64 6966 6965 6420 6365 6c6c 7320 6265  odified cells be
-00016770: 6e65 6174 6820 2877 6520 6e65 6564 206e  neath (we need n
-00016780: 6f74 2064 6f20 7468 6973 2069 6620 7468  ot do this if th
-00016790: 6520 7265 6620 7769 6c6c 2062 6520 666c  e ref will be fl
-000167a0: 6174 7465 6e65 6420 616e 7977 6179 7329  attened anyways)
-000167b0: 0a20 2020 2020 2020 2069 6620 6973 5f69  .        if is_i
-000167c0: 6e76 616c 6964 5f72 6566 2872 6566 2c20  nvalid_ref(ref, 
-000167d0: 6772 6964 5f73 697a 6529 3a0a 2020 2020  grid_size):.    
-000167e0: 2020 2020 2020 2020 696e 7661 6c69 645f          invalid_
-000167f0: 7265 6673 2e61 7070 656e 6428 7265 662e  refs.append(ref.
-00016800: 6e61 6d65 290a 2020 2020 2020 2020 656c  name).        el
-00016810: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00016820: 2320 6f74 6865 7277 6973 652c 2072 6563  # otherwise, rec
-00016830: 7572 7369 7665 6c79 2066 6c61 7474 656e  ursively flatten
-00016840: 2072 6566 7320 6966 2074 6865 2073 7562   refs if the sub
-00016850: 6365 6c6c 2068 6173 206e 6f74 2061 6c72  cell has not alr
-00016860: 6561 6479 2062 6565 6e20 7472 6176 6572  eady been traver
-00016870: 7365 640a 2020 2020 2020 2020 2020 2020  sed.            
-00016880: 6966 2072 6566 2e70 6172 656e 742e 6e61  if ref.parent.na
-00016890: 6d65 206e 6f74 2069 6e20 7472 6176 6572  me not in traver
-000168a0: 7365 645f 636f 6d70 6f6e 656e 7473 3a0a  sed_components:.
-000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168c0: 666c 6174 7465 6e5f 696e 7661 6c69 645f  flatten_invalid_
-000168d0: 7265 6673 5f72 6563 7572 7369 7665 280a  refs_recursive(.
-000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168f0: 2020 2020 7265 662e 7061 7265 6e74 2c0a      ref.parent,.
-00016900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016910: 2020 2020 6772 6964 5f73 697a 653d 6772      grid_size=gr
-00016920: 6964 5f73 697a 652c 0a20 2020 2020 2020  id_size,.       
-00016930: 2020 2020 2020 2020 2020 2020 2075 7064               upd
-00016940: 6174 6564 5f63 6f6d 706f 6e65 6e74 733d  ated_components=
-00016950: 7570 6461 7465 645f 636f 6d70 6f6e 656e  updated_componen
-00016960: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-00016970: 2020 2020 2020 2020 7472 6176 6572 7365          traverse
-00016980: 645f 636f 6d70 6f6e 656e 7473 3d74 7261  d_components=tra
-00016990: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
-000169a0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000169b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000169c0: 2023 206e 6f77 2c20 6966 2074 6865 2072   # now, if the r
-000169d0: 6566 2773 2063 656c 6c20 6265 656e 206d  ef's cell been m
-000169e0: 6f64 6966 6965 642c 206d 6172 6b20 6974  odified, mark it
-000169f0: 2061 7320 7375 6368 0a20 2020 2020 2020   as such.       
-00016a00: 2020 2020 2069 6620 7265 662e 7061 7265       if ref.pare
-00016a10: 6e74 2e6e 616d 6520 696e 2075 7064 6174  nt.name in updat
-00016a20: 6564 5f63 6f6d 706f 6e65 6e74 733a 0a20  ed_components:. 
-00016a30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016a40: 7562 6365 6c6c 5f6d 6f64 6966 6965 6420  ubcell_modified 
-00016a50: 3d20 5472 7565 0a20 2020 2069 6620 696e  = True.    if in
-00016a60: 7661 6c69 645f 7265 6673 206f 7220 7375  valid_refs or su
-00016a70: 6263 656c 6c5f 6d6f 6469 6669 6564 3a0a  bcell_modified:.
-00016a80: 2020 2020 2020 2020 6e65 775f 636f 6d70          new_comp
-00016a90: 6f6e 656e 7420 3d20 636f 6d70 6f6e 656e  onent = componen
-00016aa0: 742e 636f 7079 2829 0a20 2020 2020 2020  t.copy().       
-00016ab0: 206e 6577 5f63 6f6d 706f 6e65 6e74 2e6e   new_component.n
-00016ac0: 616d 6520 3d20 636f 6d70 6f6e 656e 742e  ame = component.
-00016ad0: 6e61 6d65 0a20 2020 2020 2020 2023 206d  name.        # m
-00016ae0: 616b 6520 7375 7265 2061 6c6c 206d 6f64  ake sure all mod
-00016af0: 6966 6965 6420 6365 6c6c 7320 6861 7665  ified cells have
-00016b00: 2074 6865 6972 2072 6566 6572 656e 6365   their reference
-00016b10: 7320 7570 6461 7465 640a 2020 2020 2020  s updated.      
-00016b20: 2020 6e65 775f 7265 6673 203d 206e 6577    new_refs = new
-00016b30: 5f63 6f6d 706f 6e65 6e74 2e72 6566 6572  _component.refer
-00016b40: 656e 6365 732e 636f 7079 2829 0a20 2020  ences.copy().   
-00016b50: 2020 2020 2066 6f72 2072 6566 2069 6e20       for ref in 
-00016b60: 6e65 775f 7265 6673 3a0a 2020 2020 2020  new_refs:.      
-00016b70: 2020 2020 2020 6966 2072 6566 2e6e 616d        if ref.nam
-00016b80: 6520 696e 2069 6e76 616c 6964 5f72 6566  e in invalid_ref
-00016b90: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00016ba0: 2020 206e 6577 5f63 6f6d 706f 6e65 6e74     new_component
-00016bb0: 2e66 6c61 7474 656e 5f72 6566 6572 656e  .flatten_referen
-00016bc0: 6365 2872 6566 290a 2020 2020 2020 2020  ce(ref).        
-00016bd0: 2020 2020 656c 6966 2028 0a20 2020 2020      elif (.     
-00016be0: 2020 2020 2020 2020 2020 2072 6566 2e70             ref.p
-00016bf0: 6172 656e 742e 6e61 6d65 2069 6e20 7570  arent.name in up
-00016c00: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
-00016c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016c20: 2061 6e64 2072 6566 2e70 6172 656e 7420   and ref.parent 
-00016c30: 6973 206e 6f74 2075 7064 6174 6564 5f63  is not updated_c
-00016c40: 6f6d 706f 6e65 6e74 735b 7265 662e 7061  omponents[ref.pa
-00016c50: 7265 6e74 2e6e 616d 655d 0a20 2020 2020  rent.name].     
-00016c60: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00016c70: 2020 2020 2020 2020 2020 7265 662e 7061            ref.pa
-00016c80: 7265 6e74 203d 2075 7064 6174 6564 5f63  rent = updated_c
-00016c90: 6f6d 706f 6e65 6e74 735b 7265 662e 7061  omponents[ref.pa
-00016ca0: 7265 6e74 2e6e 616d 655d 0a20 2020 2020  rent.name].     
-00016cb0: 2020 2063 6f6d 706f 6e65 6e74 203d 206e     component = n
-00016cc0: 6577 5f63 6f6d 706f 6e65 6e74 0a20 2020  ew_component.   
-00016cd0: 2020 2020 2075 7064 6174 6564 5f63 6f6d       updated_com
-00016ce0: 706f 6e65 6e74 735b 636f 6d70 6f6e 656e  ponents[componen
-00016cf0: 742e 6e61 6d65 5d20 3d20 6e65 775f 636f  t.name] = new_co
-00016d00: 6d70 6f6e 656e 740a 2020 2020 7472 6176  mponent.    trav
-00016d10: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
-00016d20: 2e61 6464 2863 6f6d 706f 6e65 6e74 2e6e  .add(component.n
-00016d30: 616d 6529 0a20 2020 2072 6574 7572 6e20  ame).    return 
-00016d40: 636f 6d70 6f6e 656e 740a 0a0a 6465 6620  component...def 
-00016d50: 5f63 6865 636b 5f75 6e63 6163 6865 645f  _check_uncached_
-00016d60: 636f 6d70 6f6e 656e 7473 2863 6f6d 706f  components(compo
-00016d70: 6e65 6e74 2c20 6d6f 6465 293a 0a20 2020  nent, mode):.   
-00016d80: 2076 616c 6964 5f6d 6f64 6573 203d 205b   valid_modes = [
-00016d90: 2277 6172 6e22 2c20 2265 7272 6f72 222c  "warn", "error",
-00016da0: 2022 6967 6e6f 7265 225d 0a0a 2020 2020   "ignore"]..    
-00016db0: 6966 206d 6f64 6520 3d3d 2022 6967 6e6f  if mode == "igno
-00016dc0: 7265 223a 0a20 2020 2020 2020 2072 6574  re":.        ret
-00016dd0: 7572 6e0a 2020 2020 656c 6966 206d 6f64  urn.    elif mod
-00016de0: 6520 6e6f 7420 696e 2076 616c 6964 5f6d  e not in valid_m
-00016df0: 6f64 6573 3a0a 2020 2020 2020 2020 7261  odes:.        ra
-00016e00: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-00016e10: 2020 2020 2020 2020 2020 2020 6622 7b6d              f"{m
-00016e20: 6f64 657d 2069 7320 6e6f 7420 6120 7661  ode} is not a va
-00016e30: 6c69 6420 7661 6c75 6520 666f 7220 6f6e  lid value for on
-00016e40: 5f75 6e63 6163 6865 645f 636f 6d70 6f6e  _uncached_compon
-00016e50: 656e 742e 2054 7279 206f 6e65 206f 6620  ent. Try one of 
-00016e60: 7468 6573 653a 207b 7661 6c69 645f 6d6f  these: {valid_mo
-00016e70: 6465 737d 2e22 0a20 2020 2020 2020 2029  des}.".        )
-00016e80: 0a0a 2020 2020 666f 7220 7375 625f 636f  ..    for sub_co
-00016e90: 6d70 6f6e 656e 7420 696e 2063 6f6d 706f  mponent in compo
-00016ea0: 6e65 6e74 2e67 6574 5f64 6570 656e 6465  nent.get_depende
-00016eb0: 6e63 6965 7328 7265 6375 7273 6976 653d  ncies(recursive=
-00016ec0: 5472 7565 293a 0a20 2020 2020 2020 2069  True):.        i
-00016ed0: 6620 6e6f 7420 7375 625f 636f 6d70 6f6e  f not sub_compon
-00016ee0: 656e 742e 5f6c 6f63 6b65 643a 0a20 2020  ent._locked:.   
-00016ef0: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00016f00: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00016f10: 2020 2020 2066 2243 6f6d 706f 6e65 6e74       f"Component
-00016f20: 207b 7375 625f 636f 6d70 6f6e 656e 742e   {sub_component.
-00016f30: 6e61 6d65 2172 7d20 7761 7320 4e4f 5420  name!r} was NOT 
-00016f40: 7072 6f70 6572 6c79 206c 6f63 6b65 642e  properly locked.
-00016f50: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00016f60: 2020 2022 596f 7520 6e65 6564 2074 6f20     "You need to 
-00016f70: 7772 6974 6520 6974 2069 6e74 6f20 6120  write it into a 
-00016f80: 6675 6e63 7469 6f6e 2074 6861 7420 6861  function that ha
-00016f90: 7320 7468 6520 4063 656c 6c20 6465 636f  s the @cell deco
-00016fa0: 7261 746f 722e 220a 2020 2020 2020 2020  rator.".        
-00016fb0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00016fc0: 2020 6966 206d 6f64 6520 3d3d 2022 7761    if mode == "wa
-00016fd0: 726e 223a 0a20 2020 2020 2020 2020 2020  rn":.           
-00016fe0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-00016ff0: 726e 286d 6573 7361 6765 2c20 556e 6361  rn(message, Unca
-00017000: 6368 6564 436f 6d70 6f6e 656e 7457 6172  chedComponentWar
-00017010: 6e69 6e67 290a 0a20 2020 2020 2020 2020  ning)..         
-00017020: 2020 2065 6c69 6620 6d6f 6465 203d 3d20     elif mode == 
-00017030: 2265 7272 6f72 223a 0a20 2020 2020 2020  "error":.       
-00017040: 2020 2020 2020 2020 2072 6169 7365 2055           raise U
-00017050: 6e63 6163 6865 6443 6f6d 706f 6e65 6e74  ncachedComponent
-00017060: 4572 726f 7228 6d65 7373 6167 6529 0a0a  Error(message)..
-00017070: 0a64 6566 2074 6573 745f 7361 6d65 5f75  .def test_same_u
-00017080: 6964 2829 202d 3e20 4e6f 6e65 3a0a 2020  id() -> None:.  
-00017090: 2020 696d 706f 7274 2067 6473 6661 6374    import gdsfact
-000170a0: 6f72 7920 6173 2067 660a 0a20 2020 2063  ory as gf..    c
-000170b0: 203d 2043 6f6d 706f 6e65 6e74 2829 0a20   = Component(). 
-000170c0: 2020 2063 203c 3c20 6766 2e63 6f6d 706f     c << gf.compo
-000170d0: 6e65 6e74 732e 7265 6374 616e 676c 6528  nents.rectangle(
-000170e0: 290a 2020 2020 6320 3c3c 2067 662e 636f  ).    c << gf.co
-000170f0: 6d70 6f6e 656e 7473 2e72 6563 7461 6e67  mponents.rectang
-00017100: 6c65 2829 0a0a 2020 2020 7231 203d 2063  le()..    r1 = c
-00017110: 2e72 6566 6572 656e 6365 735b 305d 2e70  .references[0].p
-00017120: 6172 656e 740a 2020 2020 7232 203d 2063  arent.    r2 = c
-00017130: 2e72 6566 6572 656e 6365 735b 315d 2e70  .references[1].p
-00017140: 6172 656e 740a 0a20 2020 2061 7373 6572  arent..    asser
-00017150: 7420 7231 2e75 6964 203d 3d20 7232 2e75  t r1.uid == r2.u
-00017160: 6964 2c20 6622 7b72 312e 7569 647d 206d  id, f"{r1.uid} m
-00017170: 7573 7420 6571 7561 6c20 7b72 322e 7569  ust equal {r2.ui
-00017180: 647d 220a 0a0a 6465 6620 7465 7374 5f6e  d}"...def test_n
-00017190: 6574 6c69 7374 5f73 696d 706c 6528 2920  etlist_simple() 
-000171a0: 2d3e 204e 6f6e 653a 0a20 2020 2069 6d70  -> None:.    imp
-000171b0: 6f72 7420 6764 7366 6163 746f 7279 2061  ort gdsfactory a
-000171c0: 7320 6766 0a0a 2020 2020 6320 3d20 6766  s gf..    c = gf
-000171d0: 2e43 6f6d 706f 6e65 6e74 2829 0a20 2020  .Component().   
-000171e0: 2063 3120 3d20 6320 3c3c 2067 662e 636f   c1 = c << gf.co
-000171f0: 6d70 6f6e 656e 7473 2e73 7472 6169 6768  mponents.straigh
-00017200: 7428 6c65 6e67 7468 3d31 2c20 7769 6474  t(length=1, widt
-00017210: 683d 3229 0a20 2020 2063 3220 3d20 6320  h=2).    c2 = c 
-00017220: 3c3c 2067 662e 636f 6d70 6f6e 656e 7473  << gf.components
-00017230: 2e73 7472 6169 6768 7428 6c65 6e67 7468  .straight(length
-00017240: 3d32 2c20 7769 6474 683d 3229 0a20 2020  =2, width=2).   
-00017250: 2063 322e 636f 6e6e 6563 7428 706f 7274   c2.connect(port
-00017260: 3d22 6f31 222c 2064 6573 7469 6e61 7469  ="o1", destinati
-00017270: 6f6e 3d63 312e 706f 7274 735b 226f 3222  on=c1.ports["o2"
-00017280: 5d29 0a20 2020 2063 2e61 6464 5f70 6f72  ]).    c.add_por
-00017290: 7428 226f 3122 2c20 706f 7274 3d63 312e  t("o1", port=c1.
-000172a0: 706f 7274 735b 226f 3122 5d29 0a20 2020  ports["o1"]).   
-000172b0: 2063 2e61 6464 5f70 6f72 7428 226f 3222   c.add_port("o2"
-000172c0: 2c20 706f 7274 3d63 322e 706f 7274 735b  , port=c2.ports[
-000172d0: 226f 3222 5d29 0a20 2020 206e 6574 6c69  "o2"]).    netli
-000172e0: 7374 203d 2063 2e67 6574 5f6e 6574 6c69  st = c.get_netli
-000172f0: 7374 2829 0a20 2020 2023 2070 7269 6e74  st().    # print
-00017300: 286e 6574 6c69 7374 2e70 7265 7474 7928  (netlist.pretty(
-00017310: 2929 0a20 2020 2061 7373 6572 7420 6c65  )).    assert le
-00017320: 6e28 6e65 746c 6973 745b 2269 6e73 7461  n(netlist["insta
-00017330: 6e63 6573 225d 2920 3d3d 2032 0a0a 0a64  nces"]) == 2...d
-00017340: 6566 2074 6573 745f 6e65 746c 6973 745f  ef test_netlist_
-00017350: 7369 6d70 6c65 5f77 6964 7468 5f6d 6973  simple_width_mis
-00017360: 6d61 7463 685f 7468 726f 7773 5f65 7272  match_throws_err
-00017370: 6f72 2829 202d 3e20 4e6f 6e65 3a0a 2020  or() -> None:.  
-00017380: 2020 696d 706f 7274 2070 7974 6573 740a    import pytest.
-00017390: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
-000173a0: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
-000173b0: 2020 6320 3d20 6766 2e43 6f6d 706f 6e65    c = gf.Compone
-000173c0: 6e74 2829 0a20 2020 2063 3120 3d20 6320  nt().    c1 = c 
-000173d0: 3c3c 2067 662e 636f 6d70 6f6e 656e 7473  << gf.components
-000173e0: 2e73 7472 6169 6768 7428 6c65 6e67 7468  .straight(length
-000173f0: 3d31 2c20 7769 6474 683d 3129 0a20 2020  =1, width=1).   
-00017400: 2063 3220 3d20 6320 3c3c 2067 662e 636f   c2 = c << gf.co
-00017410: 6d70 6f6e 656e 7473 2e73 7472 6169 6768  mponents.straigh
-00017420: 7428 6c65 6e67 7468 3d32 2c20 7769 6474  t(length=2, widt
-00017430: 683d 3229 0a20 2020 2063 322e 636f 6e6e  h=2).    c2.conn
-00017440: 6563 7428 706f 7274 3d22 6f31 222c 2064  ect(port="o1", d
-00017450: 6573 7469 6e61 7469 6f6e 3d63 312e 706f  estination=c1.po
-00017460: 7274 735b 226f 3222 5d29 0a20 2020 2063  rts["o2"]).    c
-00017470: 2e61 6464 5f70 6f72 7428 226f 3122 2c20  .add_port("o1", 
-00017480: 706f 7274 3d63 312e 706f 7274 735b 226f  port=c1.ports["o
-00017490: 3122 5d29 0a20 2020 2063 2e61 6464 5f70  1"]).    c.add_p
-000174a0: 6f72 7428 226f 3222 2c20 706f 7274 3d63  ort("o2", port=c
-000174b0: 322e 706f 7274 735b 226f 3222 5d29 0a20  2.ports["o2"]). 
-000174c0: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
-000174d0: 6169 7365 7328 5661 6c75 6545 7272 6f72  aises(ValueError
-000174e0: 293a 0a20 2020 2020 2020 2063 2e67 6574  ):.        c.get
-000174f0: 5f6e 6574 6c69 7374 2829 0a0a 0a64 6566  _netlist()...def
-00017500: 2074 6573 745f 6e65 746c 6973 745f 636f   test_netlist_co
-00017510: 6d70 6c65 7828 2920 2d3e 204e 6f6e 653a  mplex() -> None:
-00017520: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
-00017530: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
-00017540: 2020 6320 3d20 6766 2e63 6f6d 706f 6e65    c = gf.compone
-00017550: 6e74 732e 6d7a 695f 6172 6d73 2829 0a20  nts.mzi_arms(). 
-00017560: 2020 206e 6574 6c69 7374 203d 2063 2e67     netlist = c.g
-00017570: 6574 5f6e 6574 6c69 7374 2829 0a20 2020  et_netlist().   
-00017580: 2023 2070 7269 6e74 286e 6574 6c69 7374   # print(netlist
-00017590: 2e70 7265 7474 7928 2929 0a20 2020 2061  .pretty()).    a
-000175a0: 7373 6572 7420 6c65 6e28 6e65 746c 6973  ssert len(netlis
-000175b0: 745b 2269 6e73 7461 6e63 6573 225d 2920  t["instances"]) 
-000175c0: 3d3d 2034 2c20 6c65 6e28 6e65 746c 6973  == 4, len(netlis
-000175d0: 745b 2269 6e73 7461 6e63 6573 225d 290a  t["instances"]).
-000175e0: 0a0a 6465 6620 7465 7374 5f65 7874 7261  ..def test_extra
-000175f0: 6374 2829 202d 3e20 436f 6d70 6f6e 656e  ct() -> Componen
-00017600: 743a 0a20 2020 2069 6d70 6f72 7420 6764  t:.    import gd
-00017610: 7366 6163 746f 7279 2061 7320 6766 0a0a  sfactory as gf..
-00017620: 2020 2020 6320 3d20 6766 2e63 6f6d 706f      c = gf.compo
-00017630: 6e65 6e74 732e 7374 7261 6967 6874 280a  nents.straight(.
-00017640: 2020 2020 2020 2020 6c65 6e67 7468 3d31          length=1
-00017650: 302c 0a20 2020 2020 2020 2077 6964 7468  0,.        width
-00017660: 3d30 2e35 2c0a 2020 2020 2020 2020 6262  =0.5,.        bb
-00017670: 6f78 5f6c 6179 6572 733d 5b67 662e 4c41  ox_layers=[gf.LA
-00017680: 5945 522e 5747 434c 4144 5d2c 0a20 2020  YER.WGCLAD],.   
-00017690: 2020 2020 2062 626f 785f 6f66 6673 6574       bbox_offset
-000176a0: 733d 5b33 5d2c 0a20 2020 2020 2020 2077  s=[3],.        w
-000176b0: 6974 685f 6262 6f78 3d54 7275 652c 0a20  ith_bbox=True,. 
-000176c0: 2020 2020 2020 2063 6c61 6464 696e 675f         cladding_
-000176d0: 6c61 7965 7273 3d4e 6f6e 652c 0a20 2020  layers=None,.   
-000176e0: 2020 2020 2061 6464 5f70 696e 733d 4e6f       add_pins=No
-000176f0: 6e65 2c0a 2020 2020 2020 2020 6164 645f  ne,.        add_
-00017700: 6262 6f78 3d4e 6f6e 652c 0a20 2020 2029  bbox=None,.    )
-00017710: 0a20 2020 2063 3220 3d20 632e 6578 7472  .    c2 = c.extr
-00017720: 6163 7428 6c61 7965 7273 3d5b 6766 2e4c  act(layers=[gf.L
-00017730: 4159 4552 2e57 4743 4c41 445d 290a 0a20  AYER.WGCLAD]).. 
-00017740: 2020 2061 7373 6572 7420 6c65 6e28 632e     assert len(c.
-00017750: 706f 6c79 676f 6e73 2920 3d3d 2032 2c20  polygons) == 2, 
-00017760: 6c65 6e28 632e 706f 6c79 676f 6e73 290a  len(c.polygons).
-00017770: 2020 2020 6173 7365 7274 206c 656e 2863      assert len(c
-00017780: 322e 706f 6c79 676f 6e73 2920 3d3d 2031  2.polygons) == 1
-00017790: 2c20 6c65 6e28 6332 2e70 6f6c 7967 6f6e  , len(c2.polygon
-000177a0: 7329 0a20 2020 2061 7373 6572 7420 6766  s).    assert gf
-000177b0: 2e4c 4159 4552 2e57 4743 4c41 4420 696e  .LAYER.WGCLAD in
-000177c0: 2063 322e 6c61 7965 7273 0a20 2020 2072   c2.layers.    r
-000177d0: 6574 7572 6e20 6332 0a0a 0a64 6566 2068  eturn c2...def h
-000177e0: 6173 685f 6669 6c65 2866 696c 6570 6174  ash_file(filepat
-000177f0: 6829 3a0a 2020 2020 6d64 3520 3d20 6861  h):.    md5 = ha
-00017800: 7368 6c69 622e 6d64 3528 290a 2020 2020  shlib.md5().    
-00017810: 6d64 352e 7570 6461 7465 2866 696c 6570  md5.update(filep
-00017820: 6174 682e 7265 6164 5f62 7974 6573 2829  ath.read_bytes()
-00017830: 290a 2020 2020 7265 7475 726e 206d 6435  ).    return md5
-00017840: 2e68 6578 6469 6765 7374 2829 0a0a 0a64  .hexdigest()...d
-00017850: 6566 2074 6573 745f 6262 6f78 5f72 6566  ef test_bbox_ref
-00017860: 6572 656e 6365 2829 202d 3e20 436f 6d70  erence() -> Comp
-00017870: 6f6e 656e 743a 0a20 2020 2069 6d70 6f72  onent:.    impor
-00017880: 7420 6764 7366 6163 746f 7279 2061 7320  t gdsfactory as 
-00017890: 6766 0a0a 2020 2020 6320 3d20 6766 2e43  gf..    c = gf.C
-000178a0: 6f6d 706f 6e65 6e74 2822 636f 6d70 6f6e  omponent("compon
-000178b0: 656e 745f 7769 7468 5f6f 6666 6772 6964  ent_with_offgrid
-000178c0: 5f70 6f6c 7967 6f6e 7322 290a 2020 2020  _polygons").    
-000178d0: 6331 203d 2063 203c 3c20 6766 2e63 6f6d  c1 = c << gf.com
-000178e0: 706f 6e65 6e74 732e 7265 6374 616e 676c  ponents.rectangl
-000178f0: 6528 7369 7a65 3d28 312e 3565 2d33 2c20  e(size=(1.5e-3, 
-00017900: 312e 3565 2d33 292c 2070 6f72 745f 7479  1.5e-3), port_ty
-00017910: 7065 3d4e 6f6e 6529 0a20 2020 2063 3220  pe=None).    c2 
-00017920: 3d20 6320 3c3c 2067 662e 636f 6d70 6f6e  = c << gf.compon
-00017930: 656e 7473 2e72 6563 7461 6e67 6c65 2873  ents.rectangle(s
-00017940: 697a 653d 2831 2e35 652d 332c 2031 2e35  ize=(1.5e-3, 1.5
-00017950: 652d 3329 2c20 706f 7274 5f74 7970 653d  e-3), port_type=
-00017960: 4e6f 6e65 290a 2020 2020 6332 2e78 6d69  None).    c2.xmi
-00017970: 6e20 3d20 6331 2e78 6d61 780a 0a20 2020  n = c1.xmax..   
-00017980: 2061 7373 6572 7420 6332 2e78 7369 7a65   assert c2.xsize
-00017990: 203d 3d20 3265 2d33 0a20 2020 2072 6574   == 2e-3.    ret
-000179a0: 7572 6e20 6332 0a0a 0a64 6566 2074 6573  urn c2...def tes
-000179b0: 745f 6262 6f78 5f63 6f6d 706f 6e65 6e74  t_bbox_component
-000179c0: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-000179d0: 696d 706f 7274 2067 6473 6661 6374 6f72  import gdsfactor
-000179e0: 7920 6173 2067 660a 0a20 2020 2063 203d  y as gf..    c =
-000179f0: 2067 662e 636f 6d70 6f6e 656e 7473 2e72   gf.components.r
-00017a00: 6563 7461 6e67 6c65 2873 697a 653d 2831  ectangle(size=(1
-00017a10: 2e35 652d 332c 2031 2e35 652d 3329 2c20  .5e-3, 1.5e-3), 
-00017a20: 706f 7274 5f74 7970 653d 4e6f 6e65 290a  port_type=None).
-00017a30: 2020 2020 6173 7365 7274 2063 2e78 7369      assert c.xsi
-00017a40: 7a65 203d 3d20 3265 2d33 0a0a 0a64 6566  ze == 2e-3...def
-00017a50: 2074 6573 745f 7265 6d61 705f 6c61 7965   test_remap_laye
-00017a60: 7273 2829 202d 3e20 4e6f 6e65 3a0a 2020  rs() -> None:.  
-00017a70: 2020 696d 706f 7274 2067 6473 6661 6374    import gdsfact
-00017a80: 6f72 7920 6173 2067 660a 0a20 2020 2063  ory as gf..    c
-00017a90: 203d 2067 662e 636f 6d70 6f6e 656e 7473   = gf.components
-00017aa0: 2e73 7472 6169 6768 7428 6c61 7965 723d  .straight(layer=
-00017ab0: 2832 2c20 3029 290a 2020 2020 7265 6d61  (2, 0)).    rema
-00017ac0: 7020 3d20 632e 7265 6d61 705f 6c61 7965  p = c.remap_laye
-00017ad0: 7273 286c 6179 6572 6d61 703d 7b28 322c  rs(layermap={(2,
-00017ae0: 2030 293a 2067 662e 4c41 5945 522e 5747   0): gf.LAYER.WG
-00017af0: 4e7d 290a 2020 2020 6861 7368 5f67 656f  N}).    hash_geo
-00017b00: 6d65 7472 7920 3d20 2238 3366 6263 3661  metry = "83fbc6a
-00017b10: 3832 3839 3530 3565 6165 6433 6132 6533  8289505eaed3a2e3
-00017b20: 6162 3237 3963 6330 3366 3565 3464 3030  ab279cc03f5e4d00
-00017b30: 6322 0a0a 2020 2020 6173 7365 7274 2028  c"..    assert (
-00017b40: 0a20 2020 2020 2020 2072 656d 6170 2e68  .        remap.h
-00017b50: 6173 685f 6765 6f6d 6574 7279 2829 203d  ash_geometry() =
-00017b60: 3d20 6861 7368 5f67 656f 6d65 7472 790a  = hash_geometry.
-00017b70: 2020 2020 292c 2066 2268 6173 685f 6765      ), f"hash_ge
-00017b80: 6f6d 6574 7279 203d 207b 7265 6d61 702e  ometry = {remap.
-00017b90: 6861 7368 5f67 656f 6d65 7472 7928 2921  hash_geometry()!
-00017ba0: 727d 220a 0a0a 6465 6620 7465 7374 5f72  r}"...def test_r
-00017bb0: 656d 6f76 655f 6c61 6265 6c73 2829 202d  emove_labels() -
-00017bc0: 3e20 4e6f 6e65 3a0a 2020 2020 696d 706f  > None:.    impo
-00017bd0: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
-00017be0: 2067 660a 0a20 2020 2063 203d 2067 662e   gf..    c = gf.
-00017bf0: 632e 7374 7261 6967 6874 2829 0a20 2020  c.straight().   
-00017c00: 2063 2e72 656d 6f76 655f 6c61 6265 6c73   c.remove_labels
-00017c10: 2829 0a0a 2020 2020 6173 7365 7274 206c  ()..    assert l
-00017c20: 656e 2863 2e6c 6162 656c 7329 203d 3d20  en(c.labels) == 
-00017c30: 300a 0a0a 6465 6620 7465 7374 5f69 6d70  0...def test_imp
-00017c40: 6f72 745f 6764 735f 7365 7474 696e 6773  ort_gds_settings
-00017c50: 2829 3a0a 2020 2020 696d 706f 7274 2067  ():.    import g
-00017c60: 6473 6661 6374 6f72 7920 6173 2067 660a  dsfactory as gf.
-00017c70: 0a20 2020 2063 203d 2067 662e 636f 6d70  .    c = gf.comp
-00017c80: 6f6e 656e 7473 2e6d 7a69 2829 0a20 2020  onents.mzi().   
-00017c90: 2067 6473 7061 7468 203d 2063 2e77 7269   gdspath = c.wri
-00017ca0: 7465 5f67 6473 5f77 6974 685f 6d65 7461  te_gds_with_meta
-00017cb0: 6461 7461 2829 0a20 2020 2063 3220 3d20  data().    c2 = 
-00017cc0: 6766 2e69 6d70 6f72 745f 6764 7328 6764  gf.import_gds(gd
-00017cd0: 7370 6174 682c 206e 616d 653d 226d 7a69  spath, name="mzi
-00017ce0: 5f73 616d 706c 6522 2c20 7265 6164 5f6d  _sample", read_m
-00017cf0: 6574 6164 6174 613d 5472 7565 290a 2020  etadata=True).  
-00017d00: 2020 6333 203d 2067 662e 726f 7574 696e    c3 = gf.routin
-00017d10: 672e 6164 645f 6669 6265 725f 7369 6e67  g.add_fiber_sing
-00017d20: 6c65 2863 3229 0a20 2020 2061 7373 6572  le(c2).    asser
-00017d30: 7420 6333 0a0a 0a64 6566 2074 6573 745f  t c3...def test_
-00017d40: 666c 6174 7465 6e5f 696e 7661 6c69 645f  flatten_invalid_
-00017d50: 7265 6673 5f72 6563 7572 7369 7665 2829  refs_recursive()
-00017d60: 3a0a 2020 2020 696d 706f 7274 2067 6473  :.    import gds
-00017d70: 6661 6374 6f72 7920 6173 2067 660a 2020  factory as gf.  
-00017d80: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
-00017d90: 792e 6469 6666 7465 7374 2069 6d70 6f72  y.difftest impor
-00017da0: 7420 7275 6e5f 786f 720a 2020 2020 6672  t run_xor.    fr
-00017db0: 6f6d 2067 6473 6661 6374 6f72 792e 726f  om gdsfactory.ro
-00017dc0: 7574 696e 672e 616c 6c5f 616e 676c 6520  uting.all_angle 
-00017dd0: 696d 706f 7274 2067 6574 5f62 756e 646c  import get_bundl
-00017de0: 655f 616c 6c5f 616e 676c 650a 0a20 2020  e_all_angle..   
-00017df0: 2040 6766 2e63 656c 6c0a 2020 2020 6465   @gf.cell.    de
-00017e00: 6620 666c 6174 2829 3a0a 2020 2020 2020  f flat():.      
-00017e10: 2020 6320 3d20 6766 2e43 6f6d 706f 6e65    c = gf.Compone
-00017e20: 6e74 2829 0a20 2020 2020 2020 206d 6d69  nt().        mmi
-00017e30: 3120 3d20 2863 203c 3c20 6766 2e63 6f6d  1 = (c << gf.com
-00017e40: 706f 6e65 6e74 732e 6d6d 6931 7832 2829  ponents.mmi1x2()
-00017e50: 292e 6d6f 7665 2828 302c 202d 312e 3030  ).move((0, -1.00
-00017e60: 3035 2929 0a20 2020 2020 2020 206d 6d69  05)).        mmi
-00017e70: 3220 3d20 2863 203c 3c20 6766 2e63 6f6d  2 = (c << gf.com
-00017e80: 706f 6e65 6e74 732e 6d6d 6931 7832 2829  ponents.mmi1x2()
-00017e90: 292e 726f 7461 7465 2838 3029 0a20 2020  ).rotate(80).   
-00017ea0: 2020 2020 206d 6d69 322e 6d6f 7665 2828       mmi2.move((
-00017eb0: 3430 2c20 3230 2929 0a20 2020 2020 2020  40, 20)).       
-00017ec0: 2062 756e 646c 6520 3d20 6765 745f 6275   bundle = get_bu
-00017ed0: 6e64 6c65 5f61 6c6c 5f61 6e67 6c65 285b  ndle_all_angle([
-00017ee0: 6d6d 6931 2e70 6f72 7473 5b22 6f32 225d  mmi1.ports["o2"]
-00017ef0: 5d2c 205b 6d6d 6932 2e70 6f72 7473 5b22  ], [mmi2.ports["
-00017f00: 6f31 225d 5d29 0a20 2020 2020 2020 2066  o1"]]).        f
-00017f10: 6f72 2072 6f75 7465 2069 6e20 6275 6e64  or route in bund
-00017f20: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00017f30: 632e 6164 6428 726f 7574 652e 7265 6665  c.add(route.refe
-00017f40: 7265 6e63 6573 290a 2020 2020 2020 2020  rences).        
-00017f50: 7265 7475 726e 2063 0a0a 2020 2020 4067  return c..    @g
-00017f60: 662e 6365 6c6c 0a20 2020 2064 6566 2068  f.cell.    def h
-00017f70: 6965 7261 7263 6879 2829 3a0a 2020 2020  ierarchy():.    
-00017f80: 2020 2020 6320 3d20 6766 2e43 6f6d 706f      c = gf.Compo
-00017f90: 6e65 6e74 2829 0a20 2020 2020 2020 2028  nent().        (
-00017fa0: 6320 3c3c 2066 6c61 7428 2929 2e72 6f74  c << flat()).rot
-00017fb0: 6174 6528 3333 290a 2020 2020 2020 2020  ate(33).        
-00017fc0: 2863 203c 3c20 666c 6174 2829 292e 726f  (c << flat()).ro
-00017fd0: 7461 7465 2833 3329 2e6d 6f76 6528 2830  tate(33).move((0
-00017fe0: 2c20 3130 3029 290a 2020 2020 2020 2020  , 100)).        
-00017ff0: 2863 203c 3c20 666c 6174 2829 292e 6d6f  (c << flat()).mo
-00018000: 7665 2828 3130 302c 2030 2929 0a20 2020  ve((100, 0)).   
-00018010: 2020 2020 2072 6574 7572 6e20 630a 0a20       return c.. 
-00018020: 2020 2063 5f6f 7269 6720 3d20 6869 6572     c_orig = hier
-00018030: 6172 6368 7928 290a 2020 2020 635f 6e65  archy().    c_ne
-00018040: 7720 3d20 666c 6174 7465 6e5f 696e 7661  w = flatten_inva
-00018050: 6c69 645f 7265 6673 5f72 6563 7572 7369  lid_refs_recursi
-00018060: 7665 2863 5f6f 7269 6729 0a20 2020 2061  ve(c_orig).    a
-00018070: 7373 6572 7420 635f 6e65 7720 6973 206e  ssert c_new is n
-00018080: 6f74 2063 5f6f 7269 670a 2020 2020 696e  ot c_orig.    in
-00018090: 7661 6c69 645f 7265 6673 5f66 696c 656e  valid_refs_filen
-000180a0: 616d 6520 3d20 2269 6e76 616c 6964 5f72  ame = "invalid_r
-000180b0: 6566 732e 6764 7322 0a20 2020 2069 6e76  efs.gds".    inv
-000180c0: 616c 6964 5f72 6566 735f 6669 7865 645f  alid_refs_fixed_
-000180d0: 6669 6c65 6e61 6d65 203d 2022 696e 7661  filename = "inva
-000180e0: 6c69 645f 7265 6673 5f66 6978 6564 2e67  lid_refs_fixed.g
-000180f0: 6473 220a 2020 2020 2320 6764 7320 6669  ds".    # gds fi
-00018100: 6c65 7320 7368 6f75 6c64 2073 7469 6c6c  les should still
-00018110: 2062 6520 7361 6d65 2074 6f20 316e 6d20   be same to 1nm 
-00018120: 746f 6c65 7261 6e63 650a 2020 2020 635f  tolerance.    c_
-00018130: 6f72 6967 2e77 7269 7465 5f67 6473 2869  orig.write_gds(i
-00018140: 6e76 616c 6964 5f72 6566 735f 6669 6c65  nvalid_refs_file
-00018150: 6e61 6d65 290a 2020 2020 635f 6e65 772e  name).    c_new.
-00018160: 7772 6974 655f 6764 7328 696e 7661 6c69  write_gds(invali
-00018170: 645f 7265 6673 5f66 6978 6564 5f66 696c  d_refs_fixed_fil
-00018180: 656e 616d 6529 0a20 2020 2072 756e 5f78  ename).    run_x
-00018190: 6f72 2869 6e76 616c 6964 5f72 6566 735f  or(invalid_refs_
-000181a0: 6669 6c65 6e61 6d65 2c20 696e 7661 6c69  filename, invali
-000181b0: 645f 7265 6673 5f66 6978 6564 5f66 696c  d_refs_fixed_fil
-000181c0: 656e 616d 6529 0a0a 0a69 6620 5f5f 6e61  ename)...if __na
-000181d0: 6d65 5f5f 203d 3d20 225f 5f6d 6169 6e5f  me__ == "__main_
-000181e0: 5f22 3a0a 2020 2020 696d 706f 7274 2067  _":.    import g
-000181f0: 6473 6661 6374 6f72 7920 6173 2067 660a  dsfactory as gf.
-00018200: 0a20 2020 2023 2063 3220 3d20 6766 2e43  .    # c2 = gf.C
-00018210: 6f6d 706f 6e65 6e74 2829 0a20 2020 2063  omponent().    c
-00018220: 203d 2067 662e 636f 6d70 6f6e 656e 7473   = gf.components
-00018230: 2e6d 7a69 2829 0a20 2020 2070 7269 6e74  .mzi().    print
-00018240: 2863 2e67 6574 5f6c 6179 6572 5f6e 616d  (c.get_layer_nam
-00018250: 6573 2829 290a 2020 2020 2320 7220 3d20  es()).    # r = 
-00018260: 632e 7265 6628 290a 2020 2020 2320 6332  c.ref().    # c2
-00018270: 2e63 6f70 795f 6368 696c 645f 696e 666f  .copy_child_info
-00018280: 2863 2e6e 616d 6564 5f72 6566 6572 656e  (c.named_referen
-00018290: 6365 735b 2273 7874 225d 290a 2020 2020  ces["sxt"]).    
-000182a0: 2320 7465 7374 5f72 656d 6170 5f6c 6179  # test_remap_lay
-000182b0: 6572 7328 290a 2020 2020 2320 6320 3d20  ers().    # c = 
-000182c0: 7465 7374 5f67 6574 5f6c 6179 6572 7328  test_get_layers(
-000182d0: 290a 2020 2020 2320 632e 706c 6f74 5f71  ).    # c.plot_q
-000182e0: 7428 290a 2020 2020 2320 632e 706c 6f74  t().    # c.plot
-000182f0: 6828 290a 2020 2020 2320 6320 3d20 7465  h().    # c = te
-00018300: 7374 5f65 7874 7261 6374 2829 0a20 2020  st_extract().   
-00018310: 2023 2067 6473 7061 7468 203d 2063 2e77   # gdspath = c.w
-00018320: 7269 7465 5f67 6473 2829 0a20 2020 2023  rite_gds().    #
-00018330: 2067 662e 7368 6f77 2867 6473 7061 7468   gf.show(gdspath
-00018340: 290a 2020 2020 2320 632e 7368 6f77 2873  ).    # c.show(s
-00018350: 686f 775f 706f 7274 733d 5472 7565 290a  how_ports=True).
-00018360: 2020 2020 632e 7368 6f77 2829 0a             c.show().
+00008460: 2020 2065 6c69 6620 6861 7361 7474 7228     elif hasattr(
+00008470: 706f 696e 7473 2c20 2267 656f 6d73 2229  points, "geoms")
+00008480: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00008490: 7220 6765 6f6d 2069 6e20 706f 696e 7473  r geom in points
+000084a0: 2e67 656f 6d73 3a0a 2020 2020 2020 2020  .geoms:.        
+000084b0: 2020 2020 2020 2020 706f 6c79 676f 6e20          polygon 
+000084c0: 3d20 7365 6c66 2e61 6464 5f70 6f6c 7967  = self.add_polyg
+000084d0: 6f6e 2867 656f 6d2c 206c 6179 6572 3d6c  on(geom, layer=l
+000084e0: 6179 6572 290a 2020 2020 2020 2020 2020  ayer).          
+000084f0: 2020 7265 7475 726e 2070 6f6c 7967 6f6e    return polygon
+00008500: 0a20 2020 2020 2020 2065 6c69 6620 6861  .        elif ha
+00008510: 7361 7474 7228 706f 696e 7473 2c20 2265  sattr(points, "e
+00008520: 7874 6572 696f 7222 293a 2020 2320 706f  xterior"):  # po
+00008530: 696e 7473 2069 7320 6120 7368 6170 656c  ints is a shapel
+00008540: 7920 506f 6c79 676f 6e0a 2020 2020 2020  y Polygon.      
+00008550: 2020 2020 2020 6c61 7965 722c 2064 6174        layer, dat
+00008560: 6174 7970 6520 3d20 5f70 6172 7365 5f6c  atype = _parse_l
+00008570: 6179 6572 286c 6179 6572 290a 2020 2020  ayer(layer).    
+00008580: 2020 2020 2020 2020 706f 696e 7473 5f6f          points_o
+00008590: 6e5f 6772 6964 203d 206e 702e 726f 756e  n_grid = np.roun
+000085a0: 6428 706f 696e 7473 2e65 7874 6572 696f  d(points.exterio
+000085b0: 722e 636f 6f72 6473 2c20 3329 0a20 2020  r.coords, 3).   
+000085c0: 2020 2020 2020 2020 2070 6f6c 7967 6f6e           polygon
+000085d0: 203d 2067 6473 746b 2e50 6f6c 7967 6f6e   = gdstk.Polygon
+000085e0: 2870 6f69 6e74 735f 6f6e 5f67 7269 642c  (points_on_grid,
+000085f0: 206c 6179 6572 2c20 6461 7461 7479 7065   layer, datatype
+00008600: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00008610: 6620 706f 696e 7473 2e69 6e74 6572 696f  f points.interio
+00008620: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00008630: 2020 2020 6672 6f6d 2073 6861 7065 6c79      from shapely
+00008640: 2069 6d70 6f72 7420 6765 745f 636f 6f72   import get_coor
+00008650: 6469 6e61 7465 730a 0a20 2020 2020 2020  dinates..       
+00008660: 2020 2020 2020 2020 2070 6f69 6e74 735f           points_
+00008670: 6f6e 5f67 7269 645f 696e 7465 7269 6f72  on_grid_interior
+00008680: 203d 206e 702e 726f 756e 6428 6765 745f   = np.round(get_
+00008690: 636f 6f72 6469 6e61 7465 7328 706f 696e  coordinates(poin
+000086a0: 7473 2e69 6e74 6572 696f 7273 292c 2033  ts.interiors), 3
+000086b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000086c0: 2020 706f 6c79 676f 6e5f 696e 7465 7269    polygon_interi
+000086d0: 6f72 203d 2067 6473 746b 2e50 6f6c 7967  or = gdstk.Polyg
+000086e0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+000086f0: 2020 2020 2020 2020 706f 696e 7473 5f6f          points_o
+00008700: 6e5f 6772 6964 5f69 6e74 6572 696f 722c  n_grid_interior,
+00008710: 206c 6179 6572 2c20 6461 7461 7479 7065   layer, datatype
+00008720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008730: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00008740: 2020 2070 6f6c 7967 6f6e 7320 3d20 6764     polygons = gd
+00008750: 7374 6b2e 626f 6f6c 6561 6e28 0a20 2020  stk.boolean(.   
+00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008770: 2070 6f6c 7967 6f6e 2c0a 2020 2020 2020   polygon,.      
+00008780: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00008790: 6c79 676f 6e5f 696e 7465 7269 6f72 2c0a  lygon_interior,.
+000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087b0: 2020 2020 6f70 6572 6174 696f 6e3d 226e      operation="n
+000087c0: 6f74 222c 0a20 2020 2020 2020 2020 2020  ot",.           
+000087d0: 2020 2020 2020 2020 206c 6179 6572 3d6c           layer=l
+000087e0: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
+000087f0: 2020 2020 2020 2020 2020 6461 7461 7479            dataty
+00008800: 7065 3d64 6174 6174 7970 652c 0a20 2020  pe=datatype,.   
+00008810: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00008820: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00008830: 6f72 2070 6f6c 7967 6f6e 2069 6e20 706f  or polygon in po
+00008840: 6c79 676f 6e73 3a0a 2020 2020 2020 2020  lygons:.        
+00008850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008860: 2e5f 6164 645f 706f 6c79 676f 6e73 2870  ._add_polygons(p
+00008870: 6f6c 7967 6f6e 290a 2020 2020 2020 2020  olygon).        
+00008880: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+00008890: 6f6c 7967 6f6e 0a0a 2020 2020 2020 2020  olygon..        
+000088a0: 2020 2020 7365 6c66 2e5f 6164 645f 706f      self._add_po
+000088b0: 6c79 676f 6e73 2870 6f6c 7967 6f6e 290a  lygons(polygon).
+000088c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000088d0: 726e 2070 6f6c 7967 6f6e 0a0a 2020 2020  rn polygon..    
+000088e0: 2020 2020 706f 696e 7473 203d 206e 702e      points = np.
+000088f0: 6173 6172 7261 7928 706f 696e 7473 290a  asarray(points).
+00008900: 2020 2020 2020 2020 6966 2070 6f69 6e74          if point
+00008910: 732e 6e64 696d 203d 3d20 313a 0a20 2020  s.ndim == 1:.   
+00008920: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008930: 5b73 656c 662e 6164 645f 706f 6c79 676f  [self.add_polygo
+00008940: 6e28 706f 6c79 2c20 6c61 7965 723d 6c61  n(poly, layer=la
+00008950: 7965 7229 2066 6f72 2070 6f6c 7920 696e  yer) for poly in
+00008960: 2070 6f69 6e74 735d 0a20 2020 2020 2020   points].       
+00008970: 2069 6620 6c61 7965 7220 6973 206e 702e   if layer is np.
+00008980: 6e61 6e3a 0a20 2020 2020 2020 2020 2020  nan:.           
+00008990: 206c 6179 6572 203d 2030 0a0a 2020 2020   layer = 0..    
+000089a0: 2020 2020 6966 2070 6f69 6e74 732e 6e64      if points.nd
+000089b0: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
+000089c0: 2020 2020 2023 2061 6464 2073 696e 676c       # add singl
+000089d0: 6520 706f 6c79 676f 6e20 6672 6f6d 2070  e polygon from p
+000089e0: 6f69 6e74 730a 2020 2020 2020 2020 2020  oints.          
+000089f0: 2020 6966 206c 656e 2870 6f69 6e74 735b    if len(points[
+00008a00: 305d 2920 3e20 323a 0a20 2020 2020 2020  0]) > 2:.       
+00008a10: 2020 2020 2020 2020 2023 2043 6f6e 7665           # Conve
+00008a20: 7274 2074 6f20 666f 726d 205b 5b31 2c32  rt to form [[1,2
+00008a30: 5d2c 5b33 2c34 5d2c 5b35 2c36 5d5d 0a20  ],[3,4],[5,6]]. 
+00008a40: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00008a50: 6f69 6e74 7320 3d20 6e70 2e63 6f6c 756d  oints = np.colum
+00008a60: 6e5f 7374 6163 6b28 706f 696e 7473 290a  n_stack(points).
+00008a70: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+00008a80: 722c 2064 6174 6174 7970 6520 3d20 5f70  r, datatype = _p
+00008a90: 6172 7365 5f6c 6179 6572 286c 6179 6572  arse_layer(layer
+00008aa0: 290a 2020 2020 2020 2020 2020 2020 706f  ).            po
+00008ab0: 6c79 676f 6e20 3d20 506f 6c79 676f 6e28  lygon = Polygon(
+00008ac0: 706f 696e 7473 2c20 6c61 7965 723d 6c61  points, layer=la
+00008ad0: 7965 722c 2064 6174 6174 7970 653d 6461  yer, datatype=da
+00008ae0: 7461 7479 7065 290a 2020 2020 2020 2020  tatype).        
+00008af0: 2020 2020 7365 6c66 2e5f 6164 645f 706f      self._add_po
+00008b00: 6c79 676f 6e73 2870 6f6c 7967 6f6e 290a  lygons(polygon).
+00008b10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008b20: 726e 2070 6f6c 7967 6f6e 0a20 2020 2020  rn polygon.     
+00008b30: 2020 2065 6c69 6620 706f 696e 7473 2e6e     elif points.n
+00008b40: 6469 6d20 3d3d 2033 3a0a 2020 2020 2020  dim == 3:.      
+00008b50: 2020 2020 2020 6c61 7965 722c 2064 6174        layer, dat
+00008b60: 6174 7970 6520 3d20 5f70 6172 7365 5f6c  atype = _parse_l
+00008b70: 6179 6572 286c 6179 6572 290a 2020 2020  ayer(layer).    
+00008b80: 2020 2020 2020 2020 706f 6c79 676f 6e73          polygons
+00008b90: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00008ba0: 2020 2020 2050 6f6c 7967 6f6e 2870 706f       Polygon(ppo
+00008bb0: 696e 7473 2c20 6c61 7965 723d 6c61 7965  ints, layer=laye
+00008bc0: 722c 2064 6174 6174 7970 653d 6461 7461  r, datatype=data
+00008bd0: 7479 7065 2920 666f 7220 7070 6f69 6e74  type) for ppoint
+00008be0: 7320 696e 2070 6f69 6e74 730a 2020 2020  s in points.    
+00008bf0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00008c00: 2020 2020 2020 7365 6c66 2e5f 6164 645f        self._add_
+00008c10: 706f 6c79 676f 6e73 282a 706f 6c79 676f  polygons(*polygo
+00008c20: 6e73 290a 2020 2020 2020 2020 2020 2020  ns).            
+00008c30: 7265 7475 726e 2070 6f6c 7967 6f6e 730a  return polygons.
+00008c40: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00008c50: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00008c60: 5661 6c75 6545 7272 6f72 2866 2255 6e61  ValueError(f"Una
+00008c70: 626c 6520 746f 2061 6464 207b 706f 696e  ble to add {poin
+00008c80: 7473 2e6e 6469 6d7d 2d64 696d 656e 7369  ts.ndim}-dimensi
+00008c90: 6f6e 616c 2070 6f69 6e74 7320 6f62 6a65  onal points obje
+00008ca0: 6374 2229 0a0a 2020 2020 6465 6620 5f61  ct")..    def _a
+00008cb0: 6464 5f70 6f6c 7967 6f6e 7328 7365 6c66  dd_polygons(self
+00008cc0: 2c20 2a70 6f6c 7967 6f6e 733a 204c 6973  , *polygons: Lis
+00008cd0: 745b 506f 6c79 676f 6e5d 293a 0a20 2020  t[Polygon]):.   
+00008ce0: 2020 2020 2073 656c 662e 6973 5f75 6e6c       self.is_unl
+00008cf0: 6f63 6b65 6428 290a 2020 2020 2020 2020  ocked().        
+00008d00: 7365 6c66 2e5f 6365 6c6c 2e61 6464 282a  self._cell.add(*
+00008d10: 706f 6c79 676f 6e73 290a 0a20 2020 2064  polygons)..    d
+00008d20: 6566 2063 6f70 7928 7365 6c66 2920 2d3e  ef copy(self) ->
+00008d30: 2043 6f6d 706f 6e65 6e74 3a0a 2020 2020   Component:.    
+00008d40: 2020 2020 7265 7475 726e 2063 6f70 7928      return copy(
+00008d50: 7365 6c66 290a 0a20 2020 2064 6566 2061  self)..    def a
+00008d60: 6464 5f72 6566 5f63 6f6e 7461 696e 6572  dd_ref_container
+00008d70: 2873 656c 662c 2063 6f6d 706f 6e65 6e74  (self, component
+00008d80: 3a20 436f 6d70 6f6e 656e 7429 202d 3e20  : Component) -> 
+00008d90: 436f 6d70 6f6e 656e 7452 6566 6572 656e  ComponentReferen
+00008da0: 6365 3a0a 2020 2020 2020 2020 2222 2241  ce:.        """A
+00008db0: 6464 2072 6566 6572 656e 6365 2c20 706f  dd reference, po
+00008dc0: 7274 7320 616e 6420 636f 7079 5f63 6869  rts and copy_chi
+00008dd0: 6c64 5f69 6e66 6f2e 2222 220a 2020 2020  ld_info.""".    
+00008de0: 2020 2020 7265 6620 3d20 7365 6c66 203c      ref = self <
+00008df0: 3c20 636f 6d70 6f6e 656e 740a 2020 2020  < component.    
+00008e00: 2020 2020 7365 6c66 2e61 6464 5f70 6f72      self.add_por
+00008e10: 7473 2872 6566 2e70 6f72 7473 290a 2020  ts(ref.ports).  
+00008e20: 2020 2020 2020 7365 6c66 2e63 6f70 795f        self.copy_
+00008e30: 6368 696c 645f 696e 666f 2863 6f6d 706f  child_info(compo
+00008e40: 6e65 6e74 290a 2020 2020 2020 2020 7265  nent).        re
+00008e50: 7475 726e 2072 6566 0a0a 2020 2020 6465  turn ref..    de
+00008e60: 6620 636f 7079 5f63 6869 6c64 5f69 6e66  f copy_child_inf
+00008e70: 6f28 7365 6c66 2c20 636f 6d70 6f6e 656e  o(self, componen
+00008e80: 743a 2043 6f6d 706f 6e65 6e74 2920 2d3e  t: Component) ->
+00008e90: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00008ea0: 2222 436f 7079 2061 6e64 2073 6574 7469  ""Copy and setti
+00008eb0: 6e67 7320 696e 666f 2066 726f 6d20 6368  ngs info from ch
+00008ec0: 696c 6420 636f 6d70 6f6e 656e 7420 696e  ild component in
+00008ed0: 746f 2070 6172 656e 742e 0a0a 2020 2020  to parent...    
+00008ee0: 2020 2020 5061 7265 6e74 2063 6f6d 706f      Parent compo
+00008ef0: 6e65 6e74 7320 6361 6e20 6163 6365 7373  nents can access
+00008f00: 2063 6869 6c64 2063 656c 6c73 2073 6574   child cells set
+00008f10: 7469 6e67 732e 0a20 2020 2020 2020 2022  tings..        "
+00008f20: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+00008f30: 7420 6973 696e 7374 616e 6365 2863 6f6d  t isinstance(com
+00008f40: 706f 6e65 6e74 2c20 2843 6f6d 706f 6e65  ponent, (Compone
+00008f50: 6e74 2c20 436f 6d70 6f6e 656e 7452 6566  nt, ComponentRef
+00008f60: 6572 656e 6365 2929 3a0a 2020 2020 2020  erence)):.      
+00008f70: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00008f80: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00008f90: 2020 2020 2020 2020 6622 7b74 7970 6528          f"{type(
+00008fa0: 636f 6d70 6f6e 656e 7429 7d22 2022 6973  component)}" "is
+00008fb0: 206e 6f74 2061 2043 6f6d 706f 6e65 6e74   not a Component
+00008fc0: 206f 7220 436f 6d70 6f6e 656e 7452 6566   or ComponentRef
+00008fd0: 6572 656e 6365 220a 2020 2020 2020 2020  erence".        
+00008fe0: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
+00008ff0: 656c 662e 6765 745f 6368 696c 645f 6e61  elf.get_child_na
+00009000: 6d65 203d 2054 7275 650a 2020 2020 2020  me = True.      
+00009010: 2020 7365 6c66 2e63 6869 6c64 203d 2063    self.child = c
+00009020: 6f6d 706f 6e65 6e74 0a20 2020 2020 2020  omponent.       
+00009030: 2073 656c 662e 696e 666f 2e75 7064 6174   self.info.updat
+00009040: 6528 636f 6d70 6f6e 656e 742e 696e 666f  e(component.info
+00009050: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00009060: 6574 7469 6e67 732e 7570 6461 7465 2863  ettings.update(c
+00009070: 6f6d 706f 6e65 6e74 2e73 6574 7469 6e67  omponent.setting
+00009080: 7329 0a0a 2020 2020 4070 726f 7065 7274  s)..    @propert
+00009090: 790a 2020 2020 6465 6620 7369 7a65 5f69  y.    def size_i
+000090a0: 6e66 6f28 7365 6c66 2920 2d3e 2053 697a  nfo(self) -> Siz
+000090b0: 6549 6e66 6f3a 0a20 2020 2020 2020 2022  eInfo:.        "
+000090c0: 2222 5369 7a65 2069 6e66 6f20 6f66 2074  ""Size info of t
+000090d0: 6865 2063 6f6d 706f 6e65 6e74 2e22 2222  he component."""
+000090e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000090f0: 5369 7a65 496e 666f 2873 656c 662e 6262  SizeInfo(self.bb
+00009100: 6f78 290a 0a20 2020 2064 6566 2067 6574  ox)..    def get
+00009110: 5f73 6574 7469 6e67 2873 656c 662c 2073  _setting(self, s
+00009120: 6574 7469 6e67 3a20 7374 7229 202d 3e20  etting: str) -> 
+00009130: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
+00009140: 666c 6f61 745d 3a0a 2020 2020 2020 2020  float]:.        
+00009150: 7265 7475 726e 2028 0a20 2020 2020 2020  return (.       
+00009160: 2020 2020 2073 656c 662e 696e 666f 2e67       self.info.g
+00009170: 6574 2873 6574 7469 6e67 290a 2020 2020  et(setting).    
+00009180: 2020 2020 2020 2020 6f72 2073 656c 662e          or self.
+00009190: 7365 7474 696e 6773 2e66 756c 6c2e 6765  settings.full.ge
+000091a0: 7428 7365 7474 696e 6729 0a20 2020 2020  t(setting).     
+000091b0: 2020 2020 2020 206f 7220 7365 6c66 2e6d         or self.m
+000091c0: 6574 6164 6174 615f 6368 696c 642e 6765  etadata_child.ge
+000091d0: 7428 7365 7474 696e 6729 0a20 2020 2020  t(setting).     
+000091e0: 2020 2029 0a0a 2020 2020 6465 6620 6973     )..    def is
+000091f0: 5f75 6e6c 6f63 6b65 6428 7365 6c66 2920  _unlocked(self) 
+00009200: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00009210: 2022 2222 5261 6973 6573 2065 7272 6f72   """Raises error
+00009220: 2069 6620 436f 6d70 6f6e 656e 7420 6973   if Component is
+00009230: 206c 6f63 6b65 642e 2222 220a 2020 2020   locked.""".    
+00009240: 2020 2020 6966 2073 656c 662e 5f6c 6f63      if self._loc
+00009250: 6b65 643a 0a20 2020 2020 2020 2020 2020  ked:.           
+00009260: 2072 6169 7365 204d 7574 6162 696c 6974   raise Mutabilit
+00009270: 7945 7272 6f72 280a 2020 2020 2020 2020  yError(.        
+00009280: 2020 2020 2020 2020 6622 436f 6d70 6f6e          f"Compon
+00009290: 656e 7420 7b73 656c 662e 6e61 6d65 2172  ent {self.name!r
+000092a0: 7d20 6361 6e6e 6f74 2062 6520 6d6f 6469  } cannot be modi
+000092b0: 6669 6564 2061 7320 6974 2773 2061 6c72  fied as it's alr
+000092c0: 6561 6479 206f 6e20 6361 6368 652e 2022  eady on cache. "
+000092d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000092e0: 202b 206d 7574 6162 696c 6974 795f 6572   + mutability_er
+000092f0: 726f 725f 6d65 7373 6167 650a 2020 2020  ror_message.    
+00009300: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00009310: 6566 205f 6164 6428 7365 6c66 2c20 656c  ef _add(self, el
+00009320: 656d 656e 7429 202d 3e20 4e6f 6e65 3a0a  ement) -> None:.
+00009330: 2020 2020 2020 2020 2222 2241 6464 2061          """Add a
+00009340: 206e 6577 2065 6c65 6d65 6e74 206f 7220   new element or 
+00009350: 6c69 7374 206f 6620 656c 656d 656e 7473  list of elements
+00009360: 2074 6f20 7468 6973 2043 6f6d 706f 6e65   to this Compone
+00009370: 6e74 2e0a 0a20 2020 2020 2020 2041 7267  nt...        Arg
+00009380: 733a 0a20 2020 2020 2020 2020 2020 2065  s:.            e
+00009390: 6c65 6d65 6e74 3a20 506f 6c79 676f 6e2c  lement: Polygon,
+000093a0: 2043 6f6d 706f 6e65 6e74 5265 6665 7265   ComponentRefere
+000093b0: 6e63 6520 6f72 2069 7465 7261 626c 650a  nce or iterable.
+000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093d0: 5468 6520 656c 656d 656e 7420 6f72 2069  The element or i
+000093e0: 7465 7261 626c 6520 6f66 2065 6c65 6d65  terable of eleme
+000093f0: 6e74 7320 746f 2062 6520 696e 7365 7274  nts to be insert
+00009400: 6564 2069 6e20 7468 6973 2063 656c 6c2e  ed in this cell.
+00009410: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+00009420: 3a0a 2020 2020 2020 2020 2020 2020 4d75  :.            Mu
+00009430: 7461 6269 6c69 7479 4572 726f 723a 2069  tabilityError: i
+00009440: 6620 636f 6d70 6f6e 656e 7420 6973 206c  f component is l
+00009450: 6f63 6b65 642e 0a20 2020 2020 2020 2022  ocked..        "
+00009460: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00009470: 6973 5f75 6e6c 6f63 6b65 6428 290a 2020  is_unlocked().  
+00009480: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00009490: 6e63 6528 656c 656d 656e 742c 2043 6f6d  nce(element, Com
+000094a0: 706f 6e65 6e74 5265 6665 7265 6e63 6529  ponentReference)
+000094b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000094c0: 6c66 2e5f 6365 6c6c 2e61 6464 2865 6c65  lf._cell.add(ele
+000094d0: 6d65 6e74 2e5f 7265 6665 7265 6e63 6529  ment._reference)
+000094e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000094f0: 662e 5f72 6566 6572 656e 6365 732e 6170  f._references.ap
+00009500: 7065 6e64 2865 6c65 6d65 6e74 290a 2020  pend(element).  
+00009510: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009520: 2020 2020 2020 2020 7365 6c66 2e5f 6365          self._ce
+00009530: 6c6c 2e61 6464 2865 6c65 6d65 6e74 290a  ll.add(element).
+00009540: 0a20 2020 2064 6566 2061 6464 2873 656c  .    def add(sel
+00009550: 662c 2065 6c65 6d65 6e74 2920 2d3e 204e  f, element) -> N
+00009560: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00009570: 4164 6420 6120 6e65 7720 656c 656d 656e  Add a new elemen
+00009580: 7420 6f72 206c 6973 7420 6f66 2065 6c65  t or list of ele
+00009590: 6d65 6e74 7320 746f 2074 6869 7320 436f  ments to this Co
+000095a0: 6d70 6f6e 656e 742e 0a0a 2020 2020 2020  mponent...      
+000095b0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000095c0: 2020 2020 656c 656d 656e 743a 2050 6f6c      element: Pol
+000095d0: 7967 6f6e 2c20 436f 6d70 6f6e 656e 7452  ygon, ComponentR
+000095e0: 6566 6572 656e 6365 206f 7220 6974 6572  eference or iter
+000095f0: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
+00009600: 2020 2020 2054 6865 2065 6c65 6d65 6e74       The element
+00009610: 206f 7220 6974 6572 6162 6c65 206f 6620   or iterable of 
+00009620: 656c 656d 656e 7473 2074 6f20 6265 2069  elements to be i
+00009630: 6e73 6572 7465 6420 696e 2074 6869 7320  nserted in this 
+00009640: 6365 6c6c 2e0a 0a20 2020 2020 2020 2052  cell...        R
+00009650: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+00009660: 2020 204d 7574 6162 696c 6974 7945 7272     MutabilityErr
+00009670: 6f72 3a20 6966 2063 6f6d 706f 6e65 6e74  or: if component
+00009680: 2069 7320 6c6f 636b 6564 2e0a 2020 2020   is locked..    
+00009690: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000096a0: 6966 2069 7369 6e73 7461 6e63 6528 656c  if isinstance(el
+000096b0: 656d 656e 742c 2043 6f6d 706f 6e65 6e74  ement, Component
+000096c0: 5265 6665 7265 6e63 6529 3a0a 2020 2020  Reference):.    
+000096d0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+000096e0: 6769 7374 6572 5f72 6566 6572 656e 6365  gister_reference
+000096f0: 2865 6c65 6d65 6e74 290a 2020 2020 2020  (element).      
+00009700: 2020 2020 2020 7365 6c66 2e5f 6164 6428        self._add(
+00009710: 656c 656d 656e 7429 0a20 2020 2020 2020  element).       
+00009720: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00009730: 2865 6c65 6d65 6e74 2c20 4974 6572 6162  (element, Iterab
+00009740: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
+00009750: 2066 6f72 2073 7562 656c 656d 656e 7420   for subelement 
+00009760: 696e 2065 6c65 6d65 6e74 3a0a 2020 2020  in element:.    
+00009770: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009780: 2e61 6464 2873 7562 656c 656d 656e 7429  .add(subelement)
+00009790: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000097a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000097b0: 5f61 6464 2865 6c65 6d65 6e74 290a 0a20  _add(element).. 
+000097c0: 2020 2064 6566 2061 6464 5f61 7272 6179     def add_array
+000097d0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000097e0: 2020 2020 2020 2020 636f 6d70 6f6e 656e          componen
+000097f0: 743a 2043 6f6d 706f 6e65 6e74 2c0a 2020  t: Component,.  
+00009800: 2020 2020 2020 636f 6c75 6d6e 733a 2069        columns: i
+00009810: 6e74 203d 2032 2c0a 2020 2020 2020 2020  nt = 2,.        
+00009820: 726f 7773 3a20 696e 7420 3d20 322c 0a20  rows: int = 2,. 
+00009830: 2020 2020 2020 2073 7061 6369 6e67 3a20         spacing: 
+00009840: 5475 706c 655b 666c 6f61 742c 2066 6c6f  Tuple[float, flo
+00009850: 6174 5d20 3d20 2831 3030 2c20 3130 3029  at] = (100, 100)
+00009860: 2c0a 2020 2020 2020 2020 616c 6961 733a  ,.        alias:
+00009870: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00009880: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
+00009890: 436f 6d70 6f6e 656e 7452 6566 6572 656e  ComponentReferen
+000098a0: 6365 3a0a 2020 2020 2020 2020 2222 2243  ce:.        """C
+000098b0: 7265 6174 6573 2061 2043 6f6d 706f 6e65  reates a Compone
+000098c0: 6e74 5265 6665 7265 6e63 6520 7265 6665  ntReference refe
+000098d0: 7265 6e63 6520 746f 2061 2043 6f6d 706f  rence to a Compo
+000098e0: 6e65 6e74 2e0a 0a20 2020 2020 2020 2041  nent...        A
+000098f0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00009900: 2063 6f6d 706f 6e65 6e74 3a20 5468 6520   component: The 
+00009910: 7265 6665 7265 6e63 6564 2063 6f6d 706f  referenced compo
+00009920: 6e65 6e74 2e0a 2020 2020 2020 2020 2020  nent..          
+00009930: 2020 636f 6c75 6d6e 733a 204e 756d 6265    columns: Numbe
+00009940: 7220 6f66 2063 6f6c 756d 6e73 2069 6e20  r of columns in 
+00009950: 7468 6520 6172 7261 792e 0a20 2020 2020  the array..     
+00009960: 2020 2020 2020 2072 6f77 733a 204e 756d         rows: Num
+00009970: 6265 7220 6f66 2072 6f77 7320 696e 2074  ber of rows in t
+00009980: 6865 2061 7272 6179 2e0a 2020 2020 2020  he array..      
+00009990: 2020 2020 2020 7370 6163 696e 673a 2061        spacing: a
+000099a0: 7272 6179 2d6c 696b 655b 325d 206f 6620  rray-like[2] of 
+000099b0: 696e 7420 6f72 2066 6c6f 6174 2e0a 2020  int or float..  
+000099c0: 2020 2020 2020 2020 2020 2020 2020 4469                Di
+000099d0: 7374 616e 6365 2062 6574 7765 656e 2061  stance between a
+000099e0: 646a 6163 656e 7420 636f 6c75 6d6e 7320  djacent columns 
+000099f0: 616e 6420 6164 6a61 6365 6e74 2072 6f77  and adjacent row
+00009a00: 732e 0a20 2020 2020 2020 2020 2020 2061  s..            a
+00009a10: 6c69 6173 3a20 7374 7220 6f72 204e 6f6e  lias: str or Non
+00009a20: 652e 2041 6c69 6173 206f 6620 7468 6520  e. Alias of the 
+00009a30: 7265 6665 7265 6e63 6564 2043 6f6d 706f  referenced Compo
+00009a40: 6e65 6e74 2e0a 0a20 2020 2020 2020 2052  nent...        R
+00009a50: 6574 7572 6e73 0a20 2020 2020 2020 2020  eturns.         
+00009a60: 2020 2061 3a20 436f 6d70 6f6e 656e 7452     a: ComponentR
+00009a70: 6566 6572 656e 6365 2063 6f6e 7461 696e  eference contain
+00009a80: 696e 6720 7265 6665 7265 6e63 6573 2074  ing references t
+00009a90: 6f20 7468 6520 436f 6d70 6f6e 656e 742e  o the Component.
+00009aa0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009ab0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+00009ac0: 7374 616e 6365 2863 6f6d 706f 6e65 6e74  stance(component
+00009ad0: 2c20 436f 6d70 6f6e 656e 7429 3a0a 2020  , Component):.  
+00009ae0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00009af0: 5479 7065 4572 726f 7228 2261 6464 5f61  TypeError("add_a
+00009b00: 7272 6179 2829 206e 6565 6473 2061 2043  rray() needs a C
+00009b10: 6f6d 706f 6e65 6e74 206f 626a 6563 742e  omponent object.
+00009b20: 2229 0a20 2020 2020 2020 2072 6566 203d  ").        ref =
+00009b30: 2043 6f6d 706f 6e65 6e74 5265 6665 7265   ComponentRefere
+00009b40: 6e63 6528 0a20 2020 2020 2020 2020 2020  nce(.           
+00009b50: 2063 6f6d 706f 6e65 6e74 3d63 6f6d 706f   component=compo
+00009b60: 6e65 6e74 2c0a 2020 2020 2020 2020 2020  nent,.          
+00009b70: 2020 636f 6c75 6d6e 733d 696e 7428 726f    columns=int(ro
+00009b80: 756e 6428 636f 6c75 6d6e 7329 292c 0a20  und(columns)),. 
+00009b90: 2020 2020 2020 2020 2020 2072 6f77 733d             rows=
+00009ba0: 696e 7428 726f 756e 6428 726f 7773 2929  int(round(rows))
+00009bb0: 2c0a 2020 2020 2020 2020 2020 2020 7370  ,.            sp
+00009bc0: 6163 696e 673d 7370 6163 696e 672c 0a20  acing=spacing,. 
+00009bd0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00009be0: 2072 6566 2e6e 616d 6520 3d20 4e6f 6e65   ref.name = None
+00009bf0: 0a20 2020 2020 2020 2073 656c 662e 5f61  .        self._a
+00009c00: 6464 2872 6566 290a 2020 2020 2020 2020  dd(ref).        
+00009c10: 7365 6c66 2e5f 7265 6769 7374 6572 5f72  self._register_r
+00009c20: 6566 6572 656e 6365 2872 6566 6572 656e  eference(referen
+00009c30: 6365 3d72 6566 2c20 616c 6961 733d 616c  ce=ref, alias=al
+00009c40: 6961 7329 0a20 2020 2020 2020 2072 6574  ias).        ret
+00009c50: 7572 6e20 7265 660a 0a20 2020 2064 6566  urn ref..    def
+00009c60: 2064 6973 7472 6962 7574 6528 0a20 2020   distribute(.   
+00009c70: 2020 2020 2073 656c 662c 2065 6c65 6d65       self, eleme
+00009c80: 6e74 733d 2261 6c6c 222c 2064 6972 6563  nts="all", direc
+00009c90: 7469 6f6e 3d22 7822 2c20 7370 6163 696e  tion="x", spacin
+00009ca0: 673d 3130 302c 2073 6570 6172 6174 696f  g=100, separatio
+00009cb0: 6e3d 5472 7565 2c20 6564 6765 3d22 6365  n=True, edge="ce
+00009cc0: 6e74 6572 220a 2020 2020 293a 0a20 2020  nter".    ):.   
+00009cd0: 2020 2020 2022 2222 4469 7374 7269 6275       """Distribu
+00009ce0: 7465 7320 7468 6520 7370 6563 6966 6965  tes the specifie
+00009cf0: 6420 656c 656d 656e 7473 2069 6e20 7468  d elements in th
+00009d00: 6520 436f 6d70 6f6e 656e 742e 0a0a 2020  e Component...  
+00009d10: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00009d20: 2020 2020 2020 2020 656c 656d 656e 7473          elements
+00009d30: 203a 2061 7272 6179 2d6c 696b 6520 6f66   : array-like of
+00009d40: 206f 626a 6563 7473 206f 7220 2761 6c6c   objects or 'all
+00009d50: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00009d60: 2020 456c 656d 656e 7473 2074 6f20 6469    Elements to di
+00009d70: 7374 7269 6275 7465 2e0a 2020 2020 2020  stribute..      
+00009d80: 2020 2020 2020 6469 7265 6374 696f 6e20        direction 
+00009d90: 3a20 7b27 7827 2c20 2779 277d 0a20 2020  : {'x', 'y'}.   
+00009da0: 2020 2020 2020 2020 2020 2020 2044 6972               Dir
+00009db0: 6563 7469 6f6e 206f 6620 6469 7374 7269  ection of distri
+00009dc0: 6275 7469 6f6e 3b20 6569 7468 6572 2061  bution; either a
+00009dd0: 206c 696e 6520 696e 2074 6865 2078 2d64   line in the x-d
+00009de0: 6972 6563 7469 6f6e 206f 720a 2020 2020  irection or.    
+00009df0: 2020 2020 2020 2020 2020 2020 792d 6469              y-di
+00009e00: 7265 6374 696f 6e2e 0a20 2020 2020 2020  rection..       
+00009e10: 2020 2020 2073 7061 6369 6e67 203a 2069       spacing : i
+00009e20: 6e74 206f 7220 666c 6f61 740a 2020 2020  nt or float.    
+00009e30: 2020 2020 2020 2020 2020 2020 4469 7374              Dist
+00009e40: 616e 6365 2062 6574 7765 656e 2065 6c65  ance between ele
+00009e50: 6d65 6e74 732e 0a20 2020 2020 2020 2020  ments..         
+00009e60: 2020 2073 6570 6172 6174 696f 6e20 3a20     separation : 
+00009e70: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
+00009e80: 2020 2020 2049 6620 5472 7565 2c20 6775       If True, gu
+00009e90: 6172 616e 7465 6573 2065 6c65 6d65 6e74  arantees element
+00009ea0: 7320 6172 6520 7365 7061 7261 7465 6420  s are separated 
+00009eb0: 7769 7468 2061 2066 6978 6564 2073 7061  with a fixed spa
+00009ec0: 6369 6e67 0a20 2020 2020 2020 2020 2020  cing.           
+00009ed0: 2020 2020 2062 6574 7765 656e 3b20 6966       between; if
+00009ee0: 2020 4661 6c73 652c 2065 6c65 6d65 6e74    False, element
+00009ef0: 7320 6172 6520 7370 6163 6564 2065 7665  s are spaced eve
+00009f00: 6e6c 7920 616c 6f6e 6720 6120 6772 6964  nly along a grid
+00009f10: 2e0a 2020 2020 2020 2020 2020 2020 6564  ..            ed
+00009f20: 6765 203a 207b 2778 272c 2027 786d 696e  ge : {'x', 'xmin
+00009f30: 272c 2027 786d 6178 272c 2027 7927 2c20  ', 'xmax', 'y', 
+00009f40: 2779 6d69 6e27 2c20 2779 6d61 7827 7d0a  'ymin', 'ymax'}.
+00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f60: 5768 6963 6820 6564 6765 2074 6f20 7065  Which edge to pe
+00009f70: 7266 6f72 6d20 7468 6520 6469 7374 7269  rform the distri
+00009f80: 6275 7469 6f6e 2061 6c6f 6e67 2028 756e  bution along (un
+00009f90: 7573 6564 2069 660a 2020 2020 2020 2020  used if.        
+00009fa0: 2020 2020 2020 2020 7365 7061 7261 7469          separati
+00009fb0: 6f6e 203d 3d20 5472 7565 290a 0a20 2020  on == True)..   
+00009fc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00009fd0: 2069 6620 656c 656d 656e 7473 203d 3d20   if elements == 
+00009fe0: 2261 6c6c 223a 0a20 2020 2020 2020 2020  "all":.         
+00009ff0: 2020 2065 6c65 6d65 6e74 7320 3d20 7365     elements = se
+0000a000: 6c66 2e70 6f6c 7967 6f6e 7320 2b20 7365  lf.polygons + se
+0000a010: 6c66 2e72 6566 6572 656e 6365 730a 2020  lf.references.  
+0000a020: 2020 2020 2020 5f64 6973 7472 6962 7574        _distribut
+0000a030: 6528 0a20 2020 2020 2020 2020 2020 2065  e(.            e
+0000a040: 6c65 6d65 6e74 733d 656c 656d 656e 7473  lements=elements
+0000a050: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+0000a060: 7265 6374 696f 6e3d 6469 7265 6374 696f  rection=directio
+0000a070: 6e2c 0a20 2020 2020 2020 2020 2020 2073  n,.            s
+0000a080: 7061 6369 6e67 3d73 7061 6369 6e67 2c0a  pacing=spacing,.
+0000a090: 2020 2020 2020 2020 2020 2020 7365 7061              sepa
+0000a0a0: 7261 7469 6f6e 3d73 6570 6172 6174 696f  ration=separatio
+0000a0b0: 6e2c 0a20 2020 2020 2020 2020 2020 2065  n,.            e
+0000a0c0: 6467 653d 6564 6765 2c0a 2020 2020 2020  dge=edge,.      
+0000a0d0: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+0000a0e0: 726e 2073 656c 660a 0a20 2020 2064 6566  rn self..    def
+0000a0f0: 2061 6c69 676e 2873 656c 662c 2065 6c65   align(self, ele
+0000a100: 6d65 6e74 733d 2261 6c6c 222c 2061 6c69  ments="all", ali
+0000a110: 676e 6d65 6e74 3d22 796d 6178 2229 3a0a  gnment="ymax"):.
+0000a120: 2020 2020 2020 2020 2222 2241 6c69 676e          """Align
+0000a130: 2065 6c65 6d65 6e74 7320 696e 2074 6865   elements in the
+0000a140: 2043 6f6d 706f 6e65 6e74 2e0a 0a20 2020   Component...   
+0000a150: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000a160: 2020 2020 2020 2065 6c65 6d65 6e74 7320         elements 
+0000a170: 3a20 6172 7261 792d 6c69 6b65 206f 6620  : array-like of 
+0000a180: 6f62 6a65 6374 732c 206f 7220 2761 6c6c  objects, or 'all
+0000a190: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000a1a0: 2020 456c 656d 656e 7473 2069 6e20 7468    Elements in th
+0000a1b0: 6520 436f 6d70 6f6e 656e 7420 746f 2061  e Component to a
+0000a1c0: 6c69 676e 2e0a 2020 2020 2020 2020 2020  lign..          
+0000a1d0: 2020 616c 6967 6e6d 656e 7420 3a20 7b27    alignment : {'
+0000a1e0: 7827 2c20 2779 272c 2027 786d 696e 272c  x', 'y', 'xmin',
+0000a1f0: 2027 786d 6178 272c 2027 796d 696e 272c   'xmax', 'ymin',
+0000a200: 2027 796d 6178 277d 0a20 2020 2020 2020   'ymax'}.       
+0000a210: 2020 2020 2020 2020 2057 6869 6368 2065           Which e
+0000a220: 6467 6520 746f 2061 6c69 676e 2061 6c6f  dge to align alo
+0000a230: 6e67 2028 652e 672e 2027 796d 6178 2720  ng (e.g. 'ymax' 
+0000a240: 7769 6c6c 206d 6f76 6520 7468 6520 656c  will move the el
+0000a250: 656d 656e 7473 2073 7563 680a 2020 2020  ements such.    
+0000a260: 2020 2020 2020 2020 2020 2020 7468 6174              that
+0000a270: 2061 6c6c 206f 6620 7468 6569 7220 746f   all of their to
+0000a280: 706d 6f73 7420 706f 696e 7473 2061 7265  pmost points are
+0000a290: 2061 6c69 676e 6564 292e 0a20 2020 2020   aligned)..     
+0000a2a0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0000a2b0: 6620 656c 656d 656e 7473 203d 3d20 2261  f elements == "a
+0000a2c0: 6c6c 223a 0a20 2020 2020 2020 2020 2020  ll":.           
+0000a2d0: 2065 6c65 6d65 6e74 7320 3d20 7365 6c66   elements = self
+0000a2e0: 2e70 6f6c 7967 6f6e 7320 2b20 7365 6c66  .polygons + self
+0000a2f0: 2e72 6566 6572 656e 6365 730a 2020 2020  .references.    
+0000a300: 2020 2020 5f61 6c69 676e 2865 6c65 6d65      _align(eleme
+0000a310: 6e74 732c 2061 6c69 676e 6d65 6e74 3d61  nts, alignment=a
+0000a320: 6c69 676e 6d65 6e74 290a 2020 2020 2020  lignment).      
+0000a330: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
+0000a340: 2020 2064 6566 2066 6c61 7474 656e 2873     def flatten(s
+0000a350: 656c 662c 2073 696e 676c 655f 6c61 7965  elf, single_laye
+0000a360: 723a 204f 7074 696f 6e61 6c5b 4c61 7965  r: Optional[Laye
+0000a370: 7253 7065 635d 203d 204e 6f6e 6529 3a0a  rSpec] = None):.
+0000a380: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+0000a390: 6e73 2061 2066 6c61 7474 656e 6564 2063  ns a flattened c
+0000a3a0: 6f70 7920 6f66 2074 6865 2063 6f6d 706f  opy of the compo
+0000a3b0: 6e65 6e74 2e0a 0a20 2020 2020 2020 2046  nent...        F
+0000a3c0: 6c61 7474 656e 7320 7468 6520 6869 6572  lattens the hier
+0000a3d0: 6172 6368 7920 6f66 2074 6865 2043 6f6d  archy of the Com
+0000a3e0: 706f 6e65 6e74 2073 7563 6820 7468 6174  ponent such that
+0000a3f0: 2074 6865 7265 2061 7265 206e 6f20 6c6f   there are no lo
+0000a400: 6e67 6572 0a20 2020 2020 2020 2061 6e79  nger.        any
+0000a410: 2072 6566 6572 656e 6365 7320 746f 206f   references to o
+0000a420: 7468 6572 2043 6f6d 706f 6e65 6e74 732e  ther Components.
+0000a430: 2041 6c6c 2070 6f6c 7967 6f6e 7320 616e   All polygons an
+0000a440: 6420 6c61 6265 6c73 2066 726f 6d0a 2020  d labels from.  
+0000a450: 2020 2020 2020 756e 6465 726c 7969 6e67        underlying
+0000a460: 2072 6566 6572 656e 6365 7320 6172 6520   references are 
+0000a470: 636f 7069 6564 2061 6e64 2070 6c61 6365  copied and place
+0000a480: 6420 696e 2074 6865 2074 6f70 2d6c 6576  d in the top-lev
+0000a490: 656c 2043 6f6d 706f 6e65 6e74 2e0a 2020  el Component..  
+0000a4a0: 2020 2020 2020 4966 2073 696e 676c 655f        If single_
+0000a4b0: 6c61 7965 7220 6973 2073 7065 6369 6669  layer is specifi
+0000a4c0: 6564 2c20 616c 6c20 706f 6c79 676f 6e73  ed, all polygons
+0000a4d0: 2061 7265 206d 6f76 6564 2074 6f20 7468   are moved to th
+0000a4e0: 6174 206c 6179 6572 2e0a 0a20 2020 2020  at layer...     
+0000a4f0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000a500: 2020 2020 2073 696e 676c 655f 6c61 7965       single_laye
+0000a510: 723a 206d 6f76 6520 616c 6c20 706f 6c79  r: move all poly
+0000a520: 676f 6e73 2061 7265 206d 6f76 6564 2074  gons are moved t
+0000a530: 6f20 7468 6520 7370 6563 6966 6965 6420  o the specified 
+0000a540: 286f 7074 696f 6e61 6c29 2e0a 2020 2020  (optional)..    
+0000a550: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000a560: 636f 6d70 6f6e 656e 745f 666c 6174 203d  component_flat =
+0000a570: 2043 6f6d 706f 6e65 6e74 2829 0a0a 2020   Component()..  
+0000a580: 2020 2020 2020 5f63 656c 6c20 3d20 7365        _cell = se
+0000a590: 6c66 2e5f 6365 6c6c 2e63 6f70 7928 6e61  lf._cell.copy(na
+0000a5a0: 6d65 3d63 6f6d 706f 6e65 6e74 5f66 6c61  me=component_fla
+0000a5b0: 742e 6e61 6d65 290a 2020 2020 2020 2020  t.name).        
+0000a5c0: 5f63 656c 6c20 3d20 5f63 656c 6c2e 666c  _cell = _cell.fl
+0000a5d0: 6174 7465 6e28 290a 2020 2020 2020 2020  atten().        
+0000a5e0: 636f 6d70 6f6e 656e 745f 666c 6174 2e5f  component_flat._
+0000a5f0: 6365 6c6c 203d 205f 6365 6c6c 0a20 2020  cell = _cell.   
+0000a600: 2020 2020 2069 6620 7369 6e67 6c65 5f6c       if single_l
+0000a610: 6179 6572 2069 7320 6e6f 7420 4e6f 6e65  ayer is not None
+0000a620: 3a0a 2020 2020 2020 2020 2020 2020 6672  :.            fr
+0000a630: 6f6d 2067 6473 6661 6374 6f72 7920 696d  om gdsfactory im
+0000a640: 706f 7274 2067 6574 5f6c 6179 6572 0a0a  port get_layer..
+0000a650: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+0000a660: 722c 2064 6174 6174 7970 6520 3d20 6765  r, datatype = ge
+0000a670: 745f 6c61 7965 7228 7369 6e67 6c65 5f6c  t_layer(single_l
+0000a680: 6179 6572 290a 2020 2020 2020 2020 2020  ayer).          
+0000a690: 2020 666f 7220 706f 6c79 676f 6e20 696e    for polygon in
+0000a6a0: 205f 6365 6c6c 2e70 6f6c 7967 6f6e 733a   _cell.polygons:
+0000a6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a6c0: 2070 6f6c 7967 6f6e 2e6c 6179 6572 203d   polygon.layer =
+0000a6d0: 206c 6179 6572 0a20 2020 2020 2020 2020   layer.         
+0000a6e0: 2020 2020 2020 2070 6f6c 7967 6f6e 2e64         polygon.d
+0000a6f0: 6174 6174 7970 6520 3d20 6461 7461 7479  atatype = dataty
+0000a700: 7065 0a20 2020 2020 2020 2020 2020 2066  pe.            f
+0000a710: 6f72 2070 6174 6820 696e 205f 6365 6c6c  or path in _cell
+0000a720: 2e70 6174 6873 3a0a 2020 2020 2020 2020  .paths:.        
+0000a730: 2020 2020 2020 2020 7061 7468 2e73 6574          path.set
+0000a740: 5f6c 6179 6572 7328 6c61 7965 7229 0a20  _layers(layer). 
+0000a750: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000a760: 6174 682e 7365 745f 6461 7461 7479 7065  ath.set_datatype
+0000a770: 7328 6461 7461 7479 7065 290a 0a20 2020  s(datatype)..   
+0000a780: 2020 2020 2063 6f6d 706f 6e65 6e74 5f66       component_f
+0000a790: 6c61 742e 696e 666f 203d 2073 656c 662e  lat.info = self.
+0000a7a0: 696e 666f 2e63 6f70 7928 290a 2020 2020  info.copy().    
+0000a7b0: 2020 2020 636f 6d70 6f6e 656e 745f 666c      component_fl
+0000a7c0: 6174 2e61 6464 5f70 6f72 7473 2873 656c  at.add_ports(sel
+0000a7d0: 662e 706f 7274 7329 0a20 2020 2020 2020  f.ports).       
+0000a7e0: 2072 6574 7572 6e20 636f 6d70 6f6e 656e   return componen
+0000a7f0: 745f 666c 6174 0a0a 2020 2020 6465 6620  t_flat..    def 
+0000a800: 666c 6174 7465 6e5f 7265 6665 7265 6e63  flatten_referenc
+0000a810: 6528 7365 6c66 2c20 7265 663a 2043 6f6d  e(self, ref: Com
+0000a820: 706f 6e65 6e74 5265 6665 7265 6e63 6529  ponentReference)
+0000a830: 3a0a 2020 2020 2020 2020 2222 2246 726f  :.        """Fro
+0000a840: 6d20 6578 6973 7469 6e67 2063 656c 6c20  m existing cell 
+0000a850: 7265 706c 6163 6573 2072 6566 6572 656e  replaces referen
+0000a860: 6365 2077 6974 6820 6120 666c 6174 7465  ce with a flatte
+0000a870: 6e20 7265 6665 7265 6e63 6520 5c0a 2020  n reference \.  
+0000a880: 2020 2020 2020 7768 6963 6820 6861 7320        which has 
+0000a890: 7468 6520 7472 616e 7366 6f72 6d61 7469  the transformati
+0000a8a0: 6f6e 7320 616c 7265 6164 7920 6170 706c  ons already appl
+0000a8b0: 6965 642e 0a0a 2020 2020 2020 2020 5472  ied...        Tr
+0000a8c0: 616e 7366 6f72 6d65 6420 7265 6665 7265  ansformed refere
+0000a8d0: 6e63 6520 6b65 6570 7320 7468 6520 6f72  nce keeps the or
+0000a8e0: 6967 696e 616c 206e 616d 652e 0a0a 2020  iginal name...  
+0000a8f0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0000a900: 2020 2020 2020 2020 7265 663a 2074 6865          ref: the
+0000a910: 2072 6566 6572 656e 6365 2074 6f20 666c   reference to fl
+0000a920: 6174 7465 6e20 696e 746f 2061 206e 6577  atten into a new
+0000a930: 2063 656c 6c2e 0a0a 2020 2020 2020 2020   cell...        
+0000a940: 2222 220a 2020 2020 2020 2020 6672 6f6d  """.        from
+0000a950: 2067 6473 6661 6374 6f72 792e 6675 6e63   gdsfactory.func
+0000a960: 7469 6f6e 7320 696d 706f 7274 2074 7261  tions import tra
+0000a970: 6e73 666f 726d 6564 0a0a 2020 2020 2020  nsformed..      
+0000a980: 2020 7365 6c66 2e72 656d 6f76 6528 7265    self.remove(re
+0000a990: 6629 0a20 2020 2020 2020 206e 6577 5f63  f).        new_c
+0000a9a0: 6f6d 706f 6e65 6e74 203d 2074 7261 6e73  omponent = trans
+0000a9b0: 666f 726d 6564 2872 6566 2c20 6465 636f  formed(ref, deco
+0000a9c0: 7261 746f 723d 4e6f 6e65 290a 2020 2020  rator=None).    
+0000a9d0: 2020 2020 7365 6c66 2e61 6464 5f72 6566      self.add_ref
+0000a9e0: 286e 6577 5f63 6f6d 706f 6e65 6e74 2c20  (new_component, 
+0000a9f0: 616c 6961 733d 7265 662e 6e61 6d65 290a  alias=ref.name).
+0000aa00: 0a20 2020 2064 6566 2061 6464 5f72 6566  .    def add_ref
+0000aa10: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+0000aa20: 636f 6d70 6f6e 656e 743a 2043 6f6d 706f  component: Compo
+0000aa30: 6e65 6e74 2c20 616c 6961 733a 204f 7074  nent, alias: Opt
+0000aa40: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000aa50: 652c 202a 2a6b 7761 7267 730a 2020 2020  e, **kwargs.    
+0000aa60: 2920 2d3e 2043 6f6d 706f 6e65 6e74 5265  ) -> ComponentRe
+0000aa70: 6665 7265 6e63 653a 0a20 2020 2020 2020  ference:.       
+0000aa80: 2022 2222 4164 6420 436f 6d70 6f6e 656e   """Add Componen
+0000aa90: 7452 6566 6572 656e 6365 2074 6f20 7468  tReference to th
+0000aaa0: 6520 6375 7272 656e 7420 436f 6d70 6f6e  e current Compon
+0000aab0: 656e 742e 0a0a 2020 2020 2020 2020 4172  ent...        Ar
+0000aac0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000aad0: 636f 6d70 6f6e 656e 743a 2043 6f6d 706f  component: Compo
+0000aae0: 6e65 6e74 2e0a 2020 2020 2020 2020 2020  nent..          
+0000aaf0: 2020 616c 6961 733a 206e 616d 6564 5f72    alias: named_r
+0000ab00: 6566 6572 656e 6365 732e 0a0a 2020 2020  eferences...    
+0000ab10: 2020 2020 4b65 7977 6f72 6420 4172 6773      Keyword Args
+0000ab20: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+0000ab30: 6c75 6d6e 733a 204e 756d 6265 7220 6f66  lumns: Number of
+0000ab40: 2063 6f6c 756d 6e73 2069 6e20 7468 6520   columns in the 
+0000ab50: 6172 7261 792e 0a20 2020 2020 2020 2020  array..         
+0000ab60: 2020 2072 6f77 733a 204e 756d 6265 7220     rows: Number 
+0000ab70: 6f66 2072 6f77 7320 696e 2074 6865 2061  of rows in the a
+0000ab80: 7272 6179 2e0a 2020 2020 2020 2020 2020  rray..          
+0000ab90: 2020 7370 6163 696e 673a 2044 6973 7461    spacing: Dista
+0000aba0: 6e63 6573 2062 6574 7765 656e 2061 646a  nces between adj
+0000abb0: 6163 656e 7420 636f 6c75 6d6e 7320 616e  acent columns an
+0000abc0: 6420 6164 6a61 6365 6e74 2072 6f77 732e  d adjacent rows.
+0000abd0: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
+0000abe0: 6769 6e3a 2061 7272 6179 2d6c 696b 655b  gin: array-like[
+0000abf0: 325d 206f 6620 696e 7420 6f72 2066 6c6f  2] of int or flo
+0000ac00: 6174 0a20 2020 2020 2020 2020 2020 2020  at.             
+0000ac10: 2020 2050 6f73 6974 696f 6e20 7768 6572     Position wher
+0000ac20: 6520 7468 6520 6365 6c6c 2069 7320 696e  e the cell is in
+0000ac30: 7365 7274 6564 2e0a 2020 2020 2020 2020  serted..        
+0000ac40: 2020 2020 726f 7461 7469 6f6e 203a 2069      rotation : i
+0000ac50: 6e74 206f 7220 666c 6f61 740a 2020 2020  nt or float.    
+0000ac60: 2020 2020 2020 2020 2020 2020 416e 676c              Angl
+0000ac70: 6520 6f66 2072 6f74 6174 696f 6e20 6f66  e of rotation of
+0000ac80: 2074 6865 2072 6566 6572 656e 6365 2028   the reference (
+0000ac90: 696e 2060 6465 6772 6565 7360 292e 0a20  in `degrees`).. 
+0000aca0: 2020 2020 2020 2020 2020 206d 6167 6e69             magni
+0000acb0: 6669 6361 7469 6f6e 203a 2069 6e74 206f  fication : int o
+0000acc0: 7220 666c 6f61 740a 2020 2020 2020 2020  r float.        
+0000acd0: 2020 2020 2020 2020 4d61 676e 6966 6963          Magnific
+0000ace0: 6174 696f 6e20 6661 6374 6f72 2066 6f72  ation factor for
+0000acf0: 2074 6865 2072 6566 6572 656e 6365 2e0a   the reference..
+0000ad00: 2020 2020 2020 2020 2020 2020 785f 7265              x_re
+0000ad10: 666c 6563 7469 6f6e 203a 2062 6f6f 6c0a  flection : bool.
+0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad30: 4966 2054 7275 652c 2074 6865 2072 6566  If True, the ref
+0000ad40: 6572 656e 6365 2069 7320 7265 666c 6563  erence is reflec
+0000ad50: 7465 6420 7061 7261 6c6c 656c 2074 6f20  ted parallel to 
+0000ad60: 7468 6520 7820 6469 7265 6374 696f 6e0a  the x direction.
+0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad80: 6265 666f 7265 2062 6569 6e67 2072 6f74  before being rot
+0000ad90: 6174 6564 2e0a 2020 2020 2020 2020 2020  ated..          
+0000ada0: 2020 6e61 6d65 203a 2073 7472 2028 6f70    name : str (op
+0000adb0: 7469 6f6e 616c 290a 2020 2020 2020 2020  tional).        
+0000adc0: 2020 2020 2020 2020 4120 6e61 6d65 2066          A name f
+0000add0: 6f72 2074 6865 2072 6566 6572 656e 6365  or the reference
+0000ade0: 2028 6966 2070 726f 7669 6465 6429 2e0a   (if provided)..
+0000adf0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000ae00: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+0000ae10: 7374 616e 6365 2863 6f6d 706f 6e65 6e74  stance(component
+0000ae20: 2c20 436f 6d70 6f6e 656e 7429 3a0a 2020  , Component):.  
+0000ae30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000ae40: 5479 7065 4572 726f 7228 6622 7479 7065  TypeError(f"type
+0000ae50: 203d 207b 7479 7065 2843 6f6d 706f 6e65   = {type(Compone
+0000ae60: 6e74 297d 206e 6565 6473 2074 6f20 6265  nt)} needs to be
+0000ae70: 2061 2043 6f6d 706f 6e65 6e74 2e22 290a   a Component.").
+0000ae80: 2020 2020 2020 2020 7265 6620 3d20 436f          ref = Co
+0000ae90: 6d70 6f6e 656e 7452 6566 6572 656e 6365  mponentReference
+0000aea0: 2863 6f6d 706f 6e65 6e74 2c20 2a2a 6b77  (component, **kw
+0000aeb0: 6172 6773 290a 2020 2020 2020 2020 7365  args).        se
+0000aec0: 6c66 2e5f 6164 6428 7265 6629 0a20 2020  lf._add(ref).   
+0000aed0: 2020 2020 2073 656c 662e 5f72 6567 6973       self._regis
+0000aee0: 7465 725f 7265 6665 7265 6e63 6528 7265  ter_reference(re
+0000aef0: 6665 7265 6e63 653d 7265 662c 2061 6c69  ference=ref, ali
+0000af00: 6173 3d61 6c69 6173 290a 2020 2020 2020  as=alias).      
+0000af10: 2020 7265 7475 726e 2072 6566 0a0a 2020    return ref..  
+0000af20: 2020 6465 6620 5f72 6567 6973 7465 725f    def _register_
+0000af30: 7265 6665 7265 6e63 6528 0a20 2020 2020  reference(.     
+0000af40: 2020 2073 656c 662c 2072 6566 6572 656e     self, referen
+0000af50: 6365 3a20 436f 6d70 6f6e 656e 7452 6566  ce: ComponentRef
+0000af60: 6572 656e 6365 2c20 616c 6961 733a 204f  erence, alias: O
+0000af70: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000af80: 6f6e 650a 2020 2020 2920 2d3e 204e 6f6e  one.    ) -> Non
+0000af90: 653a 0a20 2020 2020 2020 2063 6f6d 706f  e:.        compo
+0000afa0: 6e65 6e74 203d 2072 6566 6572 656e 6365  nent = reference
+0000afb0: 2e70 6172 656e 740a 2020 2020 2020 2020  .parent.        
+0000afc0: 7265 6665 7265 6e63 652e 6f77 6e65 7220  reference.owner 
+0000afd0: 3d20 7365 6c66 0a0a 2020 2020 2020 2020  = self..        
+0000afe0: 6966 2061 6c69 6173 2069 7320 4e6f 6e65  if alias is None
+0000aff0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000b000: 2072 6566 6572 656e 6365 2e6e 616d 6520   reference.name 
+0000b010: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000b020: 2020 2020 2020 2020 2020 2020 2061 6c69               ali
+0000b030: 6173 203d 2072 6566 6572 656e 6365 2e6e  as = reference.n
+0000b040: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+0000b050: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000b060: 2020 2020 2020 7072 6566 6978 203d 2028        prefix = (
+0000b070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b080: 2020 2020 2063 6f6d 706f 6e65 6e74 2e73       component.s
+0000b090: 6574 7469 6e67 732e 6675 6e63 7469 6f6e  ettings.function
+0000b0a0: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
+0000b0b0: 2020 2020 2020 2020 2020 6966 2068 6173            if has
+0000b0c0: 6174 7472 2863 6f6d 706f 6e65 6e74 2c20  attr(component, 
+0000b0d0: 2273 6574 7469 6e67 7322 290a 2020 2020  "settings").    
+0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0f0: 616e 6420 6861 7361 7474 7228 636f 6d70  and hasattr(comp
+0000b100: 6f6e 656e 742e 7365 7474 696e 6773 2c20  onent.settings, 
+0000b110: 2266 756e 6374 696f 6e5f 6e61 6d65 2229  "function_name")
+0000b120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b130: 2020 2020 2065 6c73 6520 636f 6d70 6f6e       else compon
+0000b140: 656e 742e 6e61 6d65 0a20 2020 2020 2020  ent.name.       
+0000b150: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000b160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b170: 5f72 6566 6572 656e 6365 5f6e 616d 6573  _reference_names
+0000b180: 5f63 6f75 6e74 6572 2e75 7064 6174 6528  _counter.update(
+0000b190: 7b70 7265 6669 783a 2031 7d29 0a20 2020  {prefix: 1}).   
+0000b1a0: 2020 2020 2020 2020 2020 2020 2061 6c69               ali
+0000b1b0: 6173 203d 2066 227b 7072 6566 6978 7d5f  as = f"{prefix}_
+0000b1c0: 7b73 656c 662e 5f72 6566 6572 656e 6365  {self._reference
+0000b1d0: 5f6e 616d 6573 5f63 6f75 6e74 6572 5b70  _names_counter[p
+0000b1e0: 7265 6669 785d 7d22 0a0a 2020 2020 2020  refix]}"..      
+0000b1f0: 2020 2020 2020 2020 2020 7768 696c 6520            while 
+0000b200: 616c 6961 7320 696e 2073 656c 662e 5f6e  alias in self._n
+0000b210: 616d 6564 5f72 6566 6572 656e 6365 733a  amed_references:
+0000b220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b230: 2020 2020 2073 656c 662e 5f72 6566 6572       self._refer
+0000b240: 656e 6365 5f6e 616d 6573 5f63 6f75 6e74  ence_names_count
+0000b250: 6572 2e75 7064 6174 6528 7b70 7265 6669  er.update({prefi
+0000b260: 783a 2031 7d29 0a20 2020 2020 2020 2020  x: 1}).         
+0000b270: 2020 2020 2020 2020 2020 2061 6c69 6173             alias
+0000b280: 203d 2066 227b 7072 6566 6978 7d5f 7b73   = f"{prefix}_{s
+0000b290: 656c 662e 5f72 6566 6572 656e 6365 5f6e  elf._reference_n
+0000b2a0: 616d 6573 5f63 6f75 6e74 6572 5b70 7265  ames_counter[pre
+0000b2b0: 6669 785d 7d22 0a0a 2020 2020 2020 2020  fix]}"..        
+0000b2c0: 7265 6665 7265 6e63 652e 6e61 6d65 203d  reference.name =
+0000b2d0: 2061 6c69 6173 0a20 2020 2020 2020 2073   alias.        s
+0000b2e0: 656c 662e 5f6e 616d 6564 5f72 6566 6572  elf._named_refer
+0000b2f0: 656e 6365 735b 616c 6961 735d 203d 2072  ences[alias] = r
+0000b300: 6566 6572 656e 6365 0a0a 2020 2020 4070  eference..    @p
+0000b310: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000b320: 6c61 7965 7273 2873 656c 6629 202d 3e20  layers(self) -> 
+0000b330: 5365 745b 5475 706c 655b 696e 742c 2069  Set[Tuple[int, i
+0000b340: 6e74 5d5d 3a0a 2020 2020 2020 2020 2222  nt]]:.        ""
+0000b350: 2252 6574 7572 6e73 2061 2073 6574 206f  "Returns a set o
+0000b360: 6620 7468 6520 4c61 7965 7273 2069 6e20  f the Layers in 
+0000b370: 7468 6520 436f 6d70 6f6e 656e 742e 2222  the Component.""
+0000b380: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+0000b390: 2073 656c 662e 6765 745f 6c61 7965 7273   self.get_layers
+0000b3a0: 2829 0a0a 2020 2020 6465 6620 6765 745f  ()..    def get_
+0000b3b0: 6c61 7965 7273 2873 656c 6629 202d 3e20  layers(self) -> 
+0000b3c0: 5365 745b 5475 706c 655b 696e 742c 2069  Set[Tuple[int, i
+0000b3d0: 6e74 5d5d 3a0a 2020 2020 2020 2020 2222  nt]]:.        ""
+0000b3e0: 2252 6574 7572 6e20 6120 7365 7420 6f66  "Return a set of
+0000b3f0: 2028 6c61 7965 722c 2064 6174 6174 7970   (layer, datatyp
+0000b400: 6529 2e0a 0a20 2020 2020 2020 202e 2e20  e)...        .. 
+0000b410: 636f 6465 203a 3a0a 0a20 2020 2020 2020  code ::..       
+0000b420: 2020 2020 2069 6d70 6f72 7420 6764 7366       import gdsf
+0000b430: 6163 746f 7279 2061 7320 6766 0a20 2020  actory as gf.   
+0000b440: 2020 2020 2020 2020 2067 662e 636f 6d70           gf.comp
+0000b450: 6f6e 656e 7473 2e73 7472 6169 6768 7428  onents.straight(
+0000b460: 292e 6765 745f 6c61 7965 7273 2829 203d  ).get_layers() =
+0000b470: 3d20 7b28 312c 2030 292c 2028 3131 312c  = {(1, 0), (111,
+0000b480: 2030 297d 0a20 2020 2020 2020 2022 2222   0)}.        """
+0000b490: 0a20 2020 2020 2020 2070 6f6c 7967 6f6e  .        polygon
+0000b4a0: 7320 3d20 7365 6c66 2e5f 6365 6c6c 2e67  s = self._cell.g
+0000b4b0: 6574 5f70 6f6c 7967 6f6e 7328 6465 7074  et_polygons(dept
+0000b4c0: 683d 4e6f 6e65 290a 2020 2020 2020 2020  h=None).        
+0000b4d0: 7265 7475 726e 207b 2870 6f6c 7967 6f6e  return {(polygon
+0000b4e0: 2e6c 6179 6572 2c20 706f 6c79 676f 6e2e  .layer, polygon.
+0000b4f0: 6461 7461 7479 7065 2920 666f 7220 706f  datatype) for po
+0000b500: 6c79 676f 6e20 696e 2070 6f6c 7967 6f6e  lygon in polygon
+0000b510: 737d 0a0a 2020 2020 6465 6620 6765 745f  s}..    def get_
+0000b520: 6c61 7965 725f 6e61 6d65 7328 7365 6c66  layer_names(self
+0000b530: 2920 2d3e 204c 6973 745b 5475 706c 655b  ) -> List[Tuple[
+0000b540: 696e 742c 2069 6e74 5d5d 3a0a 2020 2020  int, int]]:.    
+0000b550: 2020 2020 2222 2252 6574 7572 6e20 6c61      """Return la
+0000b560: 7965 7220 6e61 6d65 7320 7573 6564 2069  yer names used i
+0000b570: 6e20 7468 6520 6465 7369 676e 2e0a 0a20  n the design... 
+0000b580: 2020 2020 2020 202e 2e20 636f 6465 203a         .. code :
+0000b590: 3a0a 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0000b5a0: 6d70 6f72 7420 6764 7366 6163 746f 7279  mport gdsfactory
+0000b5b0: 2061 7320 6766 0a20 2020 2020 2020 2020   as gf.         
+0000b5c0: 2020 2067 662e 636f 6d70 6f6e 656e 7473     gf.components
+0000b5d0: 2e73 7472 6169 6768 7428 292e 6765 745f  .straight().get_
+0000b5e0: 6e61 6d65 7328 2920 3d3d 205b 2757 4727  names() == ['WG'
+0000b5f0: 5d0a 2020 2020 2020 2020 2222 220a 2020  ].        """.  
+0000b600: 2020 2020 2020 696d 706f 7274 2067 6473        import gds
+0000b610: 6661 6374 6f72 7920 6173 2067 660a 0a20  factory as gf.. 
+0000b620: 2020 2020 2020 2050 444b 203d 2067 662e         PDK = gf.
+0000b630: 6765 745f 6163 7469 7665 5f70 646b 2829  get_active_pdk()
+0000b640: 0a20 2020 2020 2020 204c 4159 4552 5320  .        LAYERS 
+0000b650: 3d20 5044 4b2e 6c61 7965 7273 0a20 2020  = PDK.layers.   
+0000b660: 2020 2020 206e 616d 655f 746f 5f6c 6179       name_to_lay
+0000b670: 6572 203d 2064 6963 7428 4c41 5945 5253  er = dict(LAYERS
+0000b680: 290a 2020 2020 2020 2020 6c61 7965 725f  ).        layer_
+0000b690: 746f 5f6e 616d 6520 3d20 7b76 3a20 6b20  to_name = {v: k 
+0000b6a0: 666f 7220 6b2c 2076 2069 6e20 6e61 6d65  for k, v in name
+0000b6b0: 5f74 6f5f 6c61 7965 722e 6974 656d 7328  _to_layer.items(
+0000b6c0: 297d 0a20 2020 2020 2020 206c 6179 6572  )}.        layer
+0000b6d0: 5f6e 616d 6573 203d 205b 5d0a 0a20 2020  _names = []..   
+0000b6e0: 2020 2020 2066 6f72 206c 6179 6572 2069       for layer i
+0000b6f0: 6e20 7365 6c66 2e6c 6179 6572 733a 0a20  n self.layers:. 
+0000b700: 2020 2020 2020 2020 2020 2069 6620 6c61             if la
+0000b710: 7965 7220 6e6f 7420 696e 206c 6179 6572  yer not in layer
+0000b720: 5f74 6f5f 6e61 6d65 3a0a 2020 2020 2020  _to_name:.      
+0000b730: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+0000b740: 6773 2e77 6172 6e28 6622 7b6c 6179 6572  gs.warn(f"{layer
+0000b750: 7d20 6e6f 7420 696e 204c 6179 6572 4d61  } not in LayerMa
+0000b760: 702e 2e22 290a 2020 2020 2020 2020 2020  p..").          
+0000b770: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000b780: 2020 2020 2020 2020 6c61 7965 725f 6e61          layer_na
+0000b790: 6d65 732e 6170 7065 6e64 286c 6179 6572  mes.append(layer
+0000b7a0: 5f74 6f5f 6e61 6d65 5b6c 6179 6572 5d29  _to_name[layer])
+0000b7b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b7c0: 6c61 7965 725f 6e61 6d65 730a 0a20 2020  layer_names..   
+0000b7d0: 2064 6566 205f 6970 7974 686f 6e5f 6469   def _ipython_di
+0000b7e0: 7370 6c61 795f 2873 656c 6629 202d 3e20  splay_(self) -> 
+0000b7f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000b800: 2253 686f 7720 6765 6f6d 6574 7279 2069  "Show geometry i
+0000b810: 6e20 4b4c 6179 6f75 7420 616e 6420 696e  n KLayout and in
+0000b820: 206d 6174 706c 6f74 6c69 6220 666f 7220   matplotlib for 
+0000b830: 4a75 7079 7465 7220 4e6f 7465 626f 6f6b  Jupyter Notebook
+0000b840: 732e 2222 220a 2020 2020 2020 2020 7365  s.""".        se
+0000b850: 6c66 2e73 686f 7728 7368 6f77 5f70 6f72  lf.show(show_por
+0000b860: 7473 3d54 7275 6529 2020 2320 7368 6f77  ts=True)  # show
+0000b870: 2069 6e20 6b6c 6179 6f75 740a 2020 2020   in klayout.    
+0000b880: 2020 2020 7365 6c66 2e70 6c6f 745f 6b6c      self.plot_kl
+0000b890: 6179 6f75 7428 290a 2020 2020 2020 2020  ayout().        
+0000b8a0: 7072 696e 7428 7365 6c66 290a 0a20 2020  print(self)..   
+0000b8b0: 2064 6566 2061 6464 5f70 696e 735f 7472   def add_pins_tr
+0000b8c0: 6961 6e67 6c65 280a 2020 2020 2020 2020  iangle(.        
+0000b8d0: 7365 6c66 2c0a 2020 2020 2020 2020 706f  self,.        po
+0000b8e0: 7274 5f6d 6172 6b65 725f 6c61 7965 723a  rt_marker_layer:
+0000b8f0: 204c 6179 6572 203d 2028 312c 2031 3029   Layer = (1, 10)
+0000b900: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0000b910: 2022 2222 5265 7475 726e 7320 636f 6d70   """Returns comp
+0000b920: 6f6e 656e 7420 7769 7468 2074 7269 616e  onent with trian
+0000b930: 6775 6c61 7220 7069 6e73 2e22 2222 0a20  gular pins.""". 
+0000b940: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
+0000b950: 6163 746f 7279 2e61 6464 5f70 696e 7320  actory.add_pins 
+0000b960: 696d 706f 7274 2061 6464 5f70 696e 735f  import add_pins_
+0000b970: 7472 6961 6e67 6c65 0a0a 2020 2020 2020  triangle..      
+0000b980: 2020 636f 6d70 6f6e 656e 7420 3d20 7365    component = se
+0000b990: 6c66 2e63 6f70 7928 290a 2020 2020 2020  lf.copy().      
+0000b9a0: 2020 636f 6d70 6f6e 656e 742e 6e61 6d65    component.name
+0000b9b0: 203d 2073 656c 662e 6e61 6d65 0a20 2020   = self.name.   
+0000b9c0: 2020 2020 2061 6464 5f70 696e 735f 7472       add_pins_tr
+0000b9d0: 6961 6e67 6c65 2863 6f6d 706f 6e65 6e74  iangle(component
+0000b9e0: 3d63 6f6d 706f 6e65 6e74 2c20 6c61 7965  =component, laye
+0000b9f0: 723d 706f 7274 5f6d 6172 6b65 725f 6c61  r=port_marker_la
+0000ba00: 7965 7229 0a20 2020 2020 2020 2072 6574  yer).        ret
+0000ba10: 7572 6e20 636f 6d70 6f6e 656e 740a 0a20  urn component.. 
+0000ba20: 2020 2064 6566 2070 6c6f 745f 7769 6467     def plot_widg
+0000ba30: 6574 280a 2020 2020 2020 2020 7365 6c66  et(.        self
+0000ba40: 2c0a 2020 2020 2020 2020 7368 6f77 5f70  ,.        show_p
+0000ba50: 6f72 7473 3a20 626f 6f6c 203d 2054 7275  orts: bool = Tru
+0000ba60: 652c 0a20 2020 2020 2020 2070 6f72 745f  e,.        port_
+0000ba70: 6d61 726b 6572 5f6c 6179 6572 3a20 4c61  marker_layer: La
+0000ba80: 7965 7220 3d20 2831 2c20 3130 292c 0a20  yer = (1, 10),. 
+0000ba90: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0000baa0: 2252 6574 7572 6e73 2069 7079 7468 6f6e  "Returns ipython
+0000bab0: 2077 6964 6765 7420 666f 7220 6b6c 6179   widget for klay
+0000bac0: 6f75 7420 7669 7375 616c 697a 6174 696f  out visualizatio
+0000bad0: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
+0000bae0: 3a0a 2020 2020 2020 2020 2020 2020 7368  :.            sh
+0000baf0: 6f77 5f70 6f72 7473 3a20 7368 6f77 7320  ow_ports: shows 
+0000bb00: 636f 6d70 6f6e 656e 7420 7769 7468 2070  component with p
+0000bb10: 6f72 7420 6d61 726b 6572 7320 616e 6420  ort markers and 
+0000bb20: 6c61 6265 6c73 2e0a 2020 2020 2020 2020  labels..        
+0000bb30: 2020 2020 706f 7274 5f6d 6172 6b65 725f      port_marker_
+0000bb40: 6c61 7965 723a 2066 6f72 2074 6865 2070  layer: for the p
+0000bb50: 6f72 7473 2e0a 2020 2020 2020 2020 2222  orts..        ""
+0000bb60: 220a 2020 2020 2020 2020 6672 6f6d 2067  ".        from g
+0000bb70: 6473 6661 6374 6f72 792e 7064 6b20 696d  dsfactory.pdk im
+0000bb80: 706f 7274 2067 6574 5f6c 6179 6572 5f76  port get_layer_v
+0000bb90: 6965 7773 0a20 2020 2020 2020 2066 726f  iews.        fro
+0000bba0: 6d20 6764 7366 6163 746f 7279 2e77 6964  m gdsfactory.wid
+0000bbb0: 6765 7473 2e6c 6179 6f75 745f 7669 6577  gets.layout_view
+0000bbc0: 6572 2069 6d70 6f72 7420 4c61 796f 7574  er import Layout
+0000bbd0: 5669 6577 6572 0a20 2020 2020 2020 2066  Viewer.        f
+0000bbe0: 726f 6d20 4950 7974 686f 6e2e 6469 7370  rom IPython.disp
+0000bbf0: 6c61 7920 696d 706f 7274 2064 6973 706c  lay import displ
+0000bc00: 6179 0a0a 2020 2020 2020 2020 636f 6d70  ay..        comp
+0000bc10: 6f6e 656e 7420 3d20 280a 2020 2020 2020  onent = (.      
+0000bc20: 2020 2020 2020 7365 6c66 2e61 6464 5f70        self.add_p
+0000bc30: 696e 735f 7472 6961 6e67 6c65 2870 6f72  ins_triangle(por
+0000bc40: 745f 6d61 726b 6572 5f6c 6179 6572 3d70  t_marker_layer=p
+0000bc50: 6f72 745f 6d61 726b 6572 5f6c 6179 6572  ort_marker_layer
+0000bc60: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000bc70: 2073 686f 775f 706f 7274 730a 2020 2020   show_ports.    
+0000bc80: 2020 2020 2020 2020 656c 7365 2073 656c          else sel
+0000bc90: 660a 2020 2020 2020 2020 290a 0a20 2020  f.        )..   
+0000bca0: 2020 2020 2067 6473 7061 7468 203d 2063       gdspath = c
+0000bcb0: 6f6d 706f 6e65 6e74 2e77 7269 7465 5f67  omponent.write_g
+0000bcc0: 6473 286c 6f67 6769 6e67 3d46 616c 7365  ds(logging=False
+0000bcd0: 290a 2020 2020 2020 2020 6c79 705f 7061  ).        lyp_pa
+0000bce0: 7468 203d 2067 6473 7061 7468 2e77 6974  th = gdspath.wit
+0000bcf0: 685f 7375 6666 6978 2822 2e6c 7970 2229  h_suffix(".lyp")
+0000bd00: 0a0a 2020 2020 2020 2020 6c61 7965 725f  ..        layer_
+0000bd10: 7669 6577 7320 3d20 6765 745f 6c61 7965  views = get_laye
+0000bd20: 725f 7669 6577 7328 290a 2020 2020 2020  r_views().      
+0000bd30: 2020 6c61 7965 725f 7669 6577 732e 746f    layer_views.to
+0000bd40: 5f6c 7970 2866 696c 6570 6174 683d 6c79  _lyp(filepath=ly
+0000bd50: 705f 7061 7468 290a 0a20 2020 2020 2020  p_path)..       
+0000bd60: 206c 6179 6f75 7420 3d20 4c61 796f 7574   layout = Layout
+0000bd70: 5669 6577 6572 2867 6473 7061 7468 2c20  Viewer(gdspath, 
+0000bd80: 6c79 705f 7061 7468 290a 2020 2020 2020  lyp_path).      
+0000bd90: 2020 6469 7370 6c61 7928 6c61 796f 7574    display(layout
+0000bda0: 2e77 6964 6765 7429 0a0a 2020 2020 6465  .widget)..    de
+0000bdb0: 6620 706c 6f74 5f6b 6c61 796f 7574 280a  f plot_klayout(.
+0000bdc0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000bdd0: 2020 2020 2020 7368 6f77 5f70 6f72 7473        show_ports
+0000bde0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
+0000bdf0: 2020 2020 2020 2070 6f72 745f 6d61 726b         port_mark
+0000be00: 6572 5f6c 6179 6572 3a20 4c61 7965 7220  er_layer: Layer 
+0000be10: 3d20 2831 2c20 3130 292c 0a20 2020 2020  = (1, 10),.     
+0000be20: 2020 2073 686f 775f 6c61 6265 6c73 3a20     show_labels: 
+0000be30: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+0000be40: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+0000be50: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
+0000be60: 6b6c 6179 6f75 7420 696d 6167 652e 0a0a  klayout image...
+0000be70: 2020 2020 2020 2020 4966 2069 7420 6661          If it fa
+0000be80: 696c 7320 746f 2069 6d70 6f72 7420 6b6c  ils to import kl
+0000be90: 6179 6f75 7420 6465 6661 756c 7473 2074  ayout defaults t
+0000bea0: 6f20 6d61 7470 6c6f 746c 6962 2e0a 0a20  o matplotlib... 
+0000beb0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000bec0: 2020 2020 2020 2020 2073 686f 775f 706f           show_po
+0000bed0: 7274 733a 2073 686f 7773 2063 6f6d 706f  rts: shows compo
+0000bee0: 6e65 6e74 2077 6974 6820 706f 7274 206d  nent with port m
+0000bef0: 6172 6b65 7273 2061 6e64 206c 6162 656c  arkers and label
+0000bf00: 732e 0a20 2020 2020 2020 2020 2020 2070  s..            p
+0000bf10: 6f72 745f 6d61 726b 6572 5f6c 6179 6572  ort_marker_layer
+0000bf20: 3a20 666f 7220 7468 6520 706f 7274 732e  : for the ports.
+0000bf30: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
+0000bf40: 775f 6c61 6265 6c73 3a20 7368 6f77 7320  w_labels: shows 
+0000bf50: 6c61 6265 6c73 2e0a 2020 2020 2020 2020  labels..        
+0000bf60: 2222 220a 0a20 2020 2020 2020 2063 6f6d  """..        com
+0000bf70: 706f 6e65 6e74 203d 2028 0a20 2020 2020  ponent = (.     
+0000bf80: 2020 2020 2020 2073 656c 662e 6164 645f         self.add_
+0000bf90: 7069 6e73 5f74 7269 616e 676c 6528 706f  pins_triangle(po
+0000bfa0: 7274 5f6d 6172 6b65 725f 6c61 7965 723d  rt_marker_layer=
+0000bfb0: 706f 7274 5f6d 6172 6b65 725f 6c61 7965  port_marker_laye
+0000bfc0: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
+0000bfd0: 6620 7368 6f77 5f70 6f72 7473 0a20 2020  f show_ports.   
+0000bfe0: 2020 2020 2020 2020 2065 6c73 6520 7365           else se
+0000bff0: 6c66 0a20 2020 2020 2020 2029 0a0a 2020  lf.        )..  
+0000c000: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000c010: 2020 2020 2020 2069 6d70 6f72 7420 6b6c         import kl
+0000c020: 6179 6f75 742e 6462 2061 7320 6462 2020  ayout.db as db  
+0000c030: 2320 6e6f 7161 3a20 4634 3031 0a20 2020  # noqa: F401.   
+0000c040: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
+0000c050: 6b6c 6179 6f75 742e 6c61 7920 6173 206c  klayout.lay as l
+0000c060: 6179 0a20 2020 2020 2020 2020 2020 2066  ay.            f
+0000c070: 726f 6d20 6764 7366 6163 746f 7279 2e70  rom gdsfactory.p
+0000c080: 646b 2069 6d70 6f72 7420 6765 745f 6c61  dk import get_la
+0000c090: 7965 725f 7669 6577 730a 2020 2020 2020  yer_views.      
+0000c0a0: 2020 2020 2020 6672 6f6d 2049 5079 7468        from IPyth
+0000c0b0: 6f6e 2e64 6973 706c 6179 2069 6d70 6f72  on.display impor
+0000c0c0: 7420 6469 7370 6c61 790a 2020 2020 2020  t display.      
+0000c0d0: 2020 2020 2020 6672 6f6d 2069 7079 7769        from ipywi
+0000c0e0: 6467 6574 7320 696d 706f 7274 2049 6d61  dgets import Ima
+0000c0f0: 6765 0a0a 2020 2020 2020 2020 2020 2020  ge..            
+0000c100: 6764 7370 6174 6820 3d20 636f 6d70 6f6e  gdspath = compon
+0000c110: 656e 742e 7772 6974 655f 6764 7328 6c6f  ent.write_gds(lo
+0000c120: 6767 696e 673d 4661 6c73 6529 0a20 2020  gging=False).   
+0000c130: 2020 2020 2020 2020 206c 7970 5f70 6174           lyp_pat
+0000c140: 6820 3d20 6764 7370 6174 682e 7769 7468  h = gdspath.with
+0000c150: 5f73 7566 6669 7828 222e 6c79 7022 290a  _suffix(".lyp").
+0000c160: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+0000c170: 6572 5f76 6965 7773 203d 2067 6574 5f6c  er_views = get_l
+0000c180: 6179 6572 5f76 6965 7773 2829 0a20 2020  ayer_views().   
+0000c190: 2020 2020 2020 2020 206c 6179 6572 5f76           layer_v
+0000c1a0: 6965 7773 2e74 6f5f 6c79 7028 6669 6c65  iews.to_lyp(file
+0000c1b0: 7061 7468 3d6c 7970 5f70 6174 6829 0a0a  path=lyp_path)..
+0000c1c0: 2020 2020 2020 2020 2020 2020 6c61 796f              layo
+0000c1d0: 7574 5f76 6965 7720 3d20 6c61 792e 4c61  ut_view = lay.La
+0000c1e0: 796f 7574 5669 6577 2829 0a20 2020 2020  youtView().     
+0000c1f0: 2020 2020 2020 206c 6179 6f75 745f 7669         layout_vi
+0000c200: 6577 2e6c 6f61 645f 6c61 796f 7574 2873  ew.load_layout(s
+0000c210: 7472 2867 6473 7061 7468 2e61 6273 6f6c  tr(gdspath.absol
+0000c220: 7574 6528 2929 290a 2020 2020 2020 2020  ute())).        
+0000c230: 2020 2020 6c61 796f 7574 5f76 6965 772e      layout_view.
+0000c240: 6d61 785f 6869 6572 2829 0a20 2020 2020  max_hier().     
+0000c250: 2020 2020 2020 206c 6179 6f75 745f 7669         layout_vi
+0000c260: 6577 2e6c 6f61 645f 6c61 7965 725f 7072  ew.load_layer_pr
+0000c270: 6f70 7328 7374 7228 6c79 705f 7061 7468  ops(str(lyp_path
+0000c280: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+0000c290: 6c61 796f 7574 5f76 6965 772e 7365 745f  layout_view.set_
+0000c2a0: 636f 6e66 6967 2822 7465 7874 2d76 6973  config("text-vis
+0000c2b0: 6962 6c65 222c 2022 7472 7565 2220 6966  ible", "true" if
+0000c2c0: 2073 686f 775f 6c61 6265 6c73 2065 6c73   show_labels els
+0000c2d0: 6520 2266 616c 7365 2229 0a0a 2020 2020  e "false")..    
+0000c2e0: 2020 2020 2020 2020 7069 7865 6c5f 6275          pixel_bu
+0000c2f0: 6666 6572 203d 206c 6179 6f75 745f 7669  ffer = layout_vi
+0000c300: 6577 2e67 6574 5f70 6978 656c 735f 7769  ew.get_pixels_wi
+0000c310: 7468 5f6f 7074 696f 6e73 2838 3030 2c20  th_options(800, 
+0000c320: 3630 3029 0a20 2020 2020 2020 2020 2020  600).           
+0000c330: 2070 6e67 5f64 6174 6120 3d20 7069 7865   png_data = pixe
+0000c340: 6c5f 6275 6666 6572 2e74 6f5f 706e 675f  l_buffer.to_png_
+0000c350: 6461 7461 2829 0a20 2020 2020 2020 2020  data().         
+0000c360: 2020 2069 6d61 6765 203d 2049 6d61 6765     image = Image
+0000c370: 2876 616c 7565 3d70 6e67 5f64 6174 612c  (value=png_data,
+0000c380: 2066 6f72 6d61 743d 2270 6e67 2229 0a20   format="png"). 
+0000c390: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+0000c3a0: 6179 2869 6d61 6765 290a 0a20 2020 2020  ay(image)..     
+0000c3b0: 2020 2065 7863 6570 7420 496d 706f 7274     except Import
+0000c3c0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+0000c3d0: 2020 2070 7269 6e74 280a 2020 2020 2020     print(.      
+0000c3e0: 2020 2020 2020 2020 2020 2259 6f75 2063            "You c
+0000c3f0: 616e 2069 6e73 7461 6c6c 2060 7069 7020  an install `pip 
+0000c400: 696e 7374 616c 6c20 6764 7366 6163 746f  install gdsfacto
+0000c410: 7279 5b66 756c 6c5d 6020 666f 7220 6265  ry[full]` for be
+0000c420: 7474 6572 2076 6973 7561 6c69 7a61 7469  tter visualizati
+0000c430: 6f6e 220a 2020 2020 2020 2020 2020 2020  on".            
+0000c440: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+0000c450: 6d70 6f6e 656e 742e 706c 6f74 2870 6c6f  mponent.plot(plo
+0000c460: 7474 6572 3d22 6d61 7470 6c6f 746c 6962  tter="matplotlib
+0000c470: 2229 0a0a 2020 2020 6465 6620 706c 6f74  ")..    def plot
+0000c480: 5f6a 7570 7974 6572 2873 656c 6629 3a0a  _jupyter(self):.
+0000c490: 2020 2020 2020 2020 2222 2253 686f 7773          """Shows
+0000c4a0: 2063 7572 7265 6e74 2067 6473 2069 6e20   current gds in 
+0000c4b0: 6b6c 6179 6f75 742e 2055 7365 7320 4b77  klayout. Uses Kw
+0000c4c0: 6562 2069 6620 7365 7276 6572 2072 756e  eb if server run
+0000c4d0: 6e69 6e67 2e0a 0a20 2020 2020 2020 2069  ning...        i
+0000c4e0: 6620 6e6f 7420 7472 6965 7320 7573 696e  f not tries usin
+0000c4f0: 6720 4b6c 6179 6f75 7420 7769 6467 6574  g Klayout widget
+0000c500: 2061 6e64 2066 696e 616c 6c79 2064 6566   and finally def
+0000c510: 6175 6c74 7320 746f 206d 6174 706c 6f74  aults to matplot
+0000c520: 6c69 622e 0a20 2020 2020 2020 2022 2222  lib..        """
+0000c530: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+0000c540: 2020 2020 2020 2020 2020 696d 706f 7274            import
+0000c550: 206f 730a 2020 2020 2020 2020 2020 2020   os.            
+0000c560: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
+0000c570: 636f 6e66 6967 2069 6d70 6f72 7420 5041  config import PA
+0000c580: 5448 0a20 2020 2020 2020 2020 2020 2066  TH.            f
+0000c590: 726f 6d20 6764 7366 6163 746f 7279 2e70  rom gdsfactory.p
+0000c5a0: 646b 2069 6d70 6f72 7420 6765 745f 6c61  dk import get_la
+0000c5b0: 7965 725f 7669 6577 730a 2020 2020 2020  yer_views.      
+0000c5c0: 2020 2020 2020 6672 6f6d 2049 5079 7468        from IPyth
+0000c5d0: 6f6e 2e64 6973 706c 6179 2069 6d70 6f72  on.display impor
+0000c5e0: 7420 4946 7261 6d65 0a20 2020 2020 2020  t IFrame.       
+0000c5f0: 2020 2020 2069 6d70 6f72 7420 6b77 6562       import kweb
+0000c600: 2e73 6572 7665 725f 6a75 7079 7465 7220  .server_jupyter 
+0000c610: 6173 206b 6a0a 2020 2020 2020 2020 2020  as kj.          
+0000c620: 2020 6672 6f6d 2068 746d 6c20 696d 706f    from html impo
+0000c630: 7274 2065 7363 6170 650a 0a20 2020 2020  rt escape..     
+0000c640: 2020 2020 2020 2067 6473 7061 7468 203d         gdspath =
+0000c650: 2073 656c 662e 7772 6974 655f 6764 7328   self.write_gds(
+0000c660: 6764 7364 6972 3d50 4154 482e 6764 736c  gdsdir=PATH.gdsl
+0000c670: 6962 202f 2022 6578 7472 6122 2c20 6c6f  ib / "extra", lo
+0000c680: 6767 696e 673d 4661 6c73 6529 0a0a 2020  gging=False)..  
+0000c690: 2020 2020 2020 2020 2020 6469 7270 6174            dirpat
+0000c6a0: 6820 3d20 4744 5344 4952 5f54 454d 500a  h = GDSDIR_TEMP.
+0000c6b0: 2020 2020 2020 2020 2020 2020 6469 7270              dirp
+0000c6c0: 6174 682e 6d6b 6469 7228 6578 6973 745f  ath.mkdir(exist_
+0000c6d0: 6f6b 3d54 7275 652c 2070 6172 656e 7473  ok=True, parents
+0000c6e0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+0000c6f0: 2020 206c 7970 5f70 6174 6820 3d20 6469     lyp_path = di
+0000c700: 7270 6174 6820 2f20 226c 6179 6572 732e  rpath / "layers.
+0000c710: 6c79 7022 0a0a 2020 2020 2020 2020 2020  lyp"..          
+0000c720: 2020 6c61 7965 725f 7072 6f70 7320 3d20    layer_props = 
+0000c730: 6765 745f 6c61 7965 725f 7669 6577 7328  get_layer_views(
+0000c740: 290a 2020 2020 2020 2020 2020 2020 6c61  ).            la
+0000c750: 7965 725f 7072 6f70 732e 746f 5f6c 7970  yer_props.to_lyp
+0000c760: 2866 696c 6570 6174 683d 6c79 705f 7061  (filepath=lyp_pa
+0000c770: 7468 290a 0a20 2020 2020 2020 2020 2020  th)..           
+0000c780: 2073 7263 203d 2066 2268 7474 703a 2f2f   src = f"http://
+0000c790: 3132 372e 302e 302e 313a 7b6b 6a2e 706f  127.0.0.1:{kj.po
+0000c7a0: 7274 7d2f 6764 733f 6764 735f 6669 6c65  rt}/gds?gds_file
+0000c7b0: 3d7b 6573 6361 7065 2873 7472 2867 6473  ={escape(str(gds
+0000c7c0: 7061 7468 2929 7d26 6c61 7965 725f 7072  path))}&layer_pr
+0000c7d0: 6f70 733d 7b65 7363 6170 6528 7374 7228  ops={escape(str(
+0000c7e0: 6c79 705f 7061 7468 2929 7d22 0a20 2020  lyp_path))}".   
+0000c7f0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000c800: 6465 6275 6728 7372 6329 0a0a 2020 2020  debug(src)..    
+0000c810: 2020 2020 2020 2020 6966 206b 6a2e 6a75          if kj.ju
+0000c820: 7079 7465 725f 7365 7276 6572 2061 6e64  pyter_server and
+0000c830: 206e 6f74 206f 732e 656e 7669 726f 6e2e   not os.environ.
+0000c840: 6765 7428 2244 4f43 5322 2c20 4661 6c73  get("DOCS", Fals
+0000c850: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+0000c860: 2020 2020 7265 7475 726e 2049 4672 616d      return IFram
+0000c870: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+0000c880: 2020 2020 2020 2073 7263 3d73 7263 2c0a         src=src,.
+0000c890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8a0: 2020 2020 7769 6474 683d 3134 3030 2c0a      width=1400,.
+0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8c0: 2020 2020 6865 6967 6874 3d36 3030 2c0a      height=600,.
+0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8e0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000c8f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000c900: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000c910: 706c 6f74 5f6b 6c61 796f 7574 2829 0a20  plot_klayout(). 
+0000c920: 2020 2020 2020 2065 7863 6570 7420 496d         except Im
+0000c930: 706f 7274 4572 726f 723a 0a20 2020 2020  portError:.     
+0000c940: 2020 2020 2020 2070 7269 6e74 280a 2020         print(.  
+0000c950: 2020 2020 2020 2020 2020 2020 2020 2259                "Y
+0000c960: 6f75 2063 616e 2069 6e73 7461 6c6c 2060  ou can install `
+0000c970: 7069 7020 696e 7374 616c 6c20 6764 7366  pip install gdsf
+0000c980: 6163 746f 7279 5b66 756c 6c5d 6020 666f  actory[full]` fo
+0000c990: 7220 6265 7474 6572 2076 6973 7561 6c69  r better visuali
+0000c9a0: 7a61 7469 6f6e 220a 2020 2020 2020 2020  zation".        
+0000c9b0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000c9c0: 2020 7265 7475 726e 2073 656c 662e 706c    return self.pl
+0000c9d0: 6f74 5f6b 6c61 796f 7574 2829 0a0a 2020  ot_klayout()..  
+0000c9e0: 2020 6465 6620 706c 6f74 5f6d 6174 706c    def plot_matpl
+0000c9f0: 6f74 6c69 6228 7365 6c66 2c20 2a2a 6b77  otlib(self, **kw
+0000ca00: 6172 6773 2920 2d3e 204e 6f6e 653a 0a20  args) -> None:. 
+0000ca10: 2020 2020 2020 2022 2222 506c 6f74 2063         """Plot c
+0000ca20: 6f6d 706f 6e65 6e74 2075 7369 6e67 206d  omponent using m
+0000ca30: 6174 706c 6f74 6c69 622e 0a0a 2020 2020  atplotlib...    
+0000ca40: 2020 2020 4b65 7977 6f72 6420 4172 6773      Keyword Args
+0000ca50: 3a0a 2020 2020 2020 2020 2020 2020 7368  :.            sh
+0000ca60: 6f77 5f70 6f72 7473 3a20 5365 7473 2077  ow_ports: Sets w
+0000ca70: 6865 7468 6572 2070 6f72 7473 2061 7265  hether ports are
+0000ca80: 2064 7261 776e 2e0a 2020 2020 2020 2020   drawn..        
+0000ca90: 2020 2020 7368 6f77 5f73 7562 706f 7274      show_subport
+0000caa0: 733a 2053 6574 7320 7768 6574 6865 7220  s: Sets whether 
+0000cab0: 7375 6270 6f72 7473 2028 706f 7274 7320  subports (ports 
+0000cac0: 7468 6174 2062 656c 6f6e 6720 746f 2072  that belong to r
+0000cad0: 6566 6572 656e 6365 7329 2061 7265 2064  eferences) are d
+0000cae0: 7261 776e 2e0a 2020 2020 2020 2020 2020  rawn..          
+0000caf0: 2020 6c61 6265 6c5f 616c 6961 7365 733a    label_aliases:
+0000cb00: 2053 6574 7320 7768 6574 6865 7220 616c   Sets whether al
+0000cb10: 6961 7365 7320 6172 6520 6c61 6265 6c65  iases are labele
+0000cb20: 6420 7769 7468 2061 2074 6578 7420 6e61  d with a text na
+0000cb30: 6d65 2e0a 2020 2020 2020 2020 2020 2020  me..            
+0000cb40: 6e65 775f 7769 6e64 6f77 3a20 4966 2054  new_window: If T
+0000cb50: 7275 652c 2065 6163 6820 6361 6c6c 2074  rue, each call t
+0000cb60: 6f20 7175 6963 6b70 6c6f 7428 2920 7769  o quickplot() wi
+0000cb70: 6c6c 2067 656e 6572 6174 6520 6120 7365  ll generate a se
+0000cb80: 7061 7261 7465 2077 696e 646f 772e 0a20  parate window.. 
+0000cb90: 2020 2020 2020 2020 2020 2062 6c6f 636b             block
+0000cba0: 696e 673a 2049 6620 5472 7565 2c20 6361  ing: If True, ca
+0000cbb0: 6c6c 696e 6720 7175 6963 6b70 6c6f 7428  lling quickplot(
+0000cbc0: 2920 7769 6c6c 2070 6175 7365 2065 7865  ) will pause exe
+0000cbd0: 6375 7469 6f6e 206f 6620 2822 626c 6f63  cution of ("bloc
+0000cbe0: 6b22 2920 7468 650a 2020 2020 2020 2020  k") the.        
+0000cbf0: 2020 2020 2020 2020 7265 6d61 696e 6465          remainde
+0000cc00: 7220 6f66 2074 6865 2070 7974 686f 6e20  r of the python 
+0000cc10: 636f 6465 2075 6e74 696c 2074 6865 2071  code until the q
+0000cc20: 7569 636b 706c 6f74 2829 2077 696e 646f  uickplot() windo
+0000cc30: 7720 6973 2063 6c6f 7365 642e 0a20 2020  w is closed..   
+0000cc40: 2020 2020 2020 2020 2020 2020 2049 6620               If 
+0000cc50: 4661 6c73 652c 2074 6865 2077 696e 646f  False, the windo
+0000cc60: 7720 7769 6c6c 2062 6520 6f70 656e 6564  w will be opened
+0000cc70: 2061 6e64 2063 6f64 6520 7769 6c6c 2063   and code will c
+0000cc80: 6f6e 7469 6e75 6520 746f 2072 756e 2e0a  ontinue to run..
+0000cc90: 2020 2020 2020 2020 2020 2020 7a6f 6f6d              zoom
+0000cca0: 5f66 6163 746f 723a 2053 6574 7320 7468  _factor: Sets th
+0000ccb0: 6520 7363 616c 696e 6720 6661 6374 6f72  e scaling factor
+0000ccc0: 2077 6865 6e20 7a6f 6f6d 696e 6720 7468   when zooming th
+0000ccd0: 6520 7175 6963 6b70 6c6f 7420 7769 6e64  e quickplot wind
+0000cce0: 6f77 2077 6974 6820 7468 650a 2020 2020  ow with the.    
+0000ccf0: 2020 2020 2020 2020 2020 2020 6d6f 7573              mous
+0000cd00: 6577 6865 656c 2f74 7261 636b 7061 642e  ewheel/trackpad.
+0000cd10: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
+0000cd20: 6572 6163 7469 7665 5f7a 6f6f 6d3a 2045  eractive_zoom: E
+0000cd30: 6e61 626c 6573 2075 7369 6e67 206d 6f75  nables using mou
+0000cd40: 7365 7768 6565 6c2f 7472 6163 6b70 6164  sewheel/trackpad
+0000cd50: 2074 6f20 7a6f 6f6d 2e0a 2020 2020 2020   to zoom..      
+0000cd60: 2020 2020 2020 666f 6e74 7369 7a65 3a20        fontsize: 
+0000cd70: 666f 7220 6c61 6265 6c73 2e0a 2020 2020  for labels..    
+0000cd80: 2020 2020 2020 2020 6c61 7965 7273 5f65          layers_e
+0000cd90: 7863 6c75 6465 643a 206c 6973 7420 6f66  xcluded: list of
+0000cda0: 206c 6179 6572 7320 746f 2065 7863 6c75   layers to exclu
+0000cdb0: 6465 2e0a 2020 2020 2020 2020 2020 2020  de..            
+0000cdc0: 6c61 7965 725f 7669 6577 733a 206c 6179  layer_views: lay
+0000cdd0: 6572 5f76 6965 7773 2063 6f6c 6f72 7320  er_views colors 
+0000cde0: 6c6f 6164 6564 2066 726f 6d20 4b6c 6179  loaded from Klay
+0000cdf0: 6f75 742e 0a20 2020 2020 2020 2020 2020  out..           
+0000ce00: 206d 696e 5f61 7370 6563 743a 206d 696e   min_aspect: min
+0000ce10: 696d 756d 2061 7370 6563 7420 7261 7469  imum aspect rati
+0000ce20: 6f2e 0a20 2020 2020 2020 2022 2222 0a20  o..        """. 
+0000ce30: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
+0000ce40: 6163 746f 7279 2e71 7569 636b 706c 6f74  actory.quickplot
+0000ce50: 7465 7220 696d 706f 7274 2071 7569 636b  ter import quick
+0000ce60: 706c 6f74 0a0a 2020 2020 2020 2020 7175  plot..        qu
+0000ce70: 6963 6b70 6c6f 7428 7365 6c66 2c20 2a2a  ickplot(self, **
+0000ce80: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
+0000ce90: 2070 6c6f 7428 7365 6c66 2c20 706c 6f74   plot(self, plot
+0000cea0: 7465 723a 204f 7074 696f 6e61 6c5b 506c  ter: Optional[Pl
+0000ceb0: 6f74 7465 725d 203d 204e 6f6e 652c 202a  otter] = None, *
+0000cec0: 2a6b 7761 7267 7329 202d 3e20 4e6f 6e65  *kwargs) -> None
+0000ced0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+0000cee0: 7572 6e73 2063 6f6d 706f 6e65 6e74 2070  urns component p
+0000cef0: 6c6f 7420 7573 696e 6720 6b6c 6179 6f75  lot using klayou
+0000cf00: 742c 206d 6174 706c 6f74 6c69 622c 2068  t, matplotlib, h
+0000cf10: 6f6c 6f76 6965 7773 206f 7220 7174 2e0a  oloviews or qt..
+0000cf20: 0a20 2020 2020 2020 2057 6520 7265 636f  .        We reco
+0000cf30: 6d6d 656e 6420 7573 696e 6720 6b6c 6179  mmend using klay
+0000cf40: 6f75 742e 0a0a 2020 2020 2020 2020 4172  out...        Ar
+0000cf50: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000cf60: 706c 6f74 7465 723a 2070 6c6f 7420 6261  plotter: plot ba
+0000cf70: 636b 656e 6420 2827 686f 6c6f 7669 6577  ckend ('holoview
+0000cf80: 7327 2c20 276d 6174 706c 6f74 6c69 6227  s', 'matplotlib'
+0000cf90: 2c20 2771 7427 2c20 276b 6c61 796f 7574  , 'qt', 'klayout
+0000cfa0: 2729 2e0a 2020 2020 2020 2020 2222 220a  ')..        """.
+0000cfb0: 2020 2020 2020 2020 706c 6f74 7465 7220          plotter 
+0000cfc0: 3d20 706c 6f74 7465 7220 6f72 2043 4f4e  = plotter or CON
+0000cfd0: 462e 6765 7428 2270 6c6f 7474 6572 222c  F.get("plotter",
+0000cfe0: 2022 6d61 7470 6c6f 746c 6962 2229 0a0a   "matplotlib")..
+0000cff0: 2020 2020 2020 2020 6966 2070 6c6f 7474          if plott
+0000d000: 6572 203d 3d20 226b 6c61 796f 7574 223a  er == "klayout":
+0000d010: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d020: 662e 706c 6f74 5f6b 6c61 796f 7574 2829  f.plot_klayout()
+0000d030: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000d040: 7572 6e0a 0a20 2020 2020 2020 2065 6c69  urn..        eli
+0000d050: 6620 706c 6f74 7465 7220 3d3d 2022 6d61  f plotter == "ma
+0000d060: 7470 6c6f 746c 6962 223a 0a20 2020 2020  tplotlib":.     
+0000d070: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
+0000d080: 6163 746f 7279 2e71 7569 636b 706c 6f74  actory.quickplot
+0000d090: 7465 7220 696d 706f 7274 2071 7569 636b  ter import quick
+0000d0a0: 706c 6f74 0a0a 2020 2020 2020 2020 2020  plot..          
+0000d0b0: 2020 7175 6963 6b70 6c6f 7428 7365 6c66    quickplot(self
+0000d0c0: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+0000d0d0: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+0000d0e0: 2020 2020 2020 2020 656c 6966 2070 6c6f          elif plo
+0000d0f0: 7474 6572 203d 3d20 2268 6f6c 6f76 6965  tter == "holovie
+0000d100: 7773 223a 0a20 2020 2020 2020 2020 2020  ws":.           
+0000d110: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000d120: 2020 2020 2020 696d 706f 7274 2068 6f6c        import hol
+0000d130: 6f76 6965 7773 2061 7320 6876 0a0a 2020  oviews as hv..  
+0000d140: 2020 2020 2020 2020 2020 2020 2020 6876                hv
+0000d150: 2e65 7874 656e 7369 6f6e 2822 626f 6b65  .extension("boke
+0000d160: 6822 290a 2020 2020 2020 2020 2020 2020  h").            
+0000d170: 6578 6365 7074 2049 6d70 6f72 7445 7272  except ImportErr
+0000d180: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
+0000d190: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+0000d1a0: 796f 7520 6e65 6564 2074 6f20 6070 6970  you need to `pip
+0000d1b0: 2069 6e73 7461 6c6c 2068 6f6c 6f76 6965   install holovie
+0000d1c0: 7773 6022 290a 2020 2020 2020 2020 2020  ws`").          
+0000d1d0: 2020 2020 2020 7261 6973 6520 650a 2020        raise e.  
+0000d1e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000d1f0: 2073 656c 662e 706c 6f74 5f68 6f6c 6f76   self.plot_holov
+0000d200: 6965 7773 282a 2a6b 7761 7267 7329 0a0a  iews(**kwargs)..
+0000d210: 2020 2020 2020 2020 656c 6966 2070 6c6f          elif plo
+0000d220: 7474 6572 203d 3d20 2271 7422 3a0a 2020  tter == "qt":.  
+0000d230: 2020 2020 2020 2020 2020 6672 6f6d 2067            from g
+0000d240: 6473 6661 6374 6f72 792e 7175 6963 6b70  dsfactory.quickp
+0000d250: 6c6f 7474 6572 2069 6d70 6f72 7420 7175  lotter import qu
+0000d260: 6963 6b70 6c6f 7432 0a0a 2020 2020 2020  ickplot2..      
+0000d270: 2020 2020 2020 7175 6963 6b70 6c6f 7432        quickplot2
+0000d280: 2873 656c 6629 0a20 2020 2020 2020 2020  (self).         
+0000d290: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000d2a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000d2b0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000d2c0: 7272 6f72 2866 227b 706c 6f74 7465 7221  rror(f"{plotter!
+0000d2d0: 727d 206e 6f74 2069 6e20 7b50 6c6f 7474  r} not in {Plott
+0000d2e0: 6572 7d22 290a 0a20 2020 2064 6566 2070  er}")..    def p
+0000d2f0: 6c6f 745f 686f 6c6f 7669 6577 7328 0a20  lot_holoviews(. 
+0000d300: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000d310: 2020 2020 206c 6179 6572 735f 6578 636c       layers_excl
+0000d320: 7564 6564 3a20 4f70 7469 6f6e 616c 5b4c  uded: Optional[L
+0000d330: 6179 6572 735d 203d 204e 6f6e 652c 0a20  ayers] = None,. 
+0000d340: 2020 2020 2020 206c 6179 6572 5f76 6965         layer_vie
+0000d350: 7773 3a20 4f70 7469 6f6e 616c 5b4c 6179  ws: Optional[Lay
+0000d360: 6572 5669 6577 735d 203d 204e 6f6e 652c  erViews] = None,
+0000d370: 0a20 2020 2020 2020 206d 696e 5f61 7370  .        min_asp
+0000d380: 6563 743a 2066 6c6f 6174 203d 2030 2e32  ect: float = 0.2
+0000d390: 352c 0a20 2020 2020 2020 2070 6164 6469  5,.        paddi
+0000d3a0: 6e67 3a20 666c 6f61 7420 3d20 302e 352c  ng: float = 0.5,
+0000d3b0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0000d3c0: 2222 2250 6c6f 7420 636f 6d70 6f6e 656e  """Plot componen
+0000d3d0: 7420 696e 2068 6f6c 6f76 6965 7773 2e0a  t in holoviews..
+0000d3e0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000d3f0: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+0000d400: 735f 6578 636c 7564 6564 3a20 6c69 7374  s_excluded: list
+0000d410: 206f 6620 6c61 7965 7273 2074 6f20 6578   of layers to ex
+0000d420: 636c 7564 652e 0a20 2020 2020 2020 2020  clude..         
+0000d430: 2020 206c 6179 6572 5f76 6965 7773 3a20     layer_views: 
+0000d440: 6c61 7965 725f 7669 6577 7320 636f 6c6f  layer_views colo
+0000d450: 7273 206c 6f61 6465 6420 6672 6f6d 204b  rs loaded from K
+0000d460: 6c61 796f 7574 2e0a 2020 2020 2020 2020  layout..        
+0000d470: 2020 2020 6d69 6e5f 6173 7065 6374 3a20      min_aspect: 
+0000d480: 6d69 6e69 6d75 6d20 6173 7065 6374 2072  minimum aspect r
+0000d490: 6174 696f 2e0a 2020 2020 2020 2020 2020  atio..          
+0000d4a0: 2020 7061 6464 696e 673a 2061 726f 756e    padding: aroun
+0000d4b0: 6420 626f 756e 6469 6e67 2062 6f78 2e0a  d bounding box..
+0000d4c0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000d4d0: 3a0a 2020 2020 2020 2020 2020 2020 486f  :.            Ho
+0000d4e0: 6c6f 7669 6577 7320 4f76 6572 6c61 7920  loviews Overlay 
+0000d4f0: 746f 2064 6973 706c 6179 2061 6c6c 2070  to display all p
+0000d500: 6f6c 7967 6f6e 732e 0a20 2020 2020 2020  olygons..       
+0000d510: 2022 2222 0a20 2020 2020 2020 2066 726f   """.        fro
+0000d520: 6d20 6764 7366 6163 746f 7279 2e61 6464  m gdsfactory.add
+0000d530: 5f70 696e 7320 696d 706f 7274 2067 6574  _pins import get
+0000d540: 5f70 696e 5f74 7269 616e 676c 655f 706f  _pin_triangle_po
+0000d550: 6c79 676f 6e5f 7469 700a 2020 2020 2020  lygon_tip.      
+0000d560: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
+0000d570: 792e 6765 6e65 7269 635f 7465 6368 2069  y.generic_tech i
+0000d580: 6d70 6f72 7420 4c41 5945 525f 5649 4557  mport LAYER_VIEW
+0000d590: 530a 0a20 2020 2020 2020 2069 6620 6c61  S..        if la
+0000d5a0: 7965 725f 7669 6577 7320 6973 204e 6f6e  yer_views is Non
+0000d5b0: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
+0000d5c0: 6179 6572 5f76 6965 7773 203d 204c 4159  ayer_views = LAY
+0000d5d0: 4552 5f56 4945 5753 0a0a 2020 2020 2020  ER_VIEWS..      
+0000d5e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000d5f0: 2020 2069 6d70 6f72 7420 686f 6c6f 7669     import holovi
+0000d600: 6577 7320 6173 2068 760a 0a20 2020 2020  ews as hv..     
+0000d610: 2020 2020 2020 2068 762e 6578 7465 6e73         hv.extens
+0000d620: 696f 6e28 2262 6f6b 6568 2229 0a20 2020  ion("bokeh").   
+0000d630: 2020 2020 2065 7863 6570 7420 496d 706f       except Impo
+0000d640: 7274 4572 726f 7220 6173 2065 3a0a 2020  rtError as e:.  
+0000d650: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000d660: 2279 6f75 206e 6565 6420 746f 2060 7069  "you need to `pi
+0000d670: 7020 696e 7374 616c 6c20 686f 6c6f 7669  p install holovi
+0000d680: 6577 7360 2229 0a20 2020 2020 2020 2020  ews`").         
+0000d690: 2020 2072 6169 7365 2065 0a0a 2020 2020     raise e..    
+0000d6a0: 2020 2020 7365 6c66 2e5f 6262 5f76 616c      self._bb_val
+0000d6b0: 6964 203d 2046 616c 7365 2020 2320 7265  id = False  # re
+0000d6c0: 636f 6d70 7574 6520 7468 6520 626f 756e  compute the boun
+0000d6d0: 6469 6e67 2062 6f78 0a20 2020 2020 2020  ding box.       
+0000d6e0: 2062 203d 2073 656c 662e 6262 6f78 202b   b = self.bbox +
+0000d6f0: 2028 282d 7061 6464 696e 672c 202d 7061   ((-padding, -pa
+0000d700: 6464 696e 6729 2c20 2870 6164 6469 6e67  dding), (padding
+0000d710: 2c20 7061 6464 696e 6729 290a 2020 2020  , padding)).    
+0000d720: 2020 2020 6220 3d20 6e70 2e61 7272 6179      b = np.array
+0000d730: 2862 2e66 6c61 7429 0a20 2020 2020 2020  (b.flat).       
+0000d740: 2063 656e 7465 7220 3d20 6e70 2e61 7272   center = np.arr
+0000d750: 6179 2828 6e70 2e73 756d 2862 5b3a 3a32  ay((np.sum(b[::2
+0000d760: 5d29 202f 2032 2c20 6e70 2e73 756d 2862  ]) / 2, np.sum(b
+0000d770: 5b31 3a3a 325d 2920 2f20 3229 290a 2020  [1::2]) / 2)).  
+0000d780: 2020 2020 2020 7369 7a65 203d 206e 702e        size = np.
+0000d790: 6172 7261 7928 286e 702e 6162 7328 625b  array((np.abs(b[
+0000d7a0: 325d 202d 2062 5b30 5d29 2c20 6e70 2e61  2] - b[0]), np.a
+0000d7b0: 6273 2862 5b33 5d20 2d20 625b 315d 2929  bs(b[3] - b[1]))
+0000d7c0: 290a 2020 2020 2020 2020 6478 203d 206e  ).        dx = n
+0000d7d0: 702e 6172 7261 7928 0a20 2020 2020 2020  p.array(.       
+0000d7e0: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
+0000d7f0: 2020 2020 2020 206e 702e 6d61 7869 6d75         np.maximu
+0000d800: 6d28 6d69 6e5f 6173 7065 6374 202a 2073  m(min_aspect * s
+0000d810: 697a 655b 315d 2c20 7369 7a65 5b30 5d29  ize[1], size[0])
+0000d820: 202f 2032 2c0a 2020 2020 2020 2020 2020   / 2,.          
+0000d830: 2020 2020 2020 6e70 2e6d 6178 696d 756d        np.maximum
+0000d840: 2873 697a 655b 315d 2c20 6d69 6e5f 6173  (size[1], min_as
+0000d850: 7065 6374 202a 2073 697a 655b 305d 2920  pect * size[0]) 
+0000d860: 2f20 322c 0a20 2020 2020 2020 2020 2020  / 2,.           
+0000d870: 2029 0a20 2020 2020 2020 2029 0a20 2020   ).        ).   
+0000d880: 2020 2020 2062 203d 206e 702e 6873 7461       b = np.hsta
+0000d890: 636b 2828 6365 6e74 6572 202d 2064 782c  ck((center - dx,
+0000d8a0: 2063 656e 7465 7220 2b20 6478 2929 0a0a   center + dx))..
+0000d8b0: 2020 2020 2020 2020 706c 6f74 735f 746f          plots_to
+0000d8c0: 5f6f 7665 726c 6179 203d 205b 5d0a 2020  _overlay = [].  
+0000d8d0: 2020 2020 2020 6c61 7965 7273 5f65 7863        layers_exc
+0000d8e0: 6c75 6465 6420 3d20 5b5d 2069 6620 6c61  luded = [] if la
+0000d8f0: 7965 7273 5f65 7863 6c75 6465 6420 6973  yers_excluded is
+0000d900: 204e 6f6e 6520 656c 7365 206c 6179 6572   None else layer
+0000d910: 735f 6578 636c 7564 6564 0a0a 2020 2020  s_excluded..    
+0000d920: 2020 2020 666f 7220 6c61 7965 722c 2070      for layer, p
+0000d930: 6f6c 7967 6f6e 2069 6e20 7365 6c66 2e67  olygon in self.g
+0000d940: 6574 5f70 6f6c 7967 6f6e 7328 6279 5f73  et_polygons(by_s
+0000d950: 7065 633d 5472 7565 292e 6974 656d 7328  pec=True).items(
+0000d960: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0000d970: 6620 6c61 7965 7220 696e 206c 6179 6572  f layer in layer
+0000d980: 735f 6578 636c 7564 6564 3a0a 2020 2020  s_excluded:.    
+0000d990: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000d9a0: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
+0000d9b0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000d9c0: 2020 2020 2020 206c 6179 6572 5f76 6965         layer_vie
+0000d9d0: 7720 3d20 6c61 7965 725f 7669 6577 732e  w = layer_views.
+0000d9e0: 6765 745f 6672 6f6d 5f74 7570 6c65 286c  get_from_tuple(l
+0000d9f0: 6179 6572 290a 2020 2020 2020 2020 2020  ayer).          
+0000da00: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+0000da10: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+0000da20: 2020 2020 206c 6179 6572 7320 3d20 6c69       layers = li
+0000da30: 7374 286c 6179 6572 5f76 6965 7773 2e67  st(layer_views.g
+0000da40: 6574 5f6c 6179 6572 5f76 6965 7773 2829  et_layer_views()
+0000da50: 2e6b 6579 7328 2929 0a20 2020 2020 2020  .keys()).       
+0000da60: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0000da70: 732e 7761 726e 2866 227b 6c61 7965 7221  s.warn(f"{layer!
+0000da80: 727d 206e 6f74 2064 6566 696e 6564 2069  r} not defined i
+0000da90: 6e20 7b6c 6179 6572 737d 2229 0a20 2020  n {layers}").   
+0000daa0: 2020 2020 2020 2020 2020 2020 206c 6179               lay
+0000dab0: 6572 5f76 6965 7720 3d20 4c61 7965 7256  er_view = LayerV
+0000dac0: 6965 7728 6c61 7965 723d 6c61 7965 7229  iew(layer=layer)
+0000dad0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+0000dae0: 4f44 4f3a 204d 6174 6368 2075 7020 6f70  ODO: Match up op
+0000daf0: 7469 6f6e 7320 7769 7468 204c 6179 6572  tions with Layer
+0000db00: 5669 6577 730a 2020 2020 2020 2020 2020  Views.          
+0000db10: 2020 706c 6f74 735f 746f 5f6f 7665 726c    plots_to_overl
+0000db20: 6179 2e61 7070 656e 6428 0a20 2020 2020  ay.append(.     
+0000db30: 2020 2020 2020 2020 2020 2068 762e 506f             hv.Po
+0000db40: 6c79 676f 6e73 2870 6f6c 7967 6f6e 2c20  lygons(polygon, 
+0000db50: 6c61 6265 6c3d 7374 7228 6c61 7965 725f  label=str(layer_
+0000db60: 7669 6577 2e6e 616d 6529 292e 6f70 7473  view.name)).opts
+0000db70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000db80: 2020 2020 2020 6461 7461 5f61 7370 6563        data_aspec
+0000db90: 743d 312c 0a20 2020 2020 2020 2020 2020  t=1,.           
+0000dba0: 2020 2020 2020 2020 2066 7261 6d65 5f77           frame_w
+0000dbb0: 6964 7468 3d35 3030 2c0a 2020 2020 2020  idth=500,.      
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 796c                yl
+0000dbd0: 696d 3d28 625b 315d 2c20 625b 335d 292c  im=(b[1], b[3]),
+0000dbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dbf0: 2020 2020 2078 6c69 6d3d 2862 5b30 5d2c       xlim=(b[0],
+0000dc00: 2062 5b32 5d29 2c0a 2020 2020 2020 2020   b[2]),.        
+0000dc10: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
+0000dc20: 5f63 6f6c 6f72 3d6c 6179 6572 5f76 6965  _color=layer_vie
+0000dc30: 772e 6669 6c6c 5f63 6f6c 6f72 2e61 735f  w.fill_color.as_
+0000dc40: 7267 6228 2920 6f72 2022 222c 0a20 2020  rgb() or "",.   
+0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc60: 206c 696e 655f 636f 6c6f 723d 6c61 7965   line_color=laye
+0000dc70: 725f 7669 6577 2e66 7261 6d65 5f63 6f6c  r_view.frame_col
+0000dc80: 6f72 2e61 735f 7267 6228 2920 6f72 2022  or.as_rgb() or "
+0000dc90: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000dca0: 2020 2020 2020 2066 696c 6c5f 616c 7068         fill_alph
+0000dcb0: 613d 6c61 7965 725f 7669 6577 2e67 6574  a=layer_view.get
+0000dcc0: 5f61 6c70 6861 2829 206f 7220 2222 2c0a  _alpha() or "",.
+0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dce0: 2020 2020 6c69 6e65 5f61 6c70 6861 3d6c      line_alpha=l
+0000dcf0: 6179 6572 5f76 6965 772e 6765 745f 616c  ayer_view.get_al
+0000dd00: 7068 6128 2920 6f72 2022 222c 0a20 2020  pha() or "",.   
+0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd20: 2074 6f6f 6c73 3d5b 2268 6f76 6572 225d   tools=["hover"]
+0000dd30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000dd40: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000dd50: 290a 2020 2020 2020 2020 666f 7220 6e61  ).        for na
+0000dd60: 6d65 2c20 706f 7274 2069 6e20 7365 6c66  me, port in self
+0000dd70: 2e70 6f72 7473 2e69 7465 6d73 2829 3a0a  .ports.items():.
+0000dd80: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0000dd90: 203d 2073 7472 286e 616d 6529 0a20 2020   = str(name).   
+0000dda0: 2020 2020 2020 2020 2070 6f6c 7967 6f6e           polygon
+0000ddb0: 2c20 7074 6970 203d 2067 6574 5f70 696e  , ptip = get_pin
+0000ddc0: 5f74 7269 616e 676c 655f 706f 6c79 676f  _triangle_polygo
+0000ddd0: 6e5f 7469 7028 706f 7274 3d70 6f72 7429  n_tip(port=port)
+0000dde0: 0a0a 2020 2020 2020 2020 2020 2020 706c  ..            pl
+0000ddf0: 6f74 735f 746f 5f6f 7665 726c 6179 2e61  ots_to_overlay.a
+0000de00: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
+0000de10: 2020 2020 2020 2068 762e 506f 6c79 676f         hv.Polygo
+0000de20: 6e73 2870 6f6c 7967 6f6e 2c20 6c61 6265  ns(polygon, labe
+0000de30: 6c3d 6e61 6d65 292e 6f70 7473 280a 2020  l=name).opts(.  
+0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de50: 2020 6461 7461 5f61 7370 6563 743d 312c    data_aspect=1,
+0000de60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000de70: 2020 2020 2066 7261 6d65 5f77 6964 7468       frame_width
+0000de80: 3d35 3030 2c0a 2020 2020 2020 2020 2020  =500,.          
+0000de90: 2020 2020 2020 2020 2020 6669 6c6c 5f61            fill_a
+0000dea0: 6c70 6861 3d30 2c0a 2020 2020 2020 2020  lpha=0,.        
+0000deb0: 2020 2020 2020 2020 2020 2020 796c 696d              ylim
+0000dec0: 3d28 625b 315d 2c20 625b 335d 292c 0a20  =(b[1], b[3]),. 
+0000ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dee0: 2020 2078 6c69 6d3d 2862 5b30 5d2c 2062     xlim=(b[0], b
+0000def0: 5b32 5d29 2c0a 2020 2020 2020 2020 2020  [2]),.          
+0000df00: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
+0000df10: 2272 6564 222c 0a20 2020 2020 2020 2020  "red",.         
+0000df20: 2020 2020 2020 2020 2020 206c 696e 655f             line_
+0000df30: 616c 7068 613d 6c61 7965 725f 7669 6577  alpha=layer_view
+0000df40: 2e67 6574 5f61 6c70 6861 2829 206f 7220  .get_alpha() or 
+0000df50: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+0000df60: 2020 2020 2020 2020 746f 6f6c 733d 5b22          tools=["
+0000df70: 686f 7665 7222 5d2c 0a20 2020 2020 2020  hover"],.       
+0000df80: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000df90: 2020 2020 2020 2020 2020 202a 2068 762e             * hv.
+0000dfa0: 5465 7874 2870 7469 705b 305d 2c20 7074  Text(ptip[0], pt
+0000dfb0: 6970 5b31 5d2c 206e 616d 6529 0a20 2020  ip[1], name).   
+0000dfc0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000dfd0: 2020 2020 7265 7475 726e 2068 762e 4f76      return hv.Ov
+0000dfe0: 6572 6c61 7928 706c 6f74 735f 746f 5f6f  erlay(plots_to_o
+0000dff0: 7665 726c 6179 292e 6f70 7473 280a 2020  verlay).opts(.  
+0000e000: 2020 2020 2020 2020 2020 7368 6f77 5f6c            show_l
+0000e010: 6567 656e 643d 5472 7565 2c20 7368 6172  egend=True, shar
+0000e020: 6564 5f61 7865 733d 4661 6c73 652c 2079  ed_axes=False, y
+0000e030: 6c69 6d3d 2862 5b31 5d2c 2062 5b33 5d29  lim=(b[1], b[3])
+0000e040: 2c20 786c 696d 3d28 625b 305d 2c20 625b  , xlim=(b[0], b[
+0000e050: 325d 290a 2020 2020 2020 2020 290a 0a20  2]).        ).. 
+0000e060: 2020 2064 6566 2073 686f 7728 0a20 2020     def show(.   
+0000e070: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000e080: 2020 2073 686f 775f 706f 7274 733a 2062     show_ports: b
+0000e090: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+0000e0a0: 2020 2020 2073 686f 775f 7375 6270 6f72       show_subpor
+0000e0b0: 7473 3a20 626f 6f6c 203d 2046 616c 7365  ts: bool = False
+0000e0c0: 2c0a 2020 2020 2020 2020 706f 7274 5f6d  ,.        port_m
+0000e0d0: 6172 6b65 725f 6c61 7965 723a 204c 6179  arker_layer: Lay
+0000e0e0: 6572 203d 2028 312c 2031 3029 2c0a 2020  er = (1, 10),.  
+0000e0f0: 2020 2020 2020 2a2a 6b77 6172 6773 2c0a        **kwargs,.
+0000e100: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
+0000e110: 2020 2020 2020 2022 2222 5368 6f77 2063         """Show c
+0000e120: 6f6d 706f 6e65 6e74 2069 6e20 4b4c 6179  omponent in KLay
+0000e130: 6f75 742e 0a0a 2020 2020 2020 2020 7265  out...        re
+0000e140: 7475 726e 7320 6120 636f 7079 206f 6620  turns a copy of 
+0000e150: 7468 6520 436f 6d70 6f6e 656e 742c 2073  the Component, s
+0000e160: 6f20 7468 6520 6f72 6967 696e 616c 2063  o the original c
+0000e170: 6f6d 706f 6e65 6e74 2072 656d 6169 6e73  omponent remains
+0000e180: 2069 6e74 6163 742e 0a20 2020 2020 2020   intact..       
+0000e190: 2077 6974 6820 7069 6e73 206d 6172 6b65   with pins marke
+0000e1a0: 7273 206f 6e20 6561 6368 2070 6f72 7420  rs on each port 
+0000e1b0: 7368 6f77 5f70 6f72 7473 203d 2054 7275  show_ports = Tru
+0000e1c0: 652c 2061 6e64 206f 7074 696f 6e61 6c6c  e, and optionall
+0000e1d0: 7920 616c 736f 0a20 2020 2020 2020 2074  y also.        t
+0000e1e0: 6865 2070 6f72 7473 2066 726f 6d20 7468  he ports from th
+0000e1f0: 6520 7265 6665 7265 6e63 6573 2028 7368  e references (sh
+0000e200: 6f77 5f73 7562 706f 7274 733d 5472 7565  ow_subports=True
+0000e210: 290a 0a20 2020 2020 2020 2041 7267 733a  )..        Args:
+0000e220: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
+0000e230: 775f 706f 7274 733a 2073 686f 7773 2063  w_ports: shows c
+0000e240: 6f6d 706f 6e65 6e74 2077 6974 6820 706f  omponent with po
+0000e250: 7274 206d 6172 6b65 7273 2061 6e64 206c  rt markers and l
+0000e260: 6162 656c 732e 0a20 2020 2020 2020 2020  abels..         
+0000e270: 2020 2073 686f 775f 7375 6270 6f72 7473     show_subports
+0000e280: 3a20 6164 6420 706f 7274 7320 6d61 726b  : add ports mark
+0000e290: 6572 7320 616e 6420 6c61 6265 6c73 2074  ers and labels t
+0000e2a0: 6f20 7265 6665 7265 6e63 6573 2e0a 2020  o references..  
+0000e2b0: 2020 2020 2020 2020 2020 706f 7274 5f6d            port_m
+0000e2c0: 6172 6b65 725f 6c61 7965 723a 2066 6f72  arker_layer: for
+0000e2d0: 2074 6865 2070 6f72 7473 2e0a 0a20 2020   the ports...   
+0000e2e0: 2020 2020 204b 6579 776f 7264 2041 7267       Keyword Arg
+0000e2f0: 733a 0a20 2020 2020 2020 2020 2020 2067  s:.            g
+0000e300: 6473 7061 7468 3a20 4744 5320 6669 6c65  dspath: GDS file
+0000e310: 2070 6174 6820 746f 2077 7269 7465 2074   path to write t
+0000e320: 6f2e 0a20 2020 2020 2020 2020 2020 2067  o..            g
+0000e330: 6473 6469 723a 2064 6972 6563 746f 7279  dsdir: directory
+0000e340: 2066 6f72 2074 6865 2047 4453 2066 696c   for the GDS fil
+0000e350: 652e 2044 6566 6175 6c74 7320 746f 202f  e. Defaults to /
+0000e360: 746d 702f 2e0a 2020 2020 2020 2020 2020  tmp/..          
+0000e370: 2020 756e 6974 3a20 756e 6974 2073 697a    unit: unit siz
+0000e380: 6520 666f 7220 6f62 6a65 6374 7320 696e  e for objects in
+0000e390: 206c 6962 7261 7279 2e20 3175 6d20 6279   library. 1um by
+0000e3a0: 2064 6566 6175 6c74 2e0a 2020 2020 2020   default..      
+0000e3b0: 2020 2020 2020 7072 6563 6973 696f 6e3a        precision:
+0000e3c0: 2066 6f72 206f 626a 6563 7420 6469 6d65   for object dime
+0000e3d0: 6e73 696f 6e73 2069 6e20 7468 6520 6c69  nsions in the li
+0000e3e0: 6272 6172 7920 286d 292e 2031 6e6d 2062  brary (m). 1nm b
+0000e3f0: 7920 6465 6661 756c 742e 0a20 2020 2020  y default..     
+0000e400: 2020 2020 2020 2074 696d 6573 7461 6d70         timestamp
+0000e410: 3a20 4465 6661 756c 7473 2074 6f20 3230  : Defaults to 20
+0000e420: 3139 2d31 302d 3235 2e20 4966 204e 6f6e  19-10-25. If Non
+0000e430: 6520 7573 6573 2063 7572 7265 6e74 2074  e uses current t
+0000e440: 696d 652e 0a20 2020 2020 2020 2022 2222  ime..        """
+0000e450: 0a20 2020 2020 2020 2066 726f 6d20 6764  .        from gd
+0000e460: 7366 6163 746f 7279 2e61 6464 5f70 696e  sfactory.add_pin
+0000e470: 7320 696d 706f 7274 2061 6464 5f70 696e  s import add_pin
+0000e480: 735f 7472 6961 6e67 6c65 0a20 2020 2020  s_triangle.     
+0000e490: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
+0000e4a0: 7279 2e73 686f 7720 696d 706f 7274 2073  ry.show import s
+0000e4b0: 686f 770a 0a20 2020 2020 2020 2063 6f6d  how..        com
+0000e4c0: 706f 6e65 6e74 203d 2028 0a20 2020 2020  ponent = (.     
+0000e4d0: 2020 2020 2020 2073 656c 662e 6164 645f         self.add_
+0000e4e0: 7069 6e73 5f74 7269 616e 676c 6528 706f  pins_triangle(po
+0000e4f0: 7274 5f6d 6172 6b65 725f 6c61 7965 723d  rt_marker_layer=
+0000e500: 706f 7274 5f6d 6172 6b65 725f 6c61 7965  port_marker_laye
+0000e510: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
+0000e520: 6620 7368 6f77 5f70 6f72 7473 0a20 2020  f show_ports.   
+0000e530: 2020 2020 2020 2020 2065 6c73 6520 7365           else se
+0000e540: 6c66 0a20 2020 2020 2020 2029 0a0a 2020  lf.        )..  
+0000e550: 2020 2020 2020 6966 2073 686f 775f 7375        if show_su
+0000e560: 6270 6f72 7473 3a0a 2020 2020 2020 2020  bports:.        
+0000e570: 2020 2020 636f 6d70 6f6e 656e 7420 3d20      component = 
+0000e580: 7365 6c66 2e63 6f70 7928 290a 2020 2020  self.copy().    
+0000e590: 2020 2020 2020 2020 636f 6d70 6f6e 656e          componen
+0000e5a0: 742e 6e61 6d65 203d 2073 656c 662e 6e61  t.name = self.na
+0000e5b0: 6d65 0a20 2020 2020 2020 2020 2020 2066  me.            f
+0000e5c0: 6f72 2072 6566 6572 656e 6365 2069 6e20  or reference in 
+0000e5d0: 636f 6d70 6f6e 656e 742e 7265 6665 7265  component.refere
+0000e5e0: 6e63 6573 3a0a 2020 2020 2020 2020 2020  nces:.          
+0000e5f0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000e600: 6e63 6528 636f 6d70 6f6e 656e 742c 2043  nce(component, C
+0000e610: 6f6d 706f 6e65 6e74 5265 6665 7265 6e63  omponentReferenc
+0000e620: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+0000e630: 2020 2020 2020 2020 6164 645f 7069 6e73          add_pins
+0000e640: 5f74 7269 616e 676c 6528 0a20 2020 2020  _triangle(.     
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 2020 2063 6f6d 706f 6e65 6e74 3d63 6f6d     component=com
+0000e670: 706f 6e65 6e74 2c0a 2020 2020 2020 2020  ponent,.        
+0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e690: 7265 6665 7265 6e63 653d 7265 6665 7265  reference=refere
+0000e6a0: 6e63 652c 0a20 2020 2020 2020 2020 2020  nce,.           
+0000e6b0: 2020 2020 2020 2020 2020 2020 206c 6179               lay
+0000e6c0: 6572 3d70 6f72 745f 6d61 726b 6572 5f6c  er=port_marker_l
+0000e6d0: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
+0000e6e0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000e6f0: 2020 2020 2073 686f 7728 636f 6d70 6f6e       show(compon
+0000e700: 656e 742c 202a 2a6b 7761 7267 7329 0a0a  ent, **kwargs)..
+0000e710: 2020 2020 6465 6620 5f77 7269 7465 5f6c      def _write_l
+0000e720: 6962 7261 7279 280a 2020 2020 2020 2020  ibrary(.        
+0000e730: 7365 6c66 2c0a 2020 2020 2020 2020 6764  self,.        gd
+0000e740: 7370 6174 683a 204f 7074 696f 6e61 6c5b  spath: Optional[
+0000e750: 5061 7468 5479 7065 5d20 3d20 4e6f 6e65  PathType] = None
+0000e760: 2c0a 2020 2020 2020 2020 6764 7364 6972  ,.        gdsdir
+0000e770: 3a20 4f70 7469 6f6e 616c 5b50 6174 6854  : Optional[PathT
+0000e780: 7970 655d 203d 204e 6f6e 652c 0a20 2020  ype] = None,.   
+0000e790: 2020 2020 2074 696d 6573 7461 6d70 3a20       timestamp: 
+0000e7a0: 4f70 7469 6f6e 616c 5b64 6174 6574 696d  Optional[datetim
+0000e7b0: 652e 6461 7465 7469 6d65 5d20 3d20 5f74  e.datetime] = _t
+0000e7c0: 696d 6573 7461 6d70 3230 3139 2c0a 2020  imestamp2019,.  
+0000e7d0: 2020 2020 2020 6c6f 6767 696e 673a 2062        logging: b
+0000e7e0: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+0000e7f0: 2020 2020 7769 7468 5f6f 6173 6973 3a20      with_oasis: 
+0000e800: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+0000e810: 2020 2020 2020 2a2a 6b77 6172 6773 2c0a        **kwargs,.
+0000e820: 2020 2020 2920 2d3e 2050 6174 683a 0a20      ) -> Path:. 
+0000e830: 2020 2020 2020 2022 2222 5772 6974 6520         """Write 
+0000e840: 636f 6d70 6f6e 656e 7420 746f 2047 4453  component to GDS
+0000e850: 206f 7220 4f41 5349 5320 616e 6420 7265   or OASIS and re
+0000e860: 7475 726e 7320 6764 7370 6174 682e 0a0a  turns gdspath...
+0000e870: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000e880: 2020 2020 2020 2020 2020 6764 7370 6174            gdspat
+0000e890: 683a 2047 4453 2066 696c 6520 7061 7468  h: GDS file path
+0000e8a0: 2074 6f20 7772 6974 6520 746f 2e0a 2020   to write to..  
+0000e8b0: 2020 2020 2020 2020 2020 6764 7364 6972            gdsdir
+0000e8c0: 3a20 6469 7265 6374 6f72 7920 666f 7220  : directory for 
+0000e8d0: 7468 6520 4744 5320 6669 6c65 2e20 4465  the GDS file. De
+0000e8e0: 6661 756c 7473 2074 6f20 2f74 6d70 2f72  faults to /tmp/r
+0000e8f0: 616e 646f 6d46 696c 652f 6764 7366 6163  andomFile/gdsfac
+0000e900: 746f 7279 2e0a 2020 2020 2020 2020 2020  tory..          
+0000e910: 2020 7469 6d65 7374 616d 703a 2044 6566    timestamp: Def
+0000e920: 6175 6c74 7320 746f 2032 3031 392d 3130  aults to 2019-10
+0000e930: 2d32 3520 666f 7220 636f 6e73 6973 7465  -25 for consiste
+0000e940: 6e74 2068 6173 682e 0a20 2020 2020 2020  nt hash..       
+0000e950: 2020 2020 2020 2020 2049 6620 4e6f 6e65           If None
+0000e960: 2075 7365 7320 6375 7272 656e 7420 7469   uses current ti
+0000e970: 6d65 2e0a 2020 2020 2020 2020 2020 2020  me..            
+0000e980: 6c6f 6767 696e 673a 2064 6973 6162 6c65  logging: disable
+0000e990: 2047 4453 2070 6174 6820 6c6f 6767 696e   GDS path loggin
+0000e9a0: 672c 2066 6f72 2065 7861 6d70 6c65 2066  g, for example f
+0000e9b0: 6f72 2073 686f 7769 6e67 2069 7420 696e  or showing it in
+0000e9c0: 204b 4c61 796f 7574 2e0a 2020 2020 2020   KLayout..      
+0000e9d0: 2020 2020 2020 7769 7468 5f6f 6173 6973        with_oasis
+0000e9e0: 3a20 4966 2054 7275 652c 2066 696c 6520  : If True, file 
+0000e9f0: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
+0000ea00: 746f 204f 4153 4953 2e20 4f74 6865 7277  to OASIS. Otherw
+0000ea10: 6973 652c 2066 696c 6520 7769 6c6c 2062  ise, file will b
+0000ea20: 6520 7772 6974 7465 6e20 746f 2047 4453  e written to GDS
+0000ea30: 2e0a 0a20 2020 2020 2020 204b 6579 776f  ...        Keywo
+0000ea40: 7264 2041 7267 733a 0a20 2020 2020 2020  rd Args:.       
+0000ea50: 2020 2020 204b 6579 776f 7264 2061 7267       Keyword arg
+0000ea60: 756d 656e 7473 2077 696c 6c20 6f76 6572  uments will over
+0000ea70: 7269 6465 2074 6865 2061 6374 6976 6520  ride the active 
+0000ea80: 5044 4b27 7320 6465 6661 756c 7420 4764  PDK's default Gd
+0000ea90: 7357 7269 7465 5365 7474 696e 6773 2061  sWriteSettings a
+0000eaa0: 6e64 204f 6173 6973 5772 6974 6553 6574  nd OasisWriteSet
+0000eab0: 7469 6e67 732e 0a0a 2020 2020 2020 2020  tings...        
+0000eac0: 2020 2020 4764 7320 7365 7474 696e 6773      Gds settings
+0000ead0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000eae0: 2020 756e 6974 3a20 756e 6974 2073 697a    unit: unit siz
+0000eaf0: 6520 666f 7220 6f62 6a65 6374 7320 696e  e for objects in
+0000eb00: 206c 6962 7261 7279 2e20 3175 6d20 6279   library. 1um by
+0000eb10: 2064 6566 6175 6c74 2e0a 2020 2020 2020   default..      
+0000eb20: 2020 2020 2020 2020 2020 7072 6563 6973            precis
+0000eb30: 696f 6e3a 2066 6f72 2064 696d 656e 7369  ion: for dimensi
+0000eb40: 6f6e 7320 696e 2074 6865 206c 6962 7261  ons in the libra
+0000eb50: 7279 2028 6d29 2e20 316e 6d20 6279 2064  ry (m). 1nm by d
+0000eb60: 6566 6175 6c74 2e0a 2020 2020 2020 2020  efault..        
+0000eb70: 2020 2020 2020 2020 6f6e 5f64 7570 6c69          on_dupli
+0000eb80: 6361 7465 5f63 656c 6c3a 2073 7065 6369  cate_cell: speci
+0000eb90: 6679 2068 6f77 2074 6f20 7265 736f 6c76  fy how to resolv
+0000eba0: 6520 6475 706c 6963 6174 652d 6e61 6d65  e duplicate-name
+0000ebb0: 6420 6365 6c6c 732e 2043 686f 6f73 6520  d cells. Choose 
+0000ebc0: 6f6e 6520 6f66 2074 6865 2066 6f6c 6c6f  one of the follo
+0000ebd0: 7769 6e67 3a0a 2020 2020 2020 2020 2020  wing:.          
+0000ebe0: 2020 2020 2020 2020 2020 2277 6172 6e22            "warn"
+0000ebf0: 2028 6465 6661 756c 7429 3a20 6f76 6572   (default): over
+0000ec00: 7772 6974 6520 616c 6c20 6475 706c 6963  write all duplic
+0000ec10: 6174 6520 6365 6c6c 7320 7769 7468 206f  ate cells with o
+0000ec20: 6e65 206f 6620 7468 6520 6475 706c 6963  ne of the duplic
+0000ec30: 6174 6573 2028 6172 6269 7472 6172 696c  ates (arbitraril
+0000ec40: 7929 2e0a 2020 2020 2020 2020 2020 2020  y)..            
+0000ec50: 2020 2020 2020 2020 2265 7272 6f72 223a          "error":
+0000ec60: 2074 6872 6f77 2061 2056 616c 7565 4572   throw a ValueEr
+0000ec70: 726f 7220 7768 656e 2061 7474 656d 7074  ror when attempt
+0000ec80: 696e 6720 746f 2077 7269 7465 2061 2067  ing to write a g
+0000ec90: 6473 2077 6974 6820 6475 706c 6963 6174  ds with duplicat
+0000eca0: 6520 6365 6c6c 732e 0a20 2020 2020 2020  e cells..       
+0000ecb0: 2020 2020 2020 2020 2020 2020 2022 6f76               "ov
+0000ecc0: 6572 7772 6974 6522 3a20 6f76 6572 7772  erwrite": overwr
+0000ecd0: 6974 6520 616c 6c20 6475 706c 6963 6174  ite all duplicat
+0000ece0: 6520 6365 6c6c 7320 7769 7468 206f 6e65  e cells with one
+0000ecf0: 206f 6620 7468 6520 6475 706c 6963 6174   of the duplicat
+0000ed00: 6573 2c20 7769 7468 6f75 7420 7761 726e  es, without warn
+0000ed10: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
+0000ed20: 2020 2020 2020 2020 204e 6f6e 653a 2064           None: d
+0000ed30: 6f20 6e6f 7420 7472 7920 746f 2072 6573  o not try to res
+0000ed40: 6f6c 7665 2028 6174 2079 6f75 7220 6f77  olve (at your ow
+0000ed50: 6e20 7269 736b 2129 0a20 2020 2020 2020  n risk!).       
+0000ed60: 2020 2020 2020 2020 2066 6c61 7474 656e           flatten
+0000ed70: 5f69 6e76 616c 6964 5f72 6566 733a 2066  _invalid_refs: f
+0000ed80: 6c61 7474 656e 7320 636f 6d70 6f6e 656e  lattens componen
+0000ed90: 7420 7265 6665 7265 6e63 6573 2077 6869  t references whi
+0000eda0: 6368 2068 6176 6520 696e 7661 6c69 6420  ch have invalid 
+0000edb0: 7472 616e 7366 6f72 6d61 7469 6f6e 732e  transformations.
+0000edc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000edd0: 206d 6178 5f70 6f69 6e74 733a 204d 6178   max_points: Max
+0000ede0: 696d 616c 206e 756d 6265 7220 6f66 2076  imal number of v
+0000edf0: 6572 7469 6365 7320 7065 7220 706f 6c79  ertices per poly
+0000ee00: 676f 6e2e 2050 6f6c 7967 6f6e 7320 7769  gon. Polygons wi
+0000ee10: 7468 206d 6f72 6520 7665 7274 6963 6573  th more vertices
+0000ee20: 2074 6861 7420 7468 6973 2061 7265 2061   that this are a
+0000ee30: 7574 6f6d 6174 6963 616c 6c79 2066 7261  utomatically fra
+0000ee40: 6374 7572 6564 2e0a 0a20 2020 2020 2020  ctured...       
+0000ee50: 2020 2020 204f 6173 6973 2073 6574 7469       Oasis setti
+0000ee60: 6e67 733a 0a20 2020 2020 2020 2020 2020  ngs:.           
+0000ee70: 2020 2020 2063 6f6d 7072 6573 7369 6f6e       compression
+0000ee80: 5f6c 6576 656c 3a20 4c65 7665 6c20 6f66  _level: Level of
+0000ee90: 2063 6f6d 7072 6573 7369 6f6e 2066 6f72   compression for
+0000eea0: 2063 656c 6c73 2028 6265 7477 6565 6e20   cells (between 
+0000eeb0: 3020 616e 6420 3929 2e0a 2020 2020 2020  0 and 9)..      
+0000eec0: 2020 2020 2020 2020 2020 2020 2020 5365                Se
+0000eed0: 7474 696e 6720 746f 2030 2077 696c 6c20  tting to 0 will 
+0000eee0: 6469 7361 626c 6520 6365 6c6c 2063 6f6d  disable cell com
+0000eef0: 7072 6573 7369 6f6e 2c20 3120 6769 7665  pression, 1 give
+0000ef00: 7320 7468 6520 6265 7374 2073 7065 6564  s the best speed
+0000ef10: 2061 6e64 2039 2c20 7468 6520 6265 7374   and 9, the best
+0000ef20: 2063 6f6d 7072 6573 7369 6f6e 2e0a 2020   compression..  
+0000ef30: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000ef40: 7465 6374 5f72 6563 7461 6e67 6c65 733a  tect_rectangles:
+0000ef50: 2053 746f 7265 2072 6563 7461 6e67 6c65   Store rectangle
+0000ef60: 7320 696e 2063 6f6d 7072 6573 7365 6420  s in compressed 
+0000ef70: 666f 726d 6174 2e0a 2020 2020 2020 2020  format..        
+0000ef80: 2020 2020 2020 2020 6465 7465 6374 5f74          detect_t
+0000ef90: 7261 7065 7a6f 6964 733a 2053 746f 7265  rapezoids: Store
+0000efa0: 2074 7261 7065 7a6f 6964 7320 696e 2063   trapezoids in c
+0000efb0: 6f6d 7072 6573 7365 6420 666f 726d 6174  ompressed format
+0000efc0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000efd0: 2020 6369 7263 6c65 5f74 6f6c 6572 616e    circle_toleran
+0000efe0: 6365 3a20 546f 6c65 7261 6e63 6520 666f  ce: Tolerance fo
+0000eff0: 7220 6465 7465 6374 696e 6720 6369 7263  r detecting circ
+0000f000: 6c65 732e 2049 6620 6c65 7373 206f 7220  les. If less or 
+0000f010: 6571 7561 6c20 746f 2030 2c20 6e6f 2064  equal to 0, no d
+0000f020: 6574 6563 7469 6f6e 2069 7320 7065 7266  etection is perf
+0000f030: 6f72 6d65 642e 2043 6972 636c 6573 2061  ormed. Circles a
+0000f040: 7265 2073 746f 7265 6420 696e 2063 6f6d  re stored in com
+0000f050: 7072 6573 7365 6420 666f 726d 6174 2e0a  pressed format..
+0000f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f070: 7661 6c69 6461 7469 6f6e 2028 2263 7263  validation ("crc
+0000f080: 3332 222c 2022 6368 6563 6b73 756d 3332  32", "checksum32
+0000f090: 222c 204e 6f6e 6529 3a20 7479 7065 206f  ", None): type o
+0000f0a0: 6620 7661 6c69 6461 7469 6f6e 2074 6f20  f validation to 
+0000f0b0: 696e 636c 7564 6520 696e 2074 6865 2073  include in the s
+0000f0c0: 6176 6564 2066 696c 652e 0a20 2020 2020  aved file..     
+0000f0d0: 2020 2020 2020 2020 2020 2073 7461 6e64             stand
+0000f0e0: 6172 645f 7072 6f70 6572 7469 6573 3a20  ard_properties: 
+0000f0f0: 5374 6f72 6520 7374 616e 6461 7264 204f  Store standard O
+0000f100: 4153 4953 2070 726f 7065 7274 6965 7320  ASIS properties 
+0000f110: 696e 2074 6865 2066 696c 652e 0a0a 2020  in the file...  
+0000f120: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0000f130: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
+0000f140: 7279 2e70 646b 2069 6d70 6f72 7420 6765  ry.pdk import ge
+0000f150: 745f 6163 7469 7665 5f70 646b 0a0a 2020  t_active_pdk..  
+0000f160: 2020 2020 2020 6966 2067 6473 7061 7468        if gdspath
+0000f170: 2061 6e64 2067 6473 6469 723a 0a20 2020   and gdsdir:.   
+0000f180: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0000f190: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+0000f1a0: 2020 2020 2020 2020 2267 6473 7061 7468          "gdspath
+0000f1b0: 2061 6e64 2067 6473 6469 7220 6861 7665   and gdsdir have
+0000f1c0: 2062 6f74 6820 6265 656e 2073 7065 6369   both been speci
+0000f1d0: 6669 6564 2e20 6764 7370 6174 6820 7769  fied. gdspath wi
+0000f1e0: 6c6c 2074 616b 6520 7072 6563 6564 656e  ll take preceden
+0000f1f0: 6365 2061 6e64 2067 6473 6469 7220 7769  ce and gdsdir wi
+0000f200: 6c6c 2062 6520 6967 6e6f 7265 642e 220a  ll be ignored.".
+0000f210: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000f220: 2020 2020 2020 2064 6566 6175 6c74 5f73         default_s
+0000f230: 6574 7469 6e67 7320 3d20 6765 745f 6163  ettings = get_ac
+0000f240: 7469 7665 5f70 646b 2829 2e67 6473 5f77  tive_pdk().gds_w
+0000f250: 7269 7465 5f73 6574 7469 6e67 730a 2020  rite_settings.  
+0000f260: 2020 2020 2020 6465 6661 756c 745f 6f61        default_oa
+0000f270: 7369 735f 7365 7474 696e 6773 203d 2067  sis_settings = g
+0000f280: 6574 5f61 6374 6976 655f 7064 6b28 292e  et_active_pdk().
+0000f290: 6f61 7369 735f 7365 7474 696e 6773 0a0a  oasis_settings..
+0000f2a0: 2020 2020 2020 2020 6578 706c 6963 6974          explicit
+0000f2b0: 5f67 6473 5f73 6574 7469 6e67 7320 3d20  _gds_settings = 
+0000f2c0: 7b0a 2020 2020 2020 2020 2020 2020 6b3a  {.            k:
+0000f2d0: 2076 0a20 2020 2020 2020 2020 2020 2066   v.            f
+0000f2e0: 6f72 206b 2c20 7620 696e 206b 7761 7267  or k, v in kwarg
+0000f2f0: 732e 6974 656d 7328 290a 2020 2020 2020  s.items().      
+0000f300: 2020 2020 2020 6966 2076 2069 7320 6e6f        if v is no
+0000f310: 7420 4e6f 6e65 2061 6e64 206b 2069 6e20  t None and k in 
+0000f320: 6465 6661 756c 745f 7365 7474 696e 6773  default_settings
+0000f330: 2e64 6963 7428 290a 2020 2020 2020 2020  .dict().        
+0000f340: 7d0a 2020 2020 2020 2020 6578 706c 6963  }.        explic
+0000f350: 6974 5f6f 6173 5f73 6574 7469 6e67 7320  it_oas_settings 
+0000f360: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0000f370: 6b3a 2076 0a20 2020 2020 2020 2020 2020  k: v.           
+0000f380: 2066 6f72 206b 2c20 7620 696e 206b 7761   for k, v in kwa
+0000f390: 7267 732e 6974 656d 7328 290a 2020 2020  rgs.items().    
+0000f3a0: 2020 2020 2020 2020 6966 2076 2069 7320          if v is 
+0000f3b0: 6e6f 7420 4e6f 6e65 2061 6e64 206b 2069  not None and k i
+0000f3c0: 6e20 6465 6661 756c 745f 6f61 7369 735f  n default_oasis_
+0000f3d0: 7365 7474 696e 6773 2e64 6963 7428 290a  settings.dict().
+0000f3e0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0000f3f0: 2020 2320 7570 6461 7465 2074 6865 2077    # update the w
+0000f400: 7269 7465 2073 6574 7469 6e67 7320 7769  rite settings wi
+0000f410: 7468 2061 6e79 2073 6574 7469 6e67 7320  th any settings 
+0000f420: 6578 706c 6963 6974 6c79 2070 6173 7365  explicitly passe
+0000f430: 640a 2020 2020 2020 2020 7772 6974 655f  d.        write_
+0000f440: 7365 7474 696e 6773 203d 2064 6566 6175  settings = defau
+0000f450: 6c74 5f73 6574 7469 6e67 732e 636f 7079  lt_settings.copy
+0000f460: 2875 7064 6174 653d 6578 706c 6963 6974  (update=explicit
+0000f470: 5f67 6473 5f73 6574 7469 6e67 7329 0a20  _gds_settings). 
+0000f480: 2020 2020 2020 206f 6173 6973 5f73 6574         oasis_set
+0000f490: 7469 6e67 7320 3d20 6465 6661 756c 745f  tings = default_
+0000f4a0: 6f61 7369 735f 7365 7474 696e 6773 2e63  oasis_settings.c
+0000f4b0: 6f70 7928 7570 6461 7465 3d65 7870 6c69  opy(update=expli
+0000f4c0: 6369 745f 6f61 735f 7365 7474 696e 6773  cit_oas_settings
+0000f4d0: 290a 0a20 2020 2020 2020 205f 6368 6563  )..        _chec
+0000f4e0: 6b5f 756e 6361 6368 6564 5f63 6f6d 706f  k_uncached_compo
+0000f4f0: 6e65 6e74 7328 0a20 2020 2020 2020 2020  nents(.         
+0000f500: 2020 2063 6f6d 706f 6e65 6e74 3d73 656c     component=sel
+0000f510: 662c 206d 6f64 653d 7772 6974 655f 7365  f, mode=write_se
+0000f520: 7474 696e 6773 2e6f 6e5f 756e 6361 6368  ttings.on_uncach
+0000f530: 6564 5f63 6f6d 706f 6e65 6e74 0a20 2020  ed_component.   
+0000f540: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000f550: 6966 2077 7269 7465 5f73 6574 7469 6e67  if write_setting
+0000f560: 732e 666c 6174 7465 6e5f 696e 7661 6c69  s.flatten_invali
+0000f570: 645f 7265 6673 3a0a 2020 2020 2020 2020  d_refs:.        
+0000f580: 2020 2020 746f 705f 6365 6c6c 203d 2066      top_cell = f
+0000f590: 6c61 7474 656e 5f69 6e76 616c 6964 5f72  latten_invalid_r
+0000f5a0: 6566 735f 7265 6375 7273 6976 6528 7365  efs_recursive(se
+0000f5b0: 6c66 290a 2020 2020 2020 2020 656c 7365  lf).        else
+0000f5c0: 3a0a 2020 2020 2020 2020 2020 2020 746f  :.            to
+0000f5d0: 705f 6365 6c6c 203d 2073 656c 660a 0a20  p_cell = self.. 
+0000f5e0: 2020 2020 2020 2067 6473 6469 7220 3d20         gdsdir = 
+0000f5f0: 6764 7364 6972 206f 7220 4744 5344 4952  gdsdir or GDSDIR
+0000f600: 5f54 454d 500a 2020 2020 2020 2020 6764  _TEMP.        gd
+0000f610: 7364 6972 203d 2070 6174 686c 6962 2e50  sdir = pathlib.P
+0000f620: 6174 6828 6764 7364 6972 290a 2020 2020  ath(gdsdir).    
+0000f630: 2020 2020 6966 2077 6974 685f 6f61 7369      if with_oasi
+0000f640: 733a 0a20 2020 2020 2020 2020 2020 2067  s:.            g
+0000f650: 6473 7061 7468 203d 2067 6473 7061 7468  dspath = gdspath
+0000f660: 206f 7220 6764 7364 6972 202f 2066 227b   or gdsdir / f"{
+0000f670: 746f 705f 6365 6c6c 2e6e 616d 657d 2e6f  top_cell.name}.o
+0000f680: 6173 220a 2020 2020 2020 2020 656c 7365  as".        else
+0000f690: 3a0a 2020 2020 2020 2020 2020 2020 6764  :.            gd
+0000f6a0: 7370 6174 6820 3d20 6764 7370 6174 6820  spath = gdspath 
+0000f6b0: 6f72 2067 6473 6469 7220 2f20 6622 7b74  or gdsdir / f"{t
+0000f6c0: 6f70 5f63 656c 6c2e 6e61 6d65 7d2e 6764  op_cell.name}.gd
+0000f6d0: 7322 0a20 2020 2020 2020 2067 6473 7061  s".        gdspa
+0000f6e0: 7468 203d 2070 6174 686c 6962 2e50 6174  th = pathlib.Pat
+0000f6f0: 6828 6764 7370 6174 6829 0a20 2020 2020  h(gdspath).     
+0000f700: 2020 2067 6473 6469 7220 3d20 6764 7370     gdsdir = gdsp
+0000f710: 6174 682e 7061 7265 6e74 0a20 2020 2020  ath.parent.     
+0000f720: 2020 2067 6473 6469 722e 6d6b 6469 7228     gdsdir.mkdir(
+0000f730: 6578 6973 745f 6f6b 3d54 7275 652c 2070  exist_ok=True, p
+0000f740: 6172 656e 7473 3d54 7275 6529 0a0a 2020  arents=True)..  
+0000f750: 2020 2020 2020 6365 6c6c 7320 3d20 746f        cells = to
+0000f760: 705f 6365 6c6c 2e67 6574 5f64 6570 656e  p_cell.get_depen
+0000f770: 6465 6e63 6965 7328 7265 6375 7273 6976  dencies(recursiv
+0000f780: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+0000f790: 6365 6c6c 5f6e 616d 6573 203d 205b 6365  cell_names = [ce
+0000f7a0: 6c6c 2e6e 616d 6520 666f 7220 6365 6c6c  ll.name for cell
+0000f7b0: 2069 6e20 6c69 7374 2863 656c 6c73 295d   in list(cells)]
+0000f7c0: 0a20 2020 2020 2020 2063 656c 6c5f 6e61  .        cell_na
+0000f7d0: 6d65 735f 756e 6971 7565 203d 2073 6574  mes_unique = set
+0000f7e0: 2863 656c 6c5f 6e61 6d65 7329 0a0a 2020  (cell_names)..  
+0000f7f0: 2020 2020 2020 6966 206c 656e 2863 656c        if len(cel
+0000f800: 6c5f 6e61 6d65 7329 2021 3d20 6c65 6e28  l_names) != len(
+0000f810: 7365 7428 6365 6c6c 5f6e 616d 6573 2929  set(cell_names))
+0000f820: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+0000f830: 7220 6365 6c6c 5f6e 616d 6520 696e 2063  r cell_name in c
+0000f840: 656c 6c5f 6e61 6d65 735f 756e 6971 7565  ell_names_unique
+0000f850: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f860: 2020 6365 6c6c 5f6e 616d 6573 2e72 656d    cell_names.rem
+0000f870: 6f76 6528 6365 6c6c 5f6e 616d 6529 0a0a  ove(cell_name)..
+0000f880: 2020 2020 2020 2020 2020 2020 6966 2077              if w
+0000f890: 7269 7465 5f73 6574 7469 6e67 732e 6f6e  rite_settings.on
+0000f8a0: 5f64 7570 6c69 6361 7465 5f63 656c 6c20  _duplicate_cell 
+0000f8b0: 3d3d 2022 6572 726f 7222 3a0a 2020 2020  == "error":.    
+0000f8c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000f8d0: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8f0: 2020 6622 4475 706c 6963 6174 6564 2063    f"Duplicated c
+0000f900: 656c 6c20 6e61 6d65 7320 696e 207b 746f  ell names in {to
+0000f910: 705f 6365 6c6c 2e6e 616d 6521 727d 3a20  p_cell.name!r}: 
+0000f920: 7b63 656c 6c5f 6e61 6d65 7321 727d 220a  {cell_names!r}".
+0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f940: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000f950: 6966 2077 7269 7465 5f73 6574 7469 6e67  if write_setting
+0000f960: 732e 6f6e 5f64 7570 6c69 6361 7465 5f63  s.on_duplicate_c
+0000f970: 656c 6c20 696e 207b 2277 6172 6e22 2c20  ell in {"warn", 
+0000f980: 226f 7665 7277 7269 7465 227d 3a0a 2020  "overwrite"}:.  
+0000f990: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000f9a0: 2077 7269 7465 5f73 6574 7469 6e67 732e   write_settings.
+0000f9b0: 6f6e 5f64 7570 6c69 6361 7465 5f63 656c  on_duplicate_cel
+0000f9c0: 6c20 3d3d 2022 7761 726e 223a 0a20 2020  l == "warn":.   
+0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9e0: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
+0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa00: 2020 2020 2020 2020 6622 4475 706c 6963          f"Duplic
+0000fa10: 6174 6564 2063 656c 6c20 6e61 6d65 7320  ated cell names 
+0000fa20: 696e 207b 746f 705f 6365 6c6c 2e6e 616d  in {top_cell.nam
+0000fa30: 6521 727d 3a20 207b 6365 6c6c 5f6e 616d  e!r}:  {cell_nam
+0000fa40: 6573 7d22 2c0a 2020 2020 2020 2020 2020  es}",.          
+0000fa50: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000fa60: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+0000fa70: 735f 6469 6374 203d 207b 6365 6c6c 2e6e  s_dict = {cell.n
+0000fa80: 616d 653a 2063 656c 6c2e 5f63 656c 6c20  ame: cell._cell 
+0000fa90: 666f 7220 6365 6c6c 2069 6e20 6365 6c6c  for cell in cell
+0000faa0: 737d 0a20 2020 2020 2020 2020 2020 2020  s}.             
+0000fab0: 2020 2063 656c 6c73 203d 2063 656c 6c73     cells = cells
+0000fac0: 5f64 6963 742e 7661 6c75 6573 2829 0a20  _dict.values(). 
+0000fad0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0000fae0: 7772 6974 655f 7365 7474 696e 6773 2e6f  write_settings.o
+0000faf0: 6e5f 6475 706c 6963 6174 655f 6365 6c6c  n_duplicate_cell
+0000fb00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000fb10: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000fb20: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+0000fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb40: 2020 2020 6622 6f6e 5f64 7570 6c69 6361      f"on_duplica
+0000fb50: 7465 5f63 656c 6c3a 207b 7772 6974 655f  te_cell: {write_
+0000fb60: 7365 7474 696e 6773 2e6f 6e5f 6475 706c  settings.on_dupl
+0000fb70: 6963 6174 655f 6365 6c6c 2172 7d20 6e6f  icate_cell!r} no
+0000fb80: 7420 696e 2028 4e6f 6e65 2c20 7761 726e  t in (None, warn
+0000fb90: 2c20 6572 726f 722c 206f 7665 7277 7269  , error, overwri
+0000fba0: 7465 2922 0a20 2020 2020 2020 2020 2020  te)".           
+0000fbb0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000fbc0: 616c 6c5f 6365 6c6c 7320 3d20 5b74 6f70  all_cells = [top
+0000fbd0: 5f63 656c 6c2e 5f63 656c 6c5d 202b 2073  _cell._cell] + s
+0000fbe0: 6f72 7465 6428 6365 6c6c 732c 206b 6579  orted(cells, key
+0000fbf0: 3d6c 616d 6264 6120 6363 3a20 6363 2e6e  =lambda cc: cc.n
+0000fc00: 616d 6529 0a0a 2020 2020 2020 2020 6e6f  ame)..        no
+0000fc10: 5f6e 616d 655f 6365 6c6c 7320 3d20 5b0a  _name_cells = [.
+0000fc20: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+0000fc30: 2e6e 616d 6520 666f 7220 6365 6c6c 2069  .name for cell i
+0000fc40: 6e20 616c 6c5f 6365 6c6c 7320 6966 2063  n all_cells if c
+0000fc50: 656c 6c2e 6e61 6d65 2e73 7461 7274 7377  ell.name.startsw
+0000fc60: 6974 6828 2255 6e6e 616d 6564 2229 0a20  ith("Unnamed"). 
+0000fc70: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+0000fc80: 2020 6966 206e 6f5f 6e61 6d65 5f63 656c    if no_name_cel
+0000fc90: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+0000fca0: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
+0000fcb0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000fcc0: 2243 6f6d 706f 6e65 6e74 207b 746f 705f  "Component {top_
+0000fcd0: 6365 6c6c 2e6e 616d 6521 727d 2063 6f6e  cell.name!r} con
+0000fce0: 7461 696e 7320 7b6c 656e 286e 6f5f 6e61  tains {len(no_na
+0000fcf0: 6d65 5f63 656c 6c73 297d 2055 6e6e 616d  me_cells)} Unnam
+0000fd00: 6564 2063 656c 6c73 220a 2020 2020 2020  ed cells".      
+0000fd10: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000fd20: 2023 2066 6f72 2063 656c 6c20 696e 2061   # for cell in a
+0000fd30: 6c6c 5f63 656c 6c73 3a0a 2020 2020 2020  ll_cells:.      
+0000fd40: 2020 2320 2020 2020 7072 696e 7428 6365    #     print(ce
+0000fd50: 6c6c 2e6e 616d 652c 2074 7970 6528 6365  ll.name, type(ce
+0000fd60: 6c6c 2929 0a0a 2020 2020 2020 2020 6c69  ll))..        li
+0000fd70: 6220 3d20 6764 7374 6b2e 4c69 6272 6172  b = gdstk.Librar
+0000fd80: 7928 0a20 2020 2020 2020 2020 2020 2075  y(.            u
+0000fd90: 6e69 743d 7772 6974 655f 7365 7474 696e  nit=write_settin
+0000fda0: 6773 2e75 6e69 742c 2070 7265 6369 7369  gs.unit, precisi
+0000fdb0: 6f6e 3d77 7269 7465 5f73 6574 7469 6e67  on=write_setting
+0000fdc0: 732e 7072 6563 6973 696f 6e0a 2020 2020  s.precision.    
+0000fdd0: 2020 2020 290a 2020 2020 2020 2020 6c69      ).        li
+0000fde0: 622e 6164 6428 746f 705f 6365 6c6c 2e5f  b.add(top_cell._
+0000fdf0: 6365 6c6c 290a 2020 2020 2020 2020 6c69  cell).        li
+0000fe00: 622e 6164 6428 2a74 6f70 5f63 656c 6c2e  b.add(*top_cell.
+0000fe10: 5f63 656c 6c2e 6465 7065 6e64 656e 6369  _cell.dependenci
+0000fe20: 6573 2854 7275 6529 290a 0a20 2020 2020  es(True))..     
+0000fe30: 2020 2069 6620 7769 7468 5f6f 6173 6973     if with_oasis
+0000fe40: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
+0000fe50: 622e 7772 6974 655f 6f61 7328 6764 7370  b.write_oas(gdsp
+0000fe60: 6174 682c 202a 2a6f 6173 6973 5f73 6574  ath, **oasis_set
+0000fe70: 7469 6e67 732e 6469 6374 2829 290a 2020  tings.dict()).  
+0000fe80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000fe90: 2020 2020 2020 2020 6c69 622e 7772 6974          lib.writ
+0000fea0: 655f 6764 7328 0a20 2020 2020 2020 2020  e_gds(.         
+0000feb0: 2020 2020 2020 2067 6473 7061 7468 2c20         gdspath, 
+0000fec0: 7469 6d65 7374 616d 703d 7469 6d65 7374  timestamp=timest
+0000fed0: 616d 702c 206d 6178 5f70 6f69 6e74 733d  amp, max_points=
+0000fee0: 7772 6974 655f 7365 7474 696e 6773 2e6d  write_settings.m
+0000fef0: 6178 5f70 6f69 6e74 730a 2020 2020 2020  ax_points.      
+0000ff00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000ff10: 6966 206c 6f67 6769 6e67 3a0a 2020 2020  if logging:.    
+0000ff20: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+0000ff30: 6e66 6f28 6622 5772 6f74 6520 746f 207b  nfo(f"Wrote to {
+0000ff40: 7374 7228 6764 7370 6174 6829 2172 7d22  str(gdspath)!r}"
+0000ff50: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000ff60: 2067 6473 7061 7468 0a0a 2020 2020 6465   gdspath..    de
+0000ff70: 6620 7772 6974 655f 6764 7328 0a20 2020  f write_gds(.   
+0000ff80: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000ff90: 2020 2067 6473 7061 7468 3a20 4f70 7469     gdspath: Opti
+0000ffa0: 6f6e 616c 5b50 6174 6854 7970 655d 203d  onal[PathType] =
+0000ffb0: 204e 6f6e 652c 0a20 2020 2020 2020 2067   None,.        g
+0000ffc0: 6473 6469 723a 204f 7074 696f 6e61 6c5b  dsdir: Optional[
+0000ffd0: 5061 7468 5479 7065 5d20 3d20 4e6f 6e65  PathType] = None
+0000ffe0: 2c0a 2020 2020 2020 2020 2a2a 6b77 6172  ,.        **kwar
+0000fff0: 6773 2c0a 2020 2020 2920 2d3e 2050 6174  gs,.    ) -> Pat
+00010000: 683a 0a20 2020 2020 2020 2022 2222 5772  h:.        """Wr
+00010010: 6974 6520 636f 6d70 6f6e 656e 7420 746f  ite component to
+00010020: 2047 4453 2061 6e64 2072 6574 7572 6e73   GDS and returns
+00010030: 2067 6473 7061 7468 2e0a 0a20 2020 2020   gdspath...     
+00010040: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00010050: 2020 2020 2067 6473 7061 7468 3a20 4744       gdspath: GD
+00010060: 5320 6669 6c65 2070 6174 6820 746f 2077  S file path to w
+00010070: 7269 7465 2074 6f2e 0a20 2020 2020 2020  rite to..       
+00010080: 2020 2020 2067 6473 6469 723a 2064 6972       gdsdir: dir
+00010090: 6563 746f 7279 2066 6f72 2074 6865 2047  ectory for the G
+000100a0: 4453 2066 696c 652e 2044 6566 6175 6c74  DS file. Default
+000100b0: 7320 746f 202f 746d 702f 7261 6e64 6f6d  s to /tmp/random
+000100c0: 4669 6c65 2f67 6473 6661 6374 6f72 792e  File/gdsfactory.
+000100d0: 0a0a 2020 2020 2020 2020 4b65 7977 6f72  ..        Keywor
+000100e0: 6420 4172 6773 3a0a 2020 2020 2020 2020  d Args:.        
+000100f0: 2020 2020 756e 6974 3a20 756e 6974 2073      unit: unit s
+00010100: 697a 6520 666f 7220 6f62 6a65 6374 7320  ize for objects 
+00010110: 696e 206c 6962 7261 7279 2e20 3175 6d20  in library. 1um 
+00010120: 6279 2064 6566 6175 6c74 2e0a 2020 2020  by default..    
+00010130: 2020 2020 2020 2020 7072 6563 6973 696f          precisio
+00010140: 6e3a 2066 6f72 2064 696d 656e 7369 6f6e  n: for dimension
+00010150: 7320 696e 2074 6865 206c 6962 7261 7279  s in the library
+00010160: 2028 6d29 2e20 316e 6d20 6279 2064 6566   (m). 1nm by def
+00010170: 6175 6c74 2e0a 2020 2020 2020 2020 2020  ault..          
+00010180: 2020 6c6f 6767 696e 673a 2064 6973 6162    logging: disab
+00010190: 6c65 2047 4453 2070 6174 6820 6c6f 6767  le GDS path logg
+000101a0: 696e 672c 2066 6f72 2065 7861 6d70 6c65  ing, for example
+000101b0: 2066 6f72 2073 686f 7769 6e67 2069 7420   for showing it 
+000101c0: 696e 204b 4c61 796f 7574 2e0a 2020 2020  in KLayout..    
+000101d0: 2020 2020 2020 2020 6f6e 5f64 7570 6c69          on_dupli
+000101e0: 6361 7465 5f63 656c 6c3a 2073 7065 6369  cate_cell: speci
+000101f0: 6679 2068 6f77 2074 6f20 7265 736f 6c76  fy how to resolv
+00010200: 6520 6475 706c 6963 6174 652d 6e61 6d65  e duplicate-name
+00010210: 6420 6365 6c6c 732e 2043 686f 6f73 6520  d cells. Choose 
+00010220: 6f6e 6520 6f66 2074 6865 2066 6f6c 6c6f  one of the follo
+00010230: 7769 6e67 3a0a 2020 2020 2020 2020 2020  wing:.          
+00010240: 2020 2020 2020 2277 6172 6e22 2028 6465        "warn" (de
+00010250: 6661 756c 7429 3a20 6f76 6572 7772 6974  fault): overwrit
+00010260: 6520 616c 6c20 6475 706c 6963 6174 6520  e all duplicate 
+00010270: 6365 6c6c 7320 7769 7468 206f 6e65 206f  cells with one o
+00010280: 6620 7468 6520 6475 706c 6963 6174 6573  f the duplicates
+00010290: 2028 6172 6269 7472 6172 696c 7929 2e0a   (arbitrarily)..
+000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102b0: 2265 7272 6f72 223a 2074 6872 6f77 2061  "error": throw a
+000102c0: 2056 616c 7565 4572 726f 7220 7768 656e   ValueError when
+000102d0: 2061 7474 656d 7074 696e 6720 746f 2077   attempting to w
+000102e0: 7269 7465 2061 2067 6473 2077 6974 6820  rite a gds with 
+000102f0: 6475 706c 6963 6174 6520 6365 6c6c 732e  duplicate cells.
+00010300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010310: 2022 6f76 6572 7772 6974 6522 3a20 6f76   "overwrite": ov
+00010320: 6572 7772 6974 6520 616c 6c20 6475 706c  erwrite all dupl
+00010330: 6963 6174 6520 6365 6c6c 7320 7769 7468  icate cells with
+00010340: 206f 6e65 206f 6620 7468 6520 6475 706c   one of the dupl
+00010350: 6963 6174 6573 2c20 7769 7468 6f75 7420  icates, without 
+00010360: 7761 726e 696e 672e 0a20 2020 2020 2020  warning..       
+00010370: 2020 2020 206f 6e5f 756e 6361 6368 6564       on_uncached
+00010380: 5f63 6f6d 706f 6e65 6e74 3a20 4c69 7465  _component: Lite
+00010390: 7261 6c5b 2277 6172 6e22 2c20 2265 7272  ral["warn", "err
+000103a0: 6f72 225d 203d 2022 7761 726e 220a 2020  or"] = "warn".  
+000103b0: 2020 2020 2020 2020 2020 666c 6174 7465            flatte
+000103c0: 6e5f 696e 7661 6c69 645f 7265 6673 3a20  n_invalid_refs: 
+000103d0: 666c 6174 7465 6e73 2063 6f6d 706f 6e65  flattens compone
+000103e0: 6e74 2072 6566 6572 656e 6365 7320 7768  nt references wh
+000103f0: 6963 6820 6861 7665 2069 6e76 616c 6964  ich have invalid
+00010400: 2074 7261 6e73 666f 726d 6174 696f 6e73   transformations
+00010410: 2e0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+00010420: 785f 706f 696e 7473 3a20 4d61 7869 6d61  x_points: Maxima
+00010430: 6c20 6e75 6d62 6572 206f 6620 7665 7274  l number of vert
+00010440: 6963 6573 2070 6572 2070 6f6c 7967 6f6e  ices per polygon
+00010450: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010460: 2020 506f 6c79 676f 6e73 2077 6974 6820    Polygons with 
+00010470: 6d6f 7265 2076 6572 7469 6365 7320 7468  more vertices th
+00010480: 6174 2074 6869 7320 6172 6520 6175 746f  at this are auto
+00010490: 6d61 7469 6361 6c6c 7920 6672 6163 7475  matically fractu
+000104a0: 7265 642e 0a20 2020 2020 2020 2022 2222  red..        """
+000104b0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000104c0: 2073 656c 662e 5f77 7269 7465 5f6c 6962   self._write_lib
+000104d0: 7261 7279 280a 2020 2020 2020 2020 2020  rary(.          
+000104e0: 2020 6764 7370 6174 683d 6764 7370 6174    gdspath=gdspat
+000104f0: 682c 2067 6473 6469 723d 6764 7364 6972  h, gdsdir=gdsdir
+00010500: 2c20 7769 7468 5f6f 6173 6973 3d46 616c  , with_oasis=Fal
+00010510: 7365 2c20 2a2a 6b77 6172 6773 0a20 2020  se, **kwargs.   
+00010520: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00010530: 7772 6974 655f 6f61 7328 0a20 2020 2020  write_oas(.     
+00010540: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00010550: 2067 6473 7061 7468 3a20 4f70 7469 6f6e   gdspath: Option
+00010560: 616c 5b50 6174 6854 7970 655d 203d 204e  al[PathType] = N
+00010570: 6f6e 652c 0a20 2020 2020 2020 2067 6473  one,.        gds
+00010580: 6469 723a 204f 7074 696f 6e61 6c5b 5061  dir: Optional[Pa
+00010590: 7468 5479 7065 5d20 3d20 4e6f 6e65 2c0a  thType] = None,.
+000105a0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+000105b0: 2c0a 2020 2020 2920 2d3e 2050 6174 683a  ,.    ) -> Path:
+000105c0: 0a20 2020 2020 2020 2022 2222 5772 6974  .        """Writ
+000105d0: 6520 636f 6d70 6f6e 656e 7420 746f 2047  e component to G
+000105e0: 4453 2061 6e64 2072 6574 7572 6e73 2067  DS and returns g
+000105f0: 6473 7061 7468 2e0a 0a20 2020 2020 2020  dspath...       
+00010600: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00010610: 2020 2067 6473 7061 7468 3a20 4744 5320     gdspath: GDS 
+00010620: 6669 6c65 2070 6174 6820 746f 2077 7269  file path to wri
+00010630: 7465 2074 6f2e 0a20 2020 2020 2020 2020  te to..         
+00010640: 2020 2067 6473 6469 723a 2064 6972 6563     gdsdir: direc
+00010650: 746f 7279 2066 6f72 2074 6865 2047 4453  tory for the GDS
+00010660: 2066 696c 652e 2044 6566 6175 6c74 7320   file. Defaults 
+00010670: 746f 202f 746d 702f 7261 6e64 6f6d 4669  to /tmp/randomFi
+00010680: 6c65 2f67 6473 6661 6374 6f72 792e 0a0a  le/gdsfactory...
+00010690: 2020 2020 2020 2020 4b65 7977 6f72 6420          Keyword 
+000106a0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+000106b0: 2020 756e 6974 3a20 756e 6974 2073 697a    unit: unit siz
+000106c0: 6520 666f 7220 6f62 6a65 6374 7320 696e  e for objects in
+000106d0: 206c 6962 7261 7279 2e20 3175 6d20 6279   library. 1um by
+000106e0: 2064 6566 6175 6c74 2e0a 2020 2020 2020   default..      
+000106f0: 2020 2020 2020 7072 6563 6973 696f 6e3a        precision:
+00010700: 2066 6f72 2064 696d 656e 7369 6f6e 7320   for dimensions 
+00010710: 696e 2074 6865 206c 6962 7261 7279 2028  in the library (
+00010720: 6d29 2e20 316e 6d20 6279 2064 6566 6175  m). 1nm by defau
+00010730: 6c74 2e0a 2020 2020 2020 2020 2020 2020  lt..            
+00010740: 6c6f 6767 696e 673a 2064 6973 6162 6c65  logging: disable
+00010750: 2047 4453 2070 6174 6820 6c6f 6767 696e   GDS path loggin
+00010760: 672c 2066 6f72 2065 7861 6d70 6c65 2066  g, for example f
+00010770: 6f72 2073 686f 7769 6e67 2069 7420 696e  or showing it in
+00010780: 204b 4c61 796f 7574 2e0a 2020 2020 2020   KLayout..      
+00010790: 2020 2020 2020 6f6e 5f64 7570 6c69 6361        on_duplica
+000107a0: 7465 5f63 656c 6c3a 2073 7065 6369 6679  te_cell: specify
+000107b0: 2068 6f77 2074 6f20 7265 736f 6c76 6520   how to resolve 
+000107c0: 6475 706c 6963 6174 652d 6e61 6d65 6420  duplicate-named 
+000107d0: 6365 6c6c 732e 2043 686f 6f73 6520 6f6e  cells. Choose on
+000107e0: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
+000107f0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+00010800: 2020 2020 2277 6172 6e22 2028 6465 6661      "warn" (defa
+00010810: 756c 7429 3a20 6f76 6572 7772 6974 6520  ult): overwrite 
+00010820: 616c 6c20 6475 706c 6963 6174 6520 6365  all duplicate ce
+00010830: 6c6c 7320 7769 7468 206f 6e65 206f 6620  lls with one of 
+00010840: 7468 6520 6475 706c 6963 6174 6573 2028  the duplicates (
+00010850: 6172 6269 7472 6172 696c 7929 2e0a 2020  arbitrarily)..  
+00010860: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00010870: 7272 6f72 223a 2074 6872 6f77 2061 2056  rror": throw a V
+00010880: 616c 7565 4572 726f 7220 7768 656e 2061  alueError when a
+00010890: 7474 656d 7074 696e 6720 746f 2077 7269  ttempting to wri
+000108a0: 7465 2061 2067 6473 2077 6974 6820 6475  te a gds with du
+000108b0: 706c 6963 6174 6520 6365 6c6c 732e 0a20  plicate cells.. 
+000108c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000108d0: 6f76 6572 7772 6974 6522 3a20 6f76 6572  overwrite": over
+000108e0: 7772 6974 6520 616c 6c20 6475 706c 6963  write all duplic
+000108f0: 6174 6520 6365 6c6c 7320 7769 7468 206f  ate cells with o
+00010900: 6e65 206f 6620 7468 6520 6475 706c 6963  ne of the duplic
+00010910: 6174 6573 2c20 7769 7468 6f75 7420 7761  ates, without wa
+00010920: 726e 696e 672e 0a20 2020 2020 2020 2020  rning..         
+00010930: 2020 2020 2020 204e 6f6e 653a 2064 6f20         None: do 
+00010940: 6e6f 7420 7472 7920 746f 2072 6573 6f6c  not try to resol
+00010950: 7665 2028 6174 2079 6f75 7220 6f77 6e20  ve (at your own 
+00010960: 7269 736b 2129 0a20 2020 2020 2020 2020  risk!).         
+00010970: 2020 206f 6e5f 756e 6361 6368 6564 5f63     on_uncached_c
+00010980: 6f6d 706f 6e65 6e74 3a20 4c69 7465 7261  omponent: Litera
+00010990: 6c5b 2277 6172 6e22 2c20 2265 7272 6f72  l["warn", "error
+000109a0: 225d 203d 2022 7761 726e 220a 2020 2020  "] = "warn".    
+000109b0: 2020 2020 2020 2020 666c 6174 7465 6e5f          flatten_
+000109c0: 696e 7661 6c69 645f 7265 6673 3a20 666c  invalid_refs: fl
+000109d0: 6174 7465 6e73 2063 6f6d 706f 6e65 6e74  attens component
+000109e0: 2072 6566 6572 656e 6365 7320 7768 6963   references whic
+000109f0: 6820 6861 7665 2069 6e76 616c 6964 2074  h have invalid t
+00010a00: 7261 6e73 666f 726d 6174 696f 6e73 2e0a  ransformations..
+00010a10: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00010a20: 7265 7373 696f 6e5f 6c65 7665 6c3a 204c  ression_level: L
+00010a30: 6576 656c 206f 6620 636f 6d70 7265 7373  evel of compress
+00010a40: 696f 6e20 666f 7220 6365 6c6c 7320 2862  ion for cells (b
+00010a50: 6574 7765 656e 2030 2061 6e64 2039 292e  etween 0 and 9).
+00010a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010a70: 2053 6574 7469 6e67 2074 6f20 3020 7769   Setting to 0 wi
+00010a80: 6c6c 2064 6973 6162 6c65 2063 656c 6c20  ll disable cell 
+00010a90: 636f 6d70 7265 7373 696f 6e2c 2031 2067  compression, 1 g
+00010aa0: 6976 6573 2074 6865 2062 6573 7420 7370  ives the best sp
+00010ab0: 6565 6420 616e 6420 392c 2074 6865 2062  eed and 9, the b
+00010ac0: 6573 7420 636f 6d70 7265 7373 696f 6e2e  est compression.
+00010ad0: 0a20 2020 2020 2020 2020 2020 2064 6574  .            det
+00010ae0: 6563 745f 7265 6374 616e 676c 6573 3a20  ect_rectangles: 
+00010af0: 5374 6f72 6520 7265 6374 616e 676c 6573  Store rectangles
+00010b00: 2069 6e20 636f 6d70 7265 7373 6564 2066   in compressed f
+00010b10: 6f72 6d61 742e 0a20 2020 2020 2020 2020  ormat..         
+00010b20: 2020 2064 6574 6563 745f 7472 6170 657a     detect_trapez
+00010b30: 6f69 6473 3a20 5374 6f72 6520 7472 6170  oids: Store trap
+00010b40: 657a 6f69 6473 2069 6e20 636f 6d70 7265  ezoids in compre
+00010b50: 7373 6564 2066 6f72 6d61 742e 0a20 2020  ssed format..   
+00010b60: 2020 2020 2020 2020 2063 6972 636c 655f           circle_
+00010b70: 746f 6c65 7261 6e63 653a 2054 6f6c 6572  tolerance: Toler
+00010b80: 616e 6365 2066 6f72 2064 6574 6563 7469  ance for detecti
+00010b90: 6e67 2063 6972 636c 6573 2e20 4966 206c  ng circles. If l
+00010ba0: 6573 7320 6f72 2065 7175 616c 2074 6f20  ess or equal to 
+00010bb0: 302c 206e 6f20 6465 7465 6374 696f 6e20  0, no detection 
+00010bc0: 6973 2070 6572 666f 726d 6564 2e0a 2020  is performed..  
+00010bd0: 2020 2020 2020 2020 2020 2020 2020 4369                Ci
+00010be0: 7263 6c65 7320 6172 6520 7374 6f72 6564  rcles are stored
+00010bf0: 2069 6e20 636f 6d70 7265 7373 6564 2066   in compressed f
+00010c00: 6f72 6d61 742e 0a20 2020 2020 2020 2020  ormat..         
+00010c10: 2020 2076 616c 6964 6174 696f 6e20 2822     validation ("
+00010c20: 6372 6333 3222 2c20 2263 6865 636b 7375  crc32", "checksu
+00010c30: 6d33 3222 2c20 4e6f 6e65 2920 e280 9320  m32", None) ... 
+00010c40: 7479 7065 206f 6620 7661 6c69 6461 7469  type of validati
+00010c50: 6f6e 2074 6f20 696e 636c 7564 6520 696e  on to include in
+00010c60: 2074 6865 2073 6176 6564 2066 696c 652e   the saved file.
+00010c70: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00010c80: 6e64 6172 645f 7072 6f70 6572 7469 6573  ndard_properties
+00010c90: 3a20 5374 6f72 6520 7374 616e 6461 7264  : Store standard
+00010ca0: 204f 4153 4953 2070 726f 7065 7274 6965   OASIS propertie
+00010cb0: 7320 696e 2074 6865 2066 696c 652e 0a20  s in the file.. 
+00010cc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010cd0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00010ce0: 7772 6974 655f 6c69 6272 6172 7928 0a20  write_library(. 
+00010cf0: 2020 2020 2020 2020 2020 2067 6473 7061             gdspa
+00010d00: 7468 3d67 6473 7061 7468 2c0a 2020 2020  th=gdspath,.    
+00010d10: 2020 2020 2020 2020 6764 7364 6972 3d67          gdsdir=g
+00010d20: 6473 6469 722c 0a20 2020 2020 2020 2020  dsdir,.         
+00010d30: 2020 2077 6974 685f 6f61 7369 733d 5472     with_oasis=Tr
+00010d40: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00010d50: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
+00010d60: 2020 290a 0a20 2020 2064 6566 2077 7269    )..    def wri
+00010d70: 7465 5f67 6473 5f77 6974 685f 6d65 7461  te_gds_with_meta
+00010d80: 6461 7461 2873 656c 662c 202a 6172 6773  data(self, *args
+00010d90: 2c20 2a2a 6b77 6172 6773 2920 2d3e 2050  , **kwargs) -> P
+00010da0: 6174 683a 0a20 2020 2020 2020 2022 2222  ath:.        """
+00010db0: 5772 6974 6520 636f 6d70 6f6e 656e 7420  Write component 
+00010dc0: 696e 2047 4453 2061 6e64 206d 6574 6164  in GDS and metad
+00010dd0: 6174 6120 2863 6f6d 706f 6e65 6e74 2073  ata (component s
+00010de0: 6574 7469 6e67 7329 2069 6e20 5941 4d4c  ettings) in YAML
+00010df0: 2e22 2222 0a20 2020 2020 2020 2067 6473  .""".        gds
+00010e00: 7061 7468 203d 2073 656c 662e 7772 6974  path = self.writ
+00010e10: 655f 6764 7328 2a61 7267 732c 202a 2a6b  e_gds(*args, **k
+00010e20: 7761 7267 7329 0a20 2020 2020 2020 206d  wargs).        m
+00010e30: 6574 6164 6174 6120 3d20 6764 7370 6174  etadata = gdspat
+00010e40: 682e 7769 7468 5f73 7566 6669 7828 222e  h.with_suffix(".
+00010e50: 796d 6c22 290a 2020 2020 2020 2020 6d65  yml").        me
+00010e60: 7461 6461 7461 2e77 7269 7465 5f74 6578  tadata.write_tex
+00010e70: 7428 7365 6c66 2e74 6f5f 7961 6d6c 2877  t(self.to_yaml(w
+00010e80: 6974 685f 6365 6c6c 733d 5472 7565 2c20  ith_cells=True, 
+00010e90: 7769 7468 5f70 6f72 7473 3d54 7275 6529  with_ports=True)
+00010ea0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+00010eb0: 2e69 6e66 6f28 6622 5772 6974 6520 5941  .info(f"Write YA
+00010ec0: 4d4c 206d 6574 6164 6174 6120 746f 207b  ML metadata to {
+00010ed0: 7374 7228 6d65 7461 6461 7461 2921 727d  str(metadata)!r}
+00010ee0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00010ef0: 6e20 6764 7370 6174 680a 0a20 2020 2064  n gdspath..    d
+00010f00: 6566 2074 6f5f 6469 6374 280a 2020 2020  ef to_dict(.    
+00010f10: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00010f20: 2020 6967 6e6f 7265 5f63 6f6d 706f 6e65    ignore_compone
+00010f30: 6e74 735f 7072 6566 6978 3a20 4f70 7469  nts_prefix: Opti
+00010f40: 6f6e 616c 5b4c 6973 745b 7374 725d 5d20  onal[List[str]] 
+00010f50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00010f60: 6967 6e6f 7265 5f66 756e 6374 696f 6e73  ignore_functions
+00010f70: 5f70 7265 6669 783a 204f 7074 696f 6e61  _prefix: Optiona
+00010f80: 6c5b 4c69 7374 5b73 7472 5d5d 203d 204e  l[List[str]] = N
+00010f90: 6f6e 652c 0a20 2020 2020 2020 2077 6974  one,.        wit
+00010fa0: 685f 6365 6c6c 733a 2062 6f6f 6c20 3d20  h_cells: bool = 
+00010fb0: 4661 6c73 652c 0a20 2020 2020 2020 2077  False,.        w
+00010fc0: 6974 685f 706f 7274 733a 2062 6f6f 6c20  ith_ports: bool 
+00010fd0: 3d20 5472 7565 2c0a 2020 2020 2920 2d3e  = True,.    ) ->
+00010fe0: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
+00010ff0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00011000: 726e 7320 4469 6374 2072 6570 7265 7365  rns Dict represe
+00011010: 6e74 6174 696f 6e20 6f66 2061 2063 6f6d  ntation of a com
+00011020: 706f 6e65 6e74 2e0a 0a20 2020 2020 2020  ponent...       
+00011030: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00011040: 2020 2069 676e 6f72 655f 636f 6d70 6f6e     ignore_compon
+00011050: 656e 7473 5f70 7265 6669 783a 2066 6f72  ents_prefix: for
+00011060: 2063 6f6d 706f 6e65 6e74 7320 746f 2069   components to i
+00011070: 676e 6f72 6520 7768 656e 2065 7870 6f72  gnore when expor
+00011080: 7469 6e67 2e0a 2020 2020 2020 2020 2020  ting..          
+00011090: 2020 6967 6e6f 7265 5f66 756e 6374 696f    ignore_functio
+000110a0: 6e73 5f70 7265 6669 783a 2066 6f72 2066  ns_prefix: for f
+000110b0: 756e 6374 696f 6e73 2074 6f20 6967 6e6f  unctions to igno
+000110c0: 7265 2077 6865 6e20 6578 706f 7274 696e  re when exportin
+000110d0: 672e 0a20 2020 2020 2020 2020 2020 2077  g..            w
+000110e0: 6974 685f 6365 6c6c 733a 2077 7269 7465  ith_cells: write
+000110f0: 2063 656c 6c73 2072 6563 7572 7369 7665   cells recursive
+00011100: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
+00011110: 7769 7468 5f70 6f72 7473 3a20 7772 6974  with_ports: writ
+00011120: 6520 706f 7274 2069 6e66 6f72 6d61 7469  e port informati
+00011130: 6f6e 2064 6963 742e 0a20 2020 2020 2020  on dict..       
+00011140: 2022 2222 0a20 2020 2020 2020 2064 203d   """.        d =
+00011150: 207b 7d0a 2020 2020 2020 2020 6966 2077   {}.        if w
+00011160: 6974 685f 706f 7274 733a 0a20 2020 2020  ith_ports:.     
+00011170: 2020 2020 2020 2070 6f72 7473 203d 207b         ports = {
+00011180: 706f 7274 2e6e 616d 653a 2070 6f72 742e  port.name: port.
+00011190: 746f 5f64 6963 7428 2920 666f 7220 706f  to_dict() for po
+000111a0: 7274 2069 6e20 7365 6c66 2e67 6574 5f70  rt in self.get_p
+000111b0: 6f72 7473 5f6c 6973 7428 297d 0a20 2020  orts_list()}.   
+000111c0: 2020 2020 2020 2020 2064 5b22 706f 7274           d["port
+000111d0: 7322 5d20 3d20 706f 7274 730a 0a20 2020  s"] = ports..   
+000111e0: 2020 2020 2069 6620 7769 7468 5f63 656c       if with_cel
+000111f0: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+00011200: 6365 6c6c 7320 3d20 7265 6375 7273 655f  cells = recurse_
+00011210: 7374 7275 6374 7572 6573 280a 2020 2020  structures(.    
+00011220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011240: 2020 6967 6e6f 7265 5f66 756e 6374 696f    ignore_functio
+00011250: 6e73 5f70 7265 6669 783d 6967 6e6f 7265  ns_prefix=ignore
+00011260: 5f66 756e 6374 696f 6e73 5f70 7265 6669  _functions_prefi
+00011270: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
+00011280: 2020 2069 676e 6f72 655f 636f 6d70 6f6e     ignore_compon
+00011290: 656e 7473 5f70 7265 6669 783d 6967 6e6f  ents_prefix=igno
+000112a0: 7265 5f63 6f6d 706f 6e65 6e74 735f 7072  re_components_pr
+000112b0: 6566 6978 2c0a 2020 2020 2020 2020 2020  efix,.          
+000112c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000112d0: 645b 2263 656c 6c73 225d 203d 2063 6c65  d["cells"] = cle
+000112e0: 616e 5f64 6963 7428 6365 6c6c 7329 0a0a  an_dict(cells)..
+000112f0: 2020 2020 2020 2020 645b 226e 616d 6522          d["name"
+00011300: 5d20 3d20 7365 6c66 2e6e 616d 650a 2020  ] = self.name.  
+00011310: 2020 2020 2020 645b 2273 6574 7469 6e67        d["setting
+00011320: 7322 5d20 3d20 636c 6561 6e5f 6469 6374  s"] = clean_dict
+00011330: 2864 6963 7428 7365 6c66 2e73 6574 7469  (dict(self.setti
+00011340: 6e67 7329 290a 2020 2020 2020 2020 7265  ngs)).        re
+00011350: 7475 726e 2064 0a0a 2020 2020 6465 6620  turn d..    def 
+00011360: 746f 5f79 616d 6c28 7365 6c66 2c20 2a2a  to_yaml(self, **
+00011370: 6b77 6172 6773 2920 2d3e 2073 7472 3a0a  kwargs) -> str:.
+00011380: 2020 2020 2020 2020 2222 2257 7269 7465          """Write
+00011390: 2044 6963 7420 7265 7072 6573 656e 7461   Dict representa
+000113a0: 7469 6f6e 206f 6620 6120 636f 6d70 6f6e  tion of a compon
+000113b0: 656e 7420 696e 2059 414d 4c20 666f 726d  ent in YAML form
+000113c0: 6174 2e0a 0a20 2020 2020 2020 2041 7267  at...        Arg
+000113d0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+000113e0: 676e 6f72 655f 636f 6d70 6f6e 656e 7473  gnore_components
+000113f0: 5f70 7265 6669 783a 2066 6f72 2063 6f6d  _prefix: for com
+00011400: 706f 6e65 6e74 7320 746f 2069 676e 6f72  ponents to ignor
+00011410: 6520 7768 656e 2065 7870 6f72 7469 6e67  e when exporting
+00011420: 2e0a 2020 2020 2020 2020 2020 2020 6967  ..            ig
+00011430: 6e6f 7265 5f66 756e 6374 696f 6e73 5f70  nore_functions_p
+00011440: 7265 6669 783a 2066 6f72 2066 756e 6374  refix: for funct
+00011450: 696f 6e73 2074 6f20 6967 6e6f 7265 2077  ions to ignore w
+00011460: 6865 6e20 6578 706f 7274 696e 672e 0a20  hen exporting.. 
+00011470: 2020 2020 2020 2020 2020 2077 6974 685f             with_
+00011480: 6365 6c6c 733a 2077 7269 7465 2063 656c  cells: write cel
+00011490: 6c73 2072 6563 7572 7369 7665 6c79 2e0a  ls recursively..
+000114a0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+000114b0: 5f70 6f72 7473 3a20 7772 6974 6520 706f  _ports: write po
+000114c0: 7274 2069 6e66 6f72 6d61 7469 6f6e 2e0a  rt information..
+000114d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000114e0: 2020 2020 7265 7475 726e 204f 6d65 6761      return Omega
+000114f0: 436f 6e66 2e74 6f5f 7961 6d6c 2863 6c65  Conf.to_yaml(cle
+00011500: 616e 5f64 6963 7428 7365 6c66 2e74 6f5f  an_dict(self.to_
+00011510: 6469 6374 282a 2a6b 7761 7267 7329 2929  dict(**kwargs)))
+00011520: 0a0a 2020 2020 6465 6620 746f 5f64 6963  ..    def to_dic
+00011530: 745f 706f 6c79 676f 6e73 2873 656c 6629  t_polygons(self)
+00011540: 202d 3e20 4469 6374 5b73 7472 2c20 416e   -> Dict[str, An
+00011550: 795d 3a0a 2020 2020 2020 2020 2222 2252  y]:.        """R
+00011560: 6574 7572 6e73 2061 2064 6963 7420 7265  eturns a dict re
+00011570: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
+00011580: 7468 6520 666c 6174 7465 6e65 6420 636f  the flattened co
+00011590: 6d70 6f6e 656e 742e 2222 220a 2020 2020  mponent.""".    
+000115a0: 2020 2020 6420 3d20 7b7d 0a20 2020 2020      d = {}.     
+000115b0: 2020 2070 6f6c 7967 6f6e 7320 3d20 7b7d     polygons = {}
+000115c0: 0a20 2020 2020 2020 206c 6179 6572 5f74  .        layer_t
+000115d0: 6f5f 706f 6c79 676f 6e73 203d 2073 656c  o_polygons = sel
+000115e0: 662e 6765 745f 706f 6c79 676f 6e73 2862  f.get_polygons(b
+000115f0: 795f 7370 6563 3d54 7275 6529 0a0a 2020  y_spec=True)..  
+00011600: 2020 2020 2020 666f 7220 6c61 7965 722c        for layer,
+00011610: 2070 6f6c 7967 6f6e 735f 6c61 7965 7220   polygons_layer 
+00011620: 696e 206c 6179 6572 5f74 6f5f 706f 6c79  in layer_to_poly
+00011630: 676f 6e73 2e69 7465 6d73 2829 3a0a 2020  gons.items():.  
+00011640: 2020 2020 2020 2020 2020 6c61 7965 725f            layer_
+00011650: 6e61 6d65 203d 2066 227b 6c61 7965 725b  name = f"{layer[
+00011660: 305d 7d5f 7b6c 6179 6572 5b31 5d7d 220a  0]}_{layer[1]}".
+00011670: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00011680: 706f 6c79 676f 6e20 696e 2070 6f6c 7967  polygon in polyg
+00011690: 6f6e 735f 6c61 7965 723a 0a20 2020 2020  ons_layer:.     
+000116a0: 2020 2020 2020 2020 2020 2070 6f6c 7967             polyg
+000116b0: 6f6e 735b 6c61 7965 725f 6e61 6d65 5d20  ons[layer_name] 
+000116c0: 3d20 5b74 7570 6c65 2873 6e61 705f 746f  = [tuple(snap_to
+000116d0: 5f67 7269 6428 7629 2920 666f 7220 7620  _grid(v)) for v 
+000116e0: 696e 2070 6f6c 7967 6f6e 5d0a 0a20 2020  in polygon]..   
+000116f0: 2020 2020 2070 6f72 7473 203d 207b 706f       ports = {po
+00011700: 7274 2e6e 616d 653a 2070 6f72 742e 7365  rt.name: port.se
+00011710: 7474 696e 6773 2066 6f72 2070 6f72 7420  ttings for port 
+00011720: 696e 2073 656c 662e 6765 745f 706f 7274  in self.get_port
+00011730: 735f 6c69 7374 2829 7d0a 2020 2020 2020  s_list()}.      
+00011740: 2020 636c 6561 6e5f 6469 6374 2870 6f72    clean_dict(por
+00011750: 7473 290a 2020 2020 2020 2020 636c 6561  ts).        clea
+00011760: 6e5f 6469 6374 2870 6f6c 7967 6f6e 7329  n_dict(polygons)
+00011770: 0a20 2020 2020 2020 2064 2e69 6e66 6f20  .        d.info 
+00011780: 3d20 7365 6c66 2e69 6e66 6f0a 2020 2020  = self.info.    
+00011790: 2020 2020 642e 706f 6c79 676f 6e73 203d      d.polygons =
+000117a0: 2070 6f6c 7967 6f6e 730a 2020 2020 2020   polygons.      
+000117b0: 2020 642e 706f 7274 7320 3d20 706f 7274    d.ports = port
+000117c0: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+000117d0: 2064 0a0a 2020 2020 6465 6620 6175 746f   d..    def auto
+000117e0: 5f72 656e 616d 655f 706f 7274 7328 7365  _rename_ports(se
+000117f0: 6c66 2c20 2a2a 6b77 6172 6773 2920 2d3e  lf, **kwargs) ->
+00011800: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00011810: 2222 5265 6e61 6d65 2070 6f72 7473 2062  ""Rename ports b
+00011820: 7920 6f72 6965 6e74 6174 696f 6e20 4e53  y orientation NS
+00011830: 4557 2028 6e6f 7274 682c 2073 6f75 7468  EW (north, south
+00011840: 2c20 6561 7374 2c20 7765 7374 292e 0a0a  , east, west)...
+00011850: 2020 2020 2020 2020 4b65 7977 6f72 6420          Keyword 
+00011860: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00011870: 2020 6675 6e63 7469 6f6e 3a20 746f 2072    function: to r
+00011880: 656e 616d 6520 706f 7274 732e 0a20 2020  ename ports..   
+00011890: 2020 2020 2020 2020 2073 656c 6563 745f           select_
+000118a0: 706f 7274 735f 6f70 7469 6361 6c3a 2074  ports_optical: t
+000118b0: 6f20 7365 6c65 6374 206f 7074 6963 616c  o select optical
+000118c0: 2070 6f72 7473 2e0a 2020 2020 2020 2020   ports..        
+000118d0: 2020 2020 7365 6c65 6374 5f70 6f72 7473      select_ports
+000118e0: 5f65 6c65 6374 7269 6361 6c3a 2074 6f20  _electrical: to 
+000118f0: 7365 6c65 6374 2065 6c65 6374 7269 6361  select electrica
+00011900: 6c20 706f 7274 732e 0a20 2020 2020 2020  l ports..       
+00011910: 2020 2020 2070 7265 6669 785f 6f70 7469       prefix_opti
+00011920: 6361 6c3a 2070 7265 6669 782e 0a20 2020  cal: prefix..   
+00011930: 2020 2020 2020 2020 2070 7265 6669 785f           prefix_
+00011940: 656c 6563 7472 6963 616c 3a20 7072 6566  electrical: pref
+00011950: 6978 2e0a 0a20 2020 2020 2020 202e 2e20  ix...        .. 
+00011960: 636f 6465 3a3a 0a0a 2020 2020 2020 2020  code::..        
+00011970: 2020 2020 2020 2020 2020 3320 2034 0a20            3  4. 
+00011980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011990: 5f7c 5f5f 7c5f 0a20 2020 2020 2020 2020  _|__|_.         
+000119a0: 2020 2020 3220 2d7c 2020 2020 2020 7c2d      2 -|      |-
+000119b0: 2035 0a20 2020 2020 2020 2020 2020 2020   5.             
+000119c0: 2020 207c 2020 2020 2020 7c0a 2020 2020     |      |.    
+000119d0: 2020 2020 2020 2020 2031 202d 7c5f 5f5f           1 -|___
+000119e0: 5f5f 5f7c 2d20 360a 2020 2020 2020 2020  ___|- 6.        
+000119f0: 2020 2020 2020 2020 2020 7c20 207c 0a20            |  |. 
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a10: 2038 2020 370a 2020 2020 2020 2020 2222   8  7.        ""
+00011a20: 220a 2020 2020 2020 2020 7365 6c66 2e69  ".        self.i
+00011a30: 735f 756e 6c6f 636b 6564 2829 0a20 2020  s_unlocked().   
+00011a40: 2020 2020 2061 7574 6f5f 7265 6e61 6d65       auto_rename
+00011a50: 5f70 6f72 7473 2873 656c 662c 202a 2a6b  _ports(self, **k
+00011a60: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
+00011a70: 6175 746f 5f72 656e 616d 655f 706f 7274  auto_rename_port
+00011a80: 735f 636f 756e 7465 725f 636c 6f63 6b77  s_counter_clockw
+00011a90: 6973 6528 7365 6c66 2c20 2a2a 6b77 6172  ise(self, **kwar
+00011aa0: 6773 2920 2d3e 204e 6f6e 653a 0a20 2020  gs) -> None:.   
+00011ab0: 2020 2020 2073 656c 662e 6973 5f75 6e6c       self.is_unl
+00011ac0: 6f63 6b65 6428 290a 2020 2020 2020 2020  ocked().        
+00011ad0: 6175 746f 5f72 656e 616d 655f 706f 7274  auto_rename_port
+00011ae0: 735f 636f 756e 7465 725f 636c 6f63 6b77  s_counter_clockw
+00011af0: 6973 6528 7365 6c66 2c20 2a2a 6b77 6172  ise(self, **kwar
+00011b00: 6773 290a 0a20 2020 2064 6566 2061 7574  gs)..    def aut
+00011b10: 6f5f 7265 6e61 6d65 5f70 6f72 7473 5f6c  o_rename_ports_l
+00011b20: 6179 6572 5f6f 7269 656e 7461 7469 6f6e  ayer_orientation
+00011b30: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
+00011b40: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00011b50: 2020 7365 6c66 2e69 735f 756e 6c6f 636b    self.is_unlock
+00011b60: 6564 2829 0a20 2020 2020 2020 2061 7574  ed().        aut
+00011b70: 6f5f 7265 6e61 6d65 5f70 6f72 7473 5f6c  o_rename_ports_l
+00011b80: 6179 6572 5f6f 7269 656e 7461 7469 6f6e  ayer_orientation
+00011b90: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
+00011ba0: 0a0a 2020 2020 6465 6620 6175 746f 5f72  ..    def auto_r
+00011bb0: 656e 616d 655f 706f 7274 735f 6f72 6965  ename_ports_orie
+00011bc0: 6e74 6174 696f 6e28 7365 6c66 2c20 2a2a  ntation(self, **
+00011bd0: 6b77 6172 6773 2920 2d3e 204e 6f6e 653a  kwargs) -> None:
+00011be0: 0a20 2020 2020 2020 2022 2222 5265 6e61  .        """Rena
+00011bf0: 6d65 2070 6f72 7473 2062 7920 6f72 6965  me ports by orie
+00011c00: 6e74 6174 696f 6e20 4e53 4557 2028 6e6f  ntation NSEW (no
+00011c10: 7274 682c 2073 6f75 7468 2c20 6561 7374  rth, south, east
+00011c20: 2c20 7765 7374 292e 0a0a 2020 2020 2020  , west)...      
+00011c30: 2020 4b65 7977 6f72 6420 4172 6773 3a0a    Keyword Args:.
+00011c40: 2020 2020 2020 2020 2020 2020 6675 6e63              func
+00011c50: 7469 6f6e 3a20 746f 2072 656e 616d 6520  tion: to rename 
+00011c60: 706f 7274 732e 0a20 2020 2020 2020 2020  ports..         
+00011c70: 2020 2073 656c 6563 745f 706f 7274 735f     select_ports_
+00011c80: 6f70 7469 6361 6c3a 2074 6f20 7365 6c65  optical: to sele
+00011c90: 6374 2070 6f72 7473 2e0a 2020 2020 2020  ct ports..      
+00011ca0: 2020 2020 2020 7365 6c65 6374 5f70 6f72        select_por
+00011cb0: 7473 5f65 6c65 6374 7269 6361 6c3a 0a20  ts_electrical:. 
+00011cc0: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00011cd0: 785f 6f70 7469 6361 6c3a 0a20 2020 2020  x_optical:.     
+00011ce0: 2020 2020 2020 2070 7265 6669 785f 656c         prefix_el
+00011cf0: 6563 7472 6963 616c 3a0a 0a20 2020 2020  ectrical:..     
+00011d00: 2020 202e 2e20 636f 6465 3a3a 0a0a 2020     .. code::..  
+00011d10: 2020 2020 2020 2020 2020 2020 2020 204e                 N
+00011d20: 3020 204e 310a 2020 2020 2020 2020 2020  0  N1.          
+00011d30: 2020 2020 2020 207c 5f5f 5f7c 5f0a 2020         |___|_.  
+00011d40: 2020 2020 2020 2020 2020 5731 202d 7c20            W1 -| 
+00011d50: 2020 2020 207c 2d20 4531 0a20 2020 2020       |- E1.     
+00011d60: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00011d70: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
+00011d80: 5730 202d 7c5f 5f5f 5f5f 5f7c 2d20 4530  W0 -|______|- E0
+00011d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011da0: 2020 7c20 2020 7c0a 2020 2020 2020 2020    |   |.        
+00011db0: 2020 2020 2020 2020 5330 2020 2053 310a          S0   S1.
+00011dc0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011dd0: 2020 2020 7365 6c66 2e69 735f 756e 6c6f      self.is_unlo
+00011de0: 636b 6564 2829 0a20 2020 2020 2020 2061  cked().        a
+00011df0: 7574 6f5f 7265 6e61 6d65 5f70 6f72 7473  uto_rename_ports
+00011e00: 5f6f 7269 656e 7461 7469 6f6e 2873 656c  _orientation(sel
+00011e10: 662c 202a 2a6b 7761 7267 7329 0a0a 2020  f, **kwargs)..  
+00011e20: 2020 6465 6620 6d6f 7665 280a 2020 2020    def move(.    
+00011e30: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00011e40: 2020 6f72 6967 696e 3a20 466c 6f61 7432    origin: Float2
+00011e50: 203d 2028 302c 2030 292c 0a20 2020 2020   = (0, 0),.     
+00011e60: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
+00011e70: 4f70 7469 6f6e 616c 5b46 6c6f 6174 325d  Optional[Float2]
+00011e80: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00011e90: 2061 7869 733a 204f 7074 696f 6e61 6c5b   axis: Optional[
+00011ea0: 4178 6973 5d20 3d20 4e6f 6e65 2c0a 2020  Axis] = None,.  
+00011eb0: 2020 2920 2d3e 2043 6f6d 706f 6e65 6e74    ) -> Component
+00011ec0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+00011ed0: 7572 6e73 206e 6577 2043 6f6d 706f 6e65  urns new Compone
+00011ee0: 6e74 2077 6974 6820 6120 6d6f 7665 6420  nt with a moved 
+00011ef0: 7265 6665 7265 6e63 6520 746f 2074 6865  reference to the
+00011f00: 206f 7269 6769 6e61 6c2e 0a0a 2020 2020   original...    
+00011f10: 2020 2020 636f 6d70 6f6e 656e 742e 0a0a      component...
+00011f20: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00011f30: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
+00011f40: 3a20 6f66 2063 6f6d 706f 6e65 6e74 2e0a  : of component..
+00011f50: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00011f60: 696e 6174 696f 6e3a 2078 2c20 792e 0a20  ination: x, y.. 
+00011f70: 2020 2020 2020 2020 2020 2061 7869 733a             axis:
+00011f80: 2078 206f 7220 792e 0a20 2020 2020 2020   x or y..       
+00011f90: 2022 2222 0a20 2020 2020 2020 2072 6169   """.        rai
+00011fa0: 7365 2056 616c 7565 4572 726f 7228 6d6f  se ValueError(mo
+00011fb0: 7665 5f65 7272 6f72 5f6d 6573 7361 6765  ve_error_message
+00011fc0: 290a 0a20 2020 2064 6566 206d 6972 726f  )..    def mirro
+00011fd0: 7228 7365 6c66 2c20 7031 3a20 466c 6f61  r(self, p1: Floa
+00011fe0: 7432 203d 2028 302c 2031 292c 2070 323a  t2 = (0, 1), p2:
+00011ff0: 2046 6c6f 6174 3220 3d20 2830 2c20 3029   Float2 = (0, 0)
+00012000: 2c20 2a2a 6b77 6172 6773 2920 2d3e 2043  , **kwargs) -> C
+00012010: 6f6d 706f 6e65 6e74 3a0a 2020 2020 2020  omponent:.      
+00012020: 2020 2222 2252 6574 7572 6e73 206e 6577    """Returns new
+00012030: 2043 6f6d 706f 6e65 6e74 2077 6974 6820   Component with 
+00012040: 6120 6d69 7272 6f72 6564 2072 6566 6572  a mirrored refer
+00012050: 656e 6365 2e0a 0a20 2020 2020 2020 2041  ence...        A
+00012060: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00012070: 2070 313a 2066 6972 7374 2070 6f69 6e74   p1: first point
+00012080: 2074 6f20 6465 6669 6e65 206d 6972 726f   to define mirro
+00012090: 7220 6178 6973 2e0a 2020 2020 2020 2020  r axis..        
+000120a0: 2020 2020 7032 3a20 7365 636f 6e64 2070      p2: second p
+000120b0: 6f69 6e74 2074 6f20 6465 6669 6e65 206d  oint to define m
+000120c0: 6972 726f 7220 6178 6973 2e0a 2020 2020  irror axis..    
+000120d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000120e0: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
+000120f0: 6675 6e63 7469 6f6e 7320 696d 706f 7274  functions import
+00012100: 206d 6972 726f 720a 0a20 2020 2020 2020   mirror..       
+00012110: 2072 6574 7572 6e20 6d69 7272 6f72 2863   return mirror(c
+00012120: 6f6d 706f 6e65 6e74 3d73 656c 662c 2070  omponent=self, p
+00012130: 313d 7031 2c20 7032 3d70 322c 202a 2a6b  1=p1, p2=p2, **k
+00012140: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
+00012150: 726f 7461 7465 2873 656c 662c 2061 6e67  rotate(self, ang
+00012160: 6c65 3a20 666c 6f61 7420 3d20 3930 2c20  le: float = 90, 
+00012170: 2a2a 6b77 6172 6773 2920 2d3e 2043 6f6d  **kwargs) -> Com
+00012180: 706f 6e65 6e74 3a0a 2020 2020 2020 2020  ponent:.        
+00012190: 2222 2252 6574 7572 6e73 206e 6577 2063  """Returns new c
+000121a0: 6f6d 706f 6e65 6e74 2077 6974 6820 6120  omponent with a 
+000121b0: 726f 7461 7465 6420 7265 6665 7265 6e63  rotated referenc
+000121c0: 6520 746f 2074 6865 206f 7269 6769 6e61  e to the origina
+000121d0: 6c2e 0a0a 2020 2020 2020 2020 4172 6773  l...        Args
+000121e0: 3a0a 2020 2020 2020 2020 2020 2020 616e  :.            an
+000121f0: 676c 653a 2069 6e20 6465 6772 6565 732e  gle: in degrees.
+00012200: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012210: 2020 2020 2066 726f 6d20 6764 7366 6163       from gdsfac
+00012220: 746f 7279 2e66 756e 6374 696f 6e73 2069  tory.functions i
+00012230: 6d70 6f72 7420 726f 7461 7465 0a0a 2020  mport rotate..  
+00012240: 2020 2020 2020 7265 7475 726e 2072 6f74        return rot
+00012250: 6174 6528 636f 6d70 6f6e 656e 743d 7365  ate(component=se
+00012260: 6c66 2c20 616e 676c 653d 616e 676c 652c  lf, angle=angle,
+00012270: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
+00012280: 6465 6620 6164 645f 7061 6464 696e 6728  def add_padding(
+00012290: 7365 6c66 2c20 2a2a 6b77 6172 6773 2920  self, **kwargs) 
+000122a0: 2d3e 2043 6f6d 706f 6e65 6e74 3a0a 2020  -> Component:.  
+000122b0: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
+000122c0: 2073 616d 6520 636f 6d70 6f6e 656e 7420   same component 
+000122d0: 7769 7468 2070 6164 6469 6e67 2e0a 0a20  with padding... 
+000122e0: 2020 2020 2020 204b 6579 776f 7264 2041         Keyword A
+000122f0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00012300: 2063 6f6d 706f 6e65 6e74 3a20 666f 7220   component: for 
+00012310: 7061 6464 696e 672e 0a20 2020 2020 2020  padding..       
+00012320: 2020 2020 206c 6179 6572 733a 206c 6973       layers: lis
+00012330: 7420 6f66 206c 6179 6572 732e 0a20 2020  t of layers..   
+00012340: 2020 2020 2020 2020 2073 7566 6669 7820           suffix 
+00012350: 666f 7220 6e61 6d65 2e0a 2020 2020 2020  for name..      
+00012360: 2020 2020 2020 6465 6661 756c 743a 2064        default: d
+00012370: 6566 6175 6c74 2070 6164 6469 6e67 2028  efault padding (
+00012380: 3530 756d 292e 0a20 2020 2020 2020 2020  50um)..         
+00012390: 2020 2074 6f70 3a20 6e6f 7274 6820 7061     top: north pa
+000123a0: 6464 696e 672e 0a20 2020 2020 2020 2020  dding..         
+000123b0: 2020 2062 6f74 746f 6d3a 2073 6f75 7468     bottom: south
+000123c0: 2070 6164 6469 6e67 2e0a 2020 2020 2020   padding..      
+000123d0: 2020 2020 2020 7269 6768 743a 2065 6173        right: eas
+000123e0: 7420 7061 6464 696e 672e 0a20 2020 2020  t padding..     
+000123f0: 2020 2020 2020 206c 6566 743a 2077 6573         left: wes
+00012400: 7420 7061 6464 696e 672e 0a20 2020 2020  t padding..     
+00012410: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
+00012420: 726f 6d20 6764 7366 6163 746f 7279 2e61  rom gdsfactory.a
+00012430: 6464 5f70 6164 6469 6e67 2069 6d70 6f72  dd_padding impor
+00012440: 7420 6164 645f 7061 6464 696e 670a 0a20  t add_padding.. 
+00012450: 2020 2020 2020 2072 6574 7572 6e20 6164         return ad
+00012460: 645f 7061 6464 696e 6728 636f 6d70 6f6e  d_padding(compon
+00012470: 656e 743d 7365 6c66 2c20 2a2a 6b77 6172  ent=self, **kwar
+00012480: 6773 290a 0a20 2020 2064 6566 2061 6273  gs)..    def abs
+00012490: 6f72 6228 7365 6c66 2c20 7265 6665 7265  orb(self, refere
+000124a0: 6e63 6529 202d 3e20 436f 6d70 6f6e 656e  nce) -> Componen
+000124b0: 743a 0a20 2020 2020 2020 2022 2222 4162  t:.        """Ab
+000124c0: 736f 7262 7320 706f 6c79 676f 6e73 2066  sorbs polygons f
+000124d0: 726f 6d20 436f 6d70 6f6e 656e 7452 6566  rom ComponentRef
+000124e0: 6572 656e 6365 2069 6e74 6f20 436f 6d70  erence into Comp
+000124f0: 6f6e 656e 742e 0a0a 2020 2020 2020 2020  onent...        
+00012500: 4465 7374 726f 7973 2074 6865 2072 6566  Destroys the ref
+00012510: 6572 656e 6365 2069 6e20 7468 6520 7072  erence in the pr
+00012520: 6f63 6573 7320 6275 7420 6b65 6570 696e  ocess but keepin
+00012530: 6720 7468 6520 706f 6c79 676f 6e20 6765  g the polygon ge
+00012540: 6f6d 6574 7279 2e0a 0a20 2020 2020 2020  ometry...       
+00012550: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00012560: 2020 2072 6566 6572 656e 6365 3a20 436f     reference: Co
+00012570: 6d70 6f6e 656e 7452 6566 6572 656e 6365  mponentReference
+00012580: 2074 6f20 6265 2061 6273 6f72 6265 6420   to be absorbed 
+00012590: 696e 746f 2074 6865 2043 6f6d 706f 6e65  into the Compone
+000125a0: 6e74 2e0a 2020 2020 2020 2020 2222 220a  nt..        """.
+000125b0: 2020 2020 2020 2020 6966 2072 6566 6572          if refer
+000125c0: 656e 6365 206e 6f74 2069 6e20 7365 6c66  ence not in self
+000125d0: 2e72 6566 6572 656e 6365 733a 0a20 2020  .references:.   
+000125e0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000125f0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+00012600: 2020 2020 2020 2020 2020 2022 5468 6520             "The 
+00012610: 7265 6665 7265 6e63 6520 796f 7520 6173  reference you as
+00012620: 6b65 6420 746f 2061 6273 6f72 6220 646f  ked to absorb do
+00012630: 6573 206e 6f74 2065 7869 7374 2069 6e20  es not exist in 
+00012640: 7468 6973 2043 6f6d 706f 6e65 6e74 2e22  this Component."
+00012650: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00012660: 2020 2020 2020 2072 6566 5f70 6f6c 7967         ref_polyg
+00012670: 6f6e 7320 3d20 7265 6665 7265 6e63 652e  ons = reference.
+00012680: 6765 745f 706f 6c79 676f 6e73 280a 2020  get_polygons(.  
+00012690: 2020 2020 2020 2020 2020 6279 5f73 7065            by_spe
+000126a0: 633d 4661 6c73 652c 2069 6e63 6c75 6465  c=False, include
+000126b0: 5f70 6174 6873 3d46 616c 7365 2c20 6173  _paths=False, as
+000126c0: 5f61 7272 6179 3d46 616c 7365 0a20 2020  _array=False.   
+000126d0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+000126e0: 656c 662e 5f61 6464 5f70 6f6c 7967 6f6e  elf._add_polygon
+000126f0: 7328 2a72 6566 5f70 6f6c 7967 6f6e 7329  s(*ref_polygons)
+00012700: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00012710: 6464 2872 6566 6572 656e 6365 2e67 6574  dd(reference.get
+00012720: 5f6c 6162 656c 7328 2929 0a20 2020 2020  _labels()).     
+00012730: 2020 2073 656c 662e 6164 6428 7265 6665     self.add(refe
+00012740: 7265 6e63 652e 6765 745f 7061 7468 7328  rence.get_paths(
+00012750: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00012760: 7265 6d6f 7665 2872 6566 6572 656e 6365  remove(reference
+00012770: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00012780: 2073 656c 660a 0a20 2020 2064 6566 2072   self..    def r
+00012790: 656d 6f76 6528 7365 6c66 2c20 6974 656d  emove(self, item
+000127a0: 7329 3a0a 2020 2020 2020 2020 2222 2252  s):.        """R
+000127b0: 656d 6f76 6573 2069 7465 6d73 2066 726f  emoves items fro
+000127c0: 6d20 6120 436f 6d70 6f6e 656e 742c 2077  m a Component, w
+000127d0: 6869 6368 2063 616e 2069 6e63 6c75 6465  hich can include
+000127e0: 2050 6f72 7473 2c20 506f 6c79 676f 6e53   Ports, PolygonS
+000127f0: 6574 7320 5c0a 2020 2020 2020 2020 4365  ets \.        Ce
+00012800: 6c6c 5265 6665 7265 6e63 6573 2c20 436f  llReferences, Co
+00012810: 6d70 6f6e 656e 7452 6566 6572 656e 6365  mponentReference
+00012820: 7320 616e 6420 4c61 6265 6c73 2e0a 0a20  s and Labels... 
+00012830: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00012840: 2020 2020 2020 2020 2069 7465 6d73 3a20           items: 
+00012850: 6c69 7374 206f 6620 4974 656d 7320 746f  list of Items to
+00012860: 2062 6520 7265 6d6f 7665 6420 6672 6f6d   be removed from
+00012870: 2074 6865 2043 6f6d 706f 6e65 6e74 2e0a   the Component..
+00012880: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012890: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
+000128a0: 7472 2869 7465 6d73 2c20 225f 5f69 7465  tr(items, "__ite
+000128b0: 725f 5f22 293a 0a20 2020 2020 2020 2020  r__"):.         
+000128c0: 2020 2069 7465 6d73 203d 205b 6974 656d     items = [item
+000128d0: 735d 0a20 2020 2020 2020 2066 6f72 2069  s].        for i
+000128e0: 7465 6d20 696e 2069 7465 6d73 3a0a 2020  tem in items:.  
+000128f0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00012900: 6e73 7461 6e63 6528 6974 656d 2c20 506f  nstance(item, Po
+00012910: 7274 293a 0a20 2020 2020 2020 2020 2020  rt):.           
+00012920: 2020 2020 2073 656c 662e 706f 7274 7320       self.ports 
+00012930: 3d20 7b6b 3a20 7620 666f 7220 6b2c 2076  = {k: v for k, v
+00012940: 2069 6e20 7365 6c66 2e70 6f72 7473 2e69   in self.ports.i
+00012950: 7465 6d73 2829 2069 6620 7620 213d 2069  tems() if v != i
+00012960: 7465 6d7d 0a20 2020 2020 2020 2020 2020  tem}.           
+00012970: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00012980: 2869 7465 6d2c 2067 6473 746b 2e52 6566  (item, gdstk.Ref
+00012990: 6572 656e 6365 293a 0a20 2020 2020 2020  erence):.       
+000129a0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+000129b0: 656c 6c2e 7265 6d6f 7665 2869 7465 6d29  ell.remove(item)
+000129c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000129d0: 2069 7465 6d2e 6f77 6e65 7220 3d20 4e6f   item.owner = No
+000129e0: 6e65 0a20 2020 2020 2020 2020 2020 2065  ne.            e
+000129f0: 6c69 6620 6973 696e 7374 616e 6365 2869  lif isinstance(i
+00012a00: 7465 6d2c 2043 6f6d 706f 6e65 6e74 5265  tem, ComponentRe
+00012a10: 6665 7265 6e63 6529 3a0a 2020 2020 2020  ference):.      
+00012a20: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00012a30: 6566 6572 656e 6365 732e 7265 6d6f 7665  eferences.remove
+00012a40: 2869 7465 6d29 0a20 2020 2020 2020 2020  (item).         
+00012a50: 2020 2020 2020 2073 656c 662e 5f63 656c         self._cel
+00012a60: 6c2e 7265 6d6f 7665 2869 7465 6d2e 5f72  l.remove(item._r
+00012a70: 6566 6572 656e 6365 290a 2020 2020 2020  eference).      
+00012a80: 2020 2020 2020 2020 2020 6974 656d 2e6f            item.o
+00012a90: 776e 6572 203d 204e 6f6e 650a 2020 2020  wner = None.    
+00012aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012ab0: 2e5f 6e61 6d65 645f 7265 6665 7265 6e63  ._named_referenc
+00012ac0: 6573 2e70 6f70 2869 7465 6d2e 6e61 6d65  es.pop(item.name
+00012ad0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00012ae0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012af0: 2020 2020 7365 6c66 2e5f 6365 6c6c 2e72      self._cell.r
+00012b00: 656d 6f76 6528 6974 656d 290a 0a20 2020  emove(item)..   
+00012b10: 2020 2020 2073 656c 662e 5f62 625f 7661       self._bb_va
+00012b20: 6c69 6420 3d20 4661 6c73 650a 2020 2020  lid = False.    
+00012b30: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00012b40: 0a20 2020 2064 6566 2068 6173 685f 6765  .    def hash_ge
+00012b50: 6f6d 6574 7279 2873 656c 662c 2070 7265  ometry(self, pre
+00012b60: 6369 7369 6f6e 3a20 666c 6f61 7420 3d20  cision: float = 
+00012b70: 3165 2d34 2920 2d3e 2073 7472 3a0a 2020  1e-4) -> str:.  
+00012b80: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
+00012b90: 2061 6e20 5348 4131 2068 6173 6820 6f66   an SHA1 hash of
+00012ba0: 2074 6865 2067 656f 6d65 7472 7920 696e   the geometry in
+00012bb0: 2074 6865 2043 6f6d 706f 6e65 6e74 2e0a   the Component..
+00012bc0: 0a20 2020 2020 2020 2046 6f72 2065 6163  .        For eac
+00012bd0: 6820 6c61 7965 722c 2065 6163 6820 706f  h layer, each po
+00012be0: 6c79 676f 6e20 6973 2069 6e64 6976 6964  lygon is individ
+00012bf0: 7561 6c6c 7920 6861 7368 6564 2061 6e64  ually hashed and
+00012c00: 2074 6865 6e20 7468 6520 706f 6c79 676f   then the polygo
+00012c10: 6e20 6861 7368 6573 0a20 2020 2020 2020  n hashes.       
+00012c20: 2061 7265 2073 6f72 7465 642c 2074 6f20   are sorted, to 
+00012c30: 656e 7375 7265 2074 6865 2068 6173 6820  ensure the hash 
+00012c40: 7374 6179 7320 636f 6e73 7461 6e74 2072  stays constant r
+00012c50: 6567 6172 646c 6573 7320 6f66 2074 6865  egardless of the
+00012c60: 206f 7264 6572 696e 670a 2020 2020 2020   ordering.      
+00012c70: 2020 7468 6520 706f 6c79 676f 6e73 2e20    the polygons. 
+00012c80: 2053 696d 696c 6172 6c79 2c20 7468 6520   Similarly, the 
+00012c90: 6c61 7965 7273 2061 7265 2073 6f72 7465  layers are sorte
+00012ca0: 6420 6279 2028 6c61 7965 722c 2064 6174  d by (layer, dat
+00012cb0: 6174 7970 6529 2e0a 0a20 2020 2020 2020  atype)...       
+00012cc0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00012cd0: 2020 2070 7265 6369 7369 6f6e 3a20 526f     precision: Ro
+00012ce0: 756e 6469 6e67 2070 7265 6369 7369 6f6e  unding precision
+00012cf0: 2066 6f72 2074 6865 2074 6865 206f 626a   for the the obj
+00012d00: 6563 7473 2069 6e20 7468 6520 436f 6d70  ects in the Comp
+00012d10: 6f6e 656e 742e 0a20 2020 2020 2020 2020  onent..         
+00012d20: 2020 2020 2020 2046 6f72 2069 6e73 7461         For insta
+00012d30: 6e63 652c 2061 2070 7265 6369 7369 6f6e  nce, a precision
+00012d40: 206f 6620 3165 2d32 2077 696c 6c20 726f   of 1e-2 will ro
+00012d50: 756e 6420 6120 706f 696e 7420 6174 0a20  und a point at. 
+00012d60: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00012d70: 302e 3132 342c 2031 2e37 3438 2920 746f  0.124, 1.748) to
+00012d80: 2028 302e 3132 2c20 312e 3735 292e 0a0a   (0.12, 1.75)...
+00012d90: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012da0: 2020 2020 706f 6c79 676f 6e73 5f62 795f      polygons_by_
+00012db0: 7370 6563 203d 2073 656c 662e 6765 745f  spec = self.get_
+00012dc0: 706f 6c79 676f 6e73 2862 795f 7370 6563  polygons(by_spec
+00012dd0: 3d54 7275 652c 2061 735f 6172 7261 793d  =True, as_array=
+00012de0: 4661 6c73 6529 0a20 2020 2020 2020 206c  False).        l
+00012df0: 6179 6572 7320 3d20 6e70 2e61 7272 6179  ayers = np.array
+00012e00: 286c 6973 7428 706f 6c79 676f 6e73 5f62  (list(polygons_b
+00012e10: 795f 7370 6563 2e6b 6579 7328 2929 290a  y_spec.keys())).
+00012e20: 2020 2020 2020 2020 736f 7274 6564 5f6c          sorted_l
+00012e30: 6179 6572 7320 3d20 6c61 7965 7273 5b6e  ayers = layers[n
+00012e40: 702e 6c65 7873 6f72 7428 286c 6179 6572  p.lexsort((layer
+00012e50: 735b 3a2c 2030 5d2c 206c 6179 6572 735b  s[:, 0], layers[
+00012e60: 3a2c 2031 5d29 295d 0a0a 2020 2020 2020  :, 1]))]..      
+00012e70: 2020 6669 6e61 6c5f 6861 7368 203d 2068    final_hash = h
+00012e80: 6173 686c 6962 2e73 6861 3128 290a 2020  ashlib.sha1().  
+00012e90: 2020 2020 2020 666f 7220 6c61 7965 7220        for layer 
+00012ea0: 696e 2073 6f72 7465 645f 6c61 7965 7273  in sorted_layers
+00012eb0: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+00012ec0: 7965 725f 6861 7368 203d 2068 6173 686c  yer_hash = hashl
+00012ed0: 6962 2e73 6861 3128 6c61 7965 722e 6173  ib.sha1(layer.as
+00012ee0: 7479 7065 286e 702e 696e 7436 3429 292e  type(np.int64)).
+00012ef0: 6469 6765 7374 2829 0a20 2020 2020 2020  digest().       
+00012f00: 2020 2020 2070 6f6c 7967 6f6e 7320 3d20       polygons = 
+00012f10: 706f 6c79 676f 6e73 5f62 795f 7370 6563  polygons_by_spec
+00012f20: 5b74 7570 6c65 286c 6179 6572 295d 0a20  [tuple(layer)]. 
+00012f30: 2020 2020 2020 2020 2020 2070 6f6c 7967             polyg
+00012f40: 6f6e 7320 3d20 5b5f 726e 6428 702e 706f  ons = [_rnd(p.po
+00012f50: 696e 7473 2c20 7072 6563 6973 696f 6e29  ints, precision)
+00012f60: 2066 6f72 2070 2069 6e20 706f 6c79 676f   for p in polygo
+00012f70: 6e73 5d0a 2020 2020 2020 2020 2020 2020  ns].            
+00012f80: 706f 6c79 676f 6e5f 6861 7368 6573 203d  polygon_hashes =
+00012f90: 206e 702e 736f 7274 285b 6861 7368 6c69   np.sort([hashli
+00012fa0: 622e 7368 6131 2870 292e 6469 6765 7374  b.sha1(p).digest
+00012fb0: 2829 2066 6f72 2070 2069 6e20 706f 6c79  () for p in poly
+00012fc0: 676f 6e73 5d29 0a20 2020 2020 2020 2020  gons]).         
+00012fd0: 2020 2066 696e 616c 5f68 6173 682e 7570     final_hash.up
+00012fe0: 6461 7465 286c 6179 6572 5f68 6173 6829  date(layer_hash)
+00012ff0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00013000: 2070 6820 696e 2070 6f6c 7967 6f6e 5f68   ph in polygon_h
+00013010: 6173 6865 733a 0a20 2020 2020 2020 2020  ashes:.         
+00013020: 2020 2020 2020 2066 696e 616c 5f68 6173         final_has
+00013030: 682e 7570 6461 7465 2870 6829 0a0a 2020  h.update(ph)..  
+00013040: 2020 2020 2020 7265 7475 726e 2066 696e        return fin
+00013050: 616c 5f68 6173 682e 6865 7864 6967 6573  al_hash.hexdiges
+00013060: 7428 290a 0a20 2020 2064 6566 2067 6574  t()..    def get
+00013070: 5f6c 6162 656c 7328 0a20 2020 2020 2020  _labels(.       
+00013080: 2073 656c 662c 2061 7070 6c79 5f72 6570   self, apply_rep
+00013090: 6574 6974 696f 6e73 3d54 7275 652c 2064  etitions=True, d
+000130a0: 6570 7468 3a20 4f70 7469 6f6e 616c 5b69  epth: Optional[i
+000130b0: 6e74 5d20 3d20 4e6f 6e65 2c20 6c61 7965  nt] = None, laye
+000130c0: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
+000130d0: 4c69 7374 5b4c 6162 656c 5d3a 0a20 2020  List[Label]:.   
+000130e0: 2020 2020 2022 2222 5265 7475 726e 206c       """Return l
+000130f0: 6162 656c 732e 0a0a 2020 2020 2020 2020  abels...        
+00013100: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00013110: 2020 6170 706c 795f 7265 7065 7469 7469    apply_repetiti
+00013120: 6f6e 733a 2e0a 2020 2020 2020 2020 2020  ons:..          
+00013130: 2020 6465 7074 683a 204e 6f6e 6520 7265    depth: None re
+00013140: 7475 726e 7320 616c 6c20 6c61 6265 6c73  turns all labels
+00013150: 2061 6e64 2030 2074 6f70 206c 6576 656c   and 0 top level
+00013160: 2e0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00013170: 7965 723a 206c 6179 6572 7370 6563 2e0a  yer: layerspec..
+00013180: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013190: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
+000131a0: 6f72 792e 7064 6b20 696d 706f 7274 2067  ory.pdk import g
+000131b0: 6574 5f6c 6179 6572 0a0a 2020 2020 2020  et_layer..      
+000131c0: 2020 6966 206c 6179 6572 3a0a 2020 2020    if layer:.    
+000131d0: 2020 2020 2020 2020 6c61 7965 722c 2074          layer, t
+000131e0: 6578 7474 7970 6520 3d20 6765 745f 6c61  exttype = get_la
+000131f0: 7965 7228 6c61 7965 7229 0a20 2020 2020  yer(layer).     
+00013200: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00013210: 2020 2020 2074 6578 7474 7970 6520 3d20       texttype = 
+00013220: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
+00013230: 7572 6e20 7365 6c66 2e5f 6365 6c6c 2e67  urn self._cell.g
+00013240: 6574 5f6c 6162 656c 7328 0a20 2020 2020  et_labels(.     
+00013250: 2020 2020 2020 2061 7070 6c79 5f72 6570         apply_rep
+00013260: 6574 6974 696f 6e73 3d61 7070 6c79 5f72  etitions=apply_r
+00013270: 6570 6574 6974 696f 6e73 2c0a 2020 2020  epetitions,.    
+00013280: 2020 2020 2020 2020 6465 7074 683d 6465          depth=de
+00013290: 7074 682c 0a20 2020 2020 2020 2020 2020  pth,.           
+000132a0: 206c 6179 6572 3d6c 6179 6572 2c0a 2020   layer=layer,.  
+000132b0: 2020 2020 2020 2020 2020 7465 7874 7479            textty
+000132c0: 7065 3d74 6578 7474 7970 652c 0a20 2020  pe=texttype,.   
+000132d0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+000132e0: 7265 6d6f 7665 5f6c 6162 656c 7328 7365  remove_labels(se
+000132f0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00013300: 2020 2020 2022 2222 5265 6d6f 7665 206c       """Remove l
+00013310: 6162 656c 732e 2222 220a 2020 2020 2020  abels.""".      
+00013320: 2020 7365 6c66 2e5f 6365 6c6c 2e72 656d    self._cell.rem
+00013330: 6f76 6528 2a73 656c 662e 6c61 6265 6c73  ove(*self.labels
+00013340: 290a 0a20 2020 2023 2044 6570 7265 6361  )..    # Depreca
+00013350: 7465 640a 2020 2020 6465 6620 6765 745f  ted.    def get_
+00013360: 696e 666f 2873 656c 6629 3a0a 2020 2020  info(self):.    
+00013370: 2020 2020 2222 2247 6174 6865 7273 2074      """Gathers t
+00013380: 6865 202e 696e 666f 2064 6963 7469 6f6e  he .info diction
+00013390: 6172 6965 7320 6672 6f6d 2065 7665 7279  aries from every
+000133a0: 2073 7562 2d43 6f6d 706f 6e65 6e74 2061   sub-Component a
+000133b0: 6e64 2072 6574 7572 6e73 2074 6865 6d20  nd returns them 
+000133c0: 696e 2061 206c 6973 742e 0a0a 2020 2020  in a list...    
+000133d0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000133e0: 2020 2020 2020 6465 7074 683a 2069 6e74        depth: int
+000133f0: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+00013400: 2020 2020 2020 2020 2049 6620 6e6f 7420           If not 
+00013410: 4e6f 6e65 2c20 6465 6669 6e65 7320 6672  None, defines fr
+00013420: 6f6d 2068 6f77 206d 616e 7920 7265 6665  om how many refe
+00013430: 7265 6e63 6520 6c65 7665 6c73 2074 6f0a  rence levels to.
+00013440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013450: 7265 7472 6965 7665 2050 6f72 7473 2066  retrieve Ports f
+00013460: 726f 6d2e 0a0a 2020 2020 2020 2020 5265  rom...        Re
+00013470: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00013480: 2020 206c 6973 7420 6f66 2064 6963 7469     list of dicti
+00013490: 6f6e 6172 6965 730a 2020 2020 2020 2020  onaries.        
+000134a0: 2020 2020 2020 2020 4c69 7374 206f 6620          List of 
+000134b0: 7468 6520 222e 696e 666f 2220 7072 6f70  the ".info" prop
+000134c0: 6572 7479 2064 6963 7469 6f6e 6172 6965  erty dictionarie
+000134d0: 7320 6672 6f6d 2061 6c6c 2073 7562 2d43  s from all sub-C
+000134e0: 6f6d 706f 6e65 6e74 730a 2020 2020 2020  omponents.      
+000134f0: 2020 2222 220a 2020 2020 2020 2020 445f    """.        D_
+00013500: 6c69 7374 203d 2073 656c 662e 6765 745f  list = self.get_
+00013510: 6465 7065 6e64 656e 6369 6573 2872 6563  dependencies(rec
+00013520: 7572 7369 7665 3d54 7275 6529 0a20 2020  ursive=True).   
+00013530: 2020 2020 2072 6574 7572 6e20 5b44 2e69       return [D.i
+00013540: 6e66 6f2e 636f 7079 2829 2066 6f72 2044  nfo.copy() for D
+00013550: 2069 6e20 445f 6c69 7374 5d0a 0a20 2020   in D_list]..   
+00013560: 2064 6566 2072 656d 6170 5f6c 6179 6572   def remap_layer
+00013570: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+00013580: 206c 6179 6572 6d61 702c 2069 6e63 6c75   layermap, inclu
+00013590: 6465 5f6c 6162 656c 733a 2062 6f6f 6c20  de_labels: bool 
+000135a0: 3d20 5472 7565 2c20 696e 636c 7564 655f  = True, include_
+000135b0: 7061 7468 733a 2062 6f6f 6c20 3d20 5472  paths: bool = Tr
+000135c0: 7565 0a20 2020 2029 202d 3e20 436f 6d70  ue.    ) -> Comp
+000135d0: 6f6e 656e 743a 0a20 2020 2020 2020 2022  onent:.        "
+000135e0: 2222 5265 7475 726e 7320 6120 636f 7079  ""Returns a copy
+000135f0: 206f 6620 7468 6520 636f 6d70 6f6e 656e   of the componen
+00013600: 7420 7769 7468 2072 656d 6170 7065 6420  t with remapped 
+00013610: 6c61 7965 7273 2e0a 0a20 2020 2020 2020  layers...       
+00013620: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00013630: 2020 206c 6179 6572 6d61 703a 2044 6963     layermap: Dic
+00013640: 7469 6f6e 6172 7920 6f66 2076 616c 7565  tionary of value
+00013650: 7320 696e 2066 6f72 6d61 7420 7b6c 6179  s in format {lay
+00013660: 6572 5f66 726f 6d20 3a20 6c61 7965 725f  er_from : layer_
+00013670: 746f 7d2e 0a20 2020 2020 2020 2020 2020  to}..           
+00013680: 2069 6e63 6c75 6465 5f6c 6162 656c 733a   include_labels:
+00013690: 2053 656c 6563 7473 2077 6865 7468 6572   Selects whether
+000136a0: 2074 6f20 6d6f 7665 204c 6162 656c 7320   to move Labels 
+000136b0: 616c 6f6e 6720 7769 7468 2070 6f6c 7967  along with polyg
+000136c0: 6f6e 732e 0a20 2020 2020 2020 2020 2020  ons..           
+000136d0: 2069 6e63 6c75 6465 5f70 6174 6873 3a20   include_paths: 
+000136e0: 5365 6c65 6374 7320 7768 6574 6865 7220  Selects whether 
+000136f0: 746f 206d 6f76 6520 5061 7468 7320 616c  to move Paths al
+00013700: 6f6e 6720 7769 7468 2070 6f6c 7967 6f6e  ong with polygon
+00013710: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00013720: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
+00013730: 203d 2073 656c 662e 636f 7079 2829 0a20   = self.copy(). 
+00013740: 2020 2020 2020 206c 6179 6572 6d61 7020         layermap 
+00013750: 3d20 7b5f 7061 7273 655f 6c61 7965 7228  = {_parse_layer(
+00013760: 6b29 3a20 5f70 6172 7365 5f6c 6179 6572  k): _parse_layer
+00013770: 2876 2920 666f 7220 6b2c 2076 2069 6e20  (v) for k, v in 
+00013780: 6c61 7965 726d 6170 2e69 7465 6d73 2829  layermap.items()
+00013790: 7d0a 0a20 2020 2020 2020 2061 6c6c 5f44  }..        all_D
+000137a0: 203d 206c 6973 7428 636f 6d70 6f6e 656e   = list(componen
+000137b0: 742e 6765 745f 6465 7065 6e64 656e 6369  t.get_dependenci
+000137c0: 6573 2854 7275 6529 290a 2020 2020 2020  es(True)).      
+000137d0: 2020 616c 6c5f 442e 6170 7065 6e64 2863    all_D.append(c
+000137e0: 6f6d 706f 6e65 6e74 290a 2020 2020 2020  omponent).      
+000137f0: 2020 666f 7220 4420 696e 2061 6c6c 5f44    for D in all_D
+00013800: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00013810: 7220 7020 696e 2044 2e70 6f6c 7967 6f6e  r p in D.polygon
+00013820: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00013830: 2020 206c 6179 6572 203d 2028 702e 6c61     layer = (p.la
+00013840: 7965 722c 2070 2e64 6174 6174 7970 6529  yer, p.datatype)
+00013850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013860: 2069 6620 6c61 7965 7220 696e 206c 6179   if layer in lay
+00013870: 6572 6d61 703a 0a20 2020 2020 2020 2020  ermap:.         
+00013880: 2020 2020 2020 2020 2020 206e 6577 5f6c             new_l
+00013890: 6179 6572 203d 206c 6179 6572 6d61 705b  ayer = layermap[
+000138a0: 6c61 7965 725d 0a20 2020 2020 2020 2020  layer].         
+000138b0: 2020 2020 2020 2020 2020 2070 2e6c 6179             p.lay
+000138c0: 6572 203d 206e 6577 5f6c 6179 6572 5b30  er = new_layer[0
+000138d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000138e0: 2020 2020 2020 702e 6461 7461 7479 7065        p.datatype
+000138f0: 203d 206e 6577 5f6c 6179 6572 5b31 5d0a   = new_layer[1].
+00013900: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00013910: 6e63 6c75 6465 5f6c 6162 656c 733a 0a20  nclude_labels:. 
+00013920: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013930: 6f72 206c 6162 656c 2069 6e20 442e 6c61  or label in D.la
+00013940: 6265 6c73 3a0a 2020 2020 2020 2020 2020  bels:.          
+00013950: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
+00013960: 616c 5f6c 6179 6572 203d 2028 6c61 6265  al_layer = (labe
+00013970: 6c2e 6c61 7965 722c 206c 6162 656c 2e74  l.layer, label.t
+00013980: 6578 7474 7970 6529 0a20 2020 2020 2020  exttype).       
+00013990: 2020 2020 2020 2020 2020 2020 206f 7269               ori
+000139a0: 6769 6e61 6c5f 6c61 7965 7220 3d20 5f70  ginal_layer = _p
+000139b0: 6172 7365 5f6c 6179 6572 286f 7269 6769  arse_layer(origi
+000139c0: 6e61 6c5f 6c61 7965 7229 0a20 2020 2020  nal_layer).     
+000139d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000139e0: 6620 6f72 6967 696e 616c 5f6c 6179 6572  f original_layer
+000139f0: 2069 6e20 6c61 7965 726d 6170 3a0a 2020   in layermap:.  
+00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a10: 2020 2020 2020 6e65 775f 6c61 7965 7220        new_layer 
+00013a20: 3d20 6c61 7965 726d 6170 5b6f 7269 6769  = layermap[origi
+00013a30: 6e61 6c5f 6c61 7965 725d 0a20 2020 2020  nal_layer].     
+00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a50: 2020 206c 6162 656c 2e6c 6179 6572 203d     label.layer =
+00013a60: 206e 6577 5f6c 6179 6572 5b30 5d0a 2020   new_layer[0].  
+00013a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a80: 2020 2020 2020 6c61 6265 6c2e 7465 7874        label.text
+00013a90: 7479 7065 203d 206e 6577 5f6c 6179 6572  type = new_layer
+00013aa0: 5b31 5d0a 0a20 2020 2020 2020 2020 2020  [1]..           
+00013ab0: 2069 6620 696e 636c 7564 655f 7061 7468   if include_path
+00013ac0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00013ad0: 2020 2066 6f72 2070 6174 6820 696e 2044     for path in D
+00013ae0: 2e70 6174 6873 3a0a 2020 2020 2020 2020  .paths:.        
+00013af0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00013b00: 6c61 7965 7273 203d 206c 6973 7428 7061  layers = list(pa
+00013b10: 7468 2e6c 6179 6572 7329 0a20 2020 2020  th.layers).     
+00013b20: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00013b30: 6577 5f64 6174 6174 7970 6573 203d 206c  ew_datatypes = l
+00013b40: 6973 7428 7061 7468 2e64 6174 6174 7970  ist(path.datatyp
+00013b50: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+00013b60: 2020 2020 2020 2020 666f 7220 6c61 7965          for laye
+00013b70: 725f 6e75 6d62 6572 2069 6e20 7261 6e67  r_number in rang
+00013b80: 6528 6c65 6e28 6e65 775f 6c61 7965 7273  e(len(new_layers
+00013b90: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00013ba0: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
+00013bb0: 696e 616c 5f6c 6179 6572 203d 205f 7061  inal_layer = _pa
+00013bc0: 7273 655f 6c61 7965 7228 0a20 2020 2020  rse_layer(.     
+00013bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013be0: 2020 2020 2020 2028 6e65 775f 6c61 7965         (new_laye
+00013bf0: 7273 5b6c 6179 6572 5f6e 756d 6265 725d  rs[layer_number]
+00013c00: 2c20 6e65 775f 6461 7461 7479 7065 735b  , new_datatypes[
+00013c10: 6c61 7965 725f 6e75 6d62 6572 5d29 0a20  layer_number]). 
+00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c50: 2069 6620 6f72 6967 696e 616c 5f6c 6179   if original_lay
+00013c60: 6572 2069 6e20 6c61 7965 726d 6170 3a0a  er in layermap:.
+00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c80: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00013c90: 6c61 7965 7220 3d20 6c61 7965 726d 6170  layer = layermap
+00013ca0: 5b6f 7269 6769 6e61 6c5f 6c61 7965 725d  [original_layer]
+00013cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013cc0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+00013cd0: 5f6c 6179 6572 735b 6c61 7965 725f 6e75  _layers[layer_nu
+00013ce0: 6d62 6572 5d20 3d20 6e65 775f 6c61 7965  mber] = new_laye
+00013cf0: 725b 305d 0a20 2020 2020 2020 2020 2020  r[0].           
+00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d10: 206e 6577 5f64 6174 6174 7970 6573 5b6c   new_datatypes[l
+00013d20: 6179 6572 5f6e 756d 6265 725d 203d 206e  ayer_number] = n
+00013d30: 6577 5f6c 6179 6572 5b31 5d0a 2020 2020  ew_layer[1].    
+00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d50: 7061 7468 2e73 6574 5f6c 6179 6572 7328  path.set_layers(
+00013d60: 2a6e 6577 5f6c 6179 6572 7329 0a20 2020  *new_layers).   
+00013d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d80: 2070 6174 682e 7365 745f 6461 7461 7479   path.set_dataty
+00013d90: 7065 7328 2a6e 6577 5f64 6174 6174 7970  pes(*new_datatyp
+00013da0: 6573 290a 2020 2020 2020 2020 7265 7475  es).        retu
+00013db0: 726e 2063 6f6d 706f 6e65 6e74 0a0a 2020  rn component..  
+00013dc0: 2020 6465 6620 746f 5f33 6428 0a20 2020    def to_3d(.   
+00013dd0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00013de0: 2020 206c 6179 6572 5f76 6965 7773 3a20     layer_views: 
+00013df0: 4f70 7469 6f6e 616c 5b4c 6179 6572 5669  Optional[LayerVi
+00013e00: 6577 735d 203d 204e 6f6e 652c 0a20 2020  ews] = None,.   
+00013e10: 2020 2020 206c 6179 6572 5f73 7461 636b       layer_stack
+00013e20: 3a20 4f70 7469 6f6e 616c 5b4c 6179 6572  : Optional[Layer
+00013e30: 5374 6163 6b5d 203d 204e 6f6e 652c 0a20  Stack] = None,. 
+00013e40: 2020 2020 2020 2065 7863 6c75 6465 5f6c         exclude_l
+00013e50: 6179 6572 733a 204f 7074 696f 6e61 6c5b  ayers: Optional[
+00013e60: 5475 706c 655b 4c61 7965 722c 202e 2e2e  Tuple[Layer, ...
+00013e70: 5d5d 203d 204e 6f6e 652c 0a20 2020 2029  ]] = None,.    )
+00013e80: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+00013e90: 7572 6e20 436f 6d70 6f6e 656e 7420 3344  urn Component 3D
+00013ea0: 2074 7269 6d65 7368 2053 6365 6e65 2e0a   trimesh Scene..
+00013eb0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00013ec0: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
+00013ed0: 6e65 6e74 3a20 746f 2065 7874 7275 6465  nent: to extrude
+00013ee0: 2069 6e20 3344 2e0a 2020 2020 2020 2020   in 3D..        
+00013ef0: 2020 2020 6c61 7965 725f 7669 6577 733a      layer_views:
+00013f00: 206c 6179 6572 2063 6f6c 6f72 7320 6672   layer colors fr
+00013f10: 6f6d 204b 6c61 796f 7574 204c 6179 6572  om Klayout Layer
+00013f20: 2050 726f 7065 7274 6965 7320 6669 6c65   Properties file
+00013f30: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013f40: 2020 4465 6661 756c 7473 2074 6f20 6163    Defaults to ac
+00013f50: 7469 7665 2050 444b 2e6c 6179 6572 5f76  tive PDK.layer_v
+00013f60: 6965 7773 2e0a 2020 2020 2020 2020 2020  iews..          
+00013f70: 2020 6c61 7965 725f 7374 6163 6b3a 2063    layer_stack: c
+00013f80: 6f6e 7461 696e 7320 7468 6963 6b6e 6573  ontains thicknes
+00013f90: 7320 616e 6420 7a6d 696e 2066 6f72 2065  s and zmin for e
+00013fa0: 6163 6820 6c61 7965 722e 0a20 2020 2020  ach layer..     
+00013fb0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+00013fc0: 6c74 7320 746f 2061 6374 6976 6520 5044  lts to active PD
+00013fd0: 4b2e 6c61 7965 725f 7374 6163 6b2e 0a20  K.layer_stack.. 
+00013fe0: 2020 2020 2020 2020 2020 2065 7863 6c75             exclu
+00013ff0: 6465 5f6c 6179 6572 733a 206c 6179 6572  de_layers: layer
+00014000: 7320 746f 2065 7863 6c75 6465 2e0a 0a20  s to exclude... 
+00014010: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014020: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
+00014030: 7279 2e65 7870 6f72 742e 746f 5f33 6420  ry.export.to_3d 
+00014040: 696d 706f 7274 2074 6f5f 3364 0a0a 2020  import to_3d..  
+00014050: 2020 2020 2020 7265 7475 726e 2074 6f5f        return to_
+00014060: 3364 280a 2020 2020 2020 2020 2020 2020  3d(.            
+00014070: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00014080: 2020 6c61 7965 725f 7669 6577 733d 6c61    layer_views=la
+00014090: 7965 725f 7669 6577 732c 0a20 2020 2020  yer_views,.     
+000140a0: 2020 2020 2020 206c 6179 6572 5f73 7461         layer_sta
+000140b0: 636b 3d6c 6179 6572 5f73 7461 636b 2c0a  ck=layer_stack,.
+000140c0: 2020 2020 2020 2020 2020 2020 6578 636c              excl
+000140d0: 7564 655f 6c61 7965 7273 3d65 7863 6c75  ude_layers=exclu
+000140e0: 6465 5f6c 6179 6572 732c 0a20 2020 2020  de_layers,.     
+000140f0: 2020 2029 0a0a 2020 2020 6465 6620 746f     )..    def to
+00014100: 5f6e 7028 0a20 2020 2020 2020 2073 656c  _np(.        sel
+00014110: 662c 0a20 2020 2020 2020 206e 6d5f 7065  f,.        nm_pe
+00014120: 725f 7069 7865 6c3a 2069 6e74 203d 2032  r_pixel: int = 2
+00014130: 302c 0a20 2020 2020 2020 206c 6179 6572  0,.        layer
+00014140: 733a 204c 6179 6572 7320 3d20 2828 312c  s: Layers = ((1,
+00014150: 2030 292c 292c 0a20 2020 2020 2020 2076   0),),.        v
+00014160: 616c 7565 733a 204f 7074 696f 6e61 6c5b  alues: Optional[
+00014170: 5475 706c 655b 666c 6f61 742c 202e 2e2e  Tuple[float, ...
+00014180: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+00014190: 2020 2070 6164 5f77 6964 7468 3a20 696e     pad_width: in
+000141a0: 7420 3d20 312c 0a20 2020 2029 202d 3e20  t = 1,.    ) -> 
+000141b0: 6e70 2e6e 6461 7272 6179 3a0a 2020 2020  np.ndarray:.    
+000141c0: 2020 2020 2222 2252 6574 7572 6e73 2061      """Returns a
+000141d0: 2070 6978 656c 6174 6564 206e 756d 7079   pixelated numpy
+000141e0: 2061 7272 6179 2066 726f 6d20 436f 6d70   array from Comp
+000141f0: 6f6e 656e 7420 706f 6c79 676f 6e73 2e0a  onent polygons..
+00014200: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00014210: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
+00014220: 6e65 6e74 3a20 436f 6d70 6f6e 656e 742e  nent: Component.
+00014230: 0a20 2020 2020 2020 2020 2020 206e 6d5f  .            nm_
+00014240: 7065 725f 7069 7865 6c3a 2079 6f75 2063  per_pixel: you c
+00014250: 616e 2067 6f20 6672 6f6d 2032 3020 2863  an go from 20 (c
+00014260: 6f61 7273 6529 2074 6f20 3420 2866 696e  oarse) to 4 (fin
+00014270: 6529 2e0a 2020 2020 2020 2020 2020 2020  e)..            
+00014280: 6c61 7965 7273 3a20 746f 2063 6f6e 7665  layers: to conve
+00014290: 7274 2e20 4f72 6465 7220 6d61 7474 6572  rt. Order matter
+000142a0: 7320 286c 6174 7465 7220 6f76 6572 7772  s (latter overwr
+000142b0: 6974 6520 666f 726d 6572 292e 0a20 2020  ite former)..   
+000142c0: 2020 2020 2020 2020 2076 616c 7565 733a           values:
+000142d0: 2061 7373 6f63 6961 7465 6420 746f 2065   associated to e
+000142e0: 6163 6820 6c61 7965 7220 2864 6566 6175  ach layer (defau
+000142f0: 6c74 7320 746f 2031 292e 0a20 2020 2020  lts to 1)..     
+00014300: 2020 2020 2020 2070 6164 5f77 6964 7468         pad_width
+00014310: 3a20 7061 6464 696e 6720 7069 7865 6c73  : padding pixels
+00014320: 2061 726f 756e 6420 7468 6520 696d 6167   around the imag
+00014330: 652e 0a0a 2020 2020 2020 2020 2222 220a  e...        """.
+00014340: 2020 2020 2020 2020 6672 6f6d 2067 6473          from gds
+00014350: 6661 6374 6f72 792e 6578 706f 7274 2e74  factory.export.t
+00014360: 6f5f 6e70 2069 6d70 6f72 7420 746f 5f6e  o_np import to_n
+00014370: 700a 0a20 2020 2020 2020 2072 6574 7572  p..        retur
+00014380: 6e20 746f 5f6e 7028 0a20 2020 2020 2020  n to_np(.       
+00014390: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000143a0: 2020 2020 2020 206e 6d5f 7065 725f 7069         nm_per_pi
+000143b0: 7865 6c3d 6e6d 5f70 6572 5f70 6978 656c  xel=nm_per_pixel
+000143c0: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
+000143d0: 7965 7273 3d6c 6179 6572 732c 0a20 2020  yers=layers,.   
+000143e0: 2020 2020 2020 2020 2076 616c 7565 733d           values=
+000143f0: 7661 6c75 6573 2c0a 2020 2020 2020 2020  values,.        
+00014400: 2020 2020 7061 645f 7769 6474 683d 7061      pad_width=pa
+00014410: 645f 7769 6474 682c 0a20 2020 2020 2020  d_width,.       
+00014420: 2029 0a0a 2020 2020 6465 6620 7772 6974   )..    def writ
+00014430: 655f 7374 6c28 0a20 2020 2020 2020 2073  e_stl(.        s
+00014440: 656c 662c 0a20 2020 2020 2020 2066 696c  elf,.        fil
+00014450: 6570 6174 683a 2073 7472 2c0a 2020 2020  epath: str,.    
+00014460: 2020 2020 6c61 7965 725f 7374 6163 6b3a      layer_stack:
+00014470: 204f 7074 696f 6e61 6c5b 4c61 7965 7253   Optional[LayerS
+00014480: 7461 636b 5d20 3d20 4e6f 6e65 2c0a 2020  tack] = None,.  
+00014490: 2020 2020 2020 6578 636c 7564 655f 6c61        exclude_la
+000144a0: 7965 7273 3a20 4f70 7469 6f6e 616c 5b54  yers: Optional[T
+000144b0: 7570 6c65 5b4c 6179 6572 2c20 2e2e 2e5d  uple[Layer, ...]
+000144c0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2920  ] = None,.    ) 
+000144d0: 2d3e 206e 702e 6e64 6172 7261 793a 0a20  -> np.ndarray:. 
+000144e0: 2020 2020 2020 2022 2222 5772 6974 6520         """Write 
+000144f0: 6120 436f 6d70 6f6e 656e 7420 746f 2053  a Component to S
+00014500: 544c 2066 6f72 2033 4420 7072 696e 7469  TL for 3D printi
+00014510: 6e67 2e0a 0a20 2020 2020 2020 2041 7267  ng...        Arg
+00014520: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+00014530: 696c 6570 6174 683a 2074 6f20 7772 6974  ilepath: to writ
+00014540: 6520 5354 4c20 746f 2e0a 2020 2020 2020  e STL to..      
+00014550: 2020 2020 2020 6c61 7965 725f 7374 6163        layer_stac
+00014560: 6b3a 2063 6f6e 7461 696e 7320 7468 6963  k: contains thic
+00014570: 6b6e 6573 7320 616e 6420 7a6d 696e 2066  kness and zmin f
+00014580: 6f72 2065 6163 6820 6c61 7965 722e 0a20  or each layer.. 
+00014590: 2020 2020 2020 2020 2020 2065 7863 6c75             exclu
+000145a0: 6465 5f6c 6179 6572 733a 206c 6179 6572  de_layers: layer
+000145b0: 7320 746f 2065 7863 6c75 6465 2e0a 2020  s to exclude..  
+000145c0: 2020 2020 2020 2020 2020 7573 655f 6c61            use_la
+000145d0: 7965 725f 6e61 6d65 3a20 4966 2054 7275  yer_name: If Tru
+000145e0: 652c 2075 7365 7320 4c61 7965 724c 6576  e, uses LayerLev
+000145f0: 656c 206e 616d 6573 2069 6e20 6f75 7470  el names in outp
+00014600: 7574 2066 696c 656e 616d 6573 2072 6174  ut filenames rat
+00014610: 6865 7220 7468 616e 2067 6473 5f6c 6179  her than gds_lay
+00014620: 6572 2061 6e64 2067 6473 5f64 6174 6174  er and gds_datat
+00014630: 7970 652e 0a20 2020 2020 2020 2020 2020  ype..           
+00014640: 2068 756c 6c5f 696e 7661 6c69 645f 706f   hull_invalid_po
+00014650: 6c79 676f 6e73 3a20 4966 2054 7275 652c  lygons: If True,
+00014660: 2072 6570 6c61 6365 7320 696e 7661 6c69   replaces invali
+00014670: 6420 706f 6c79 676f 6e73 2028 6465 7465  d polygons (dete
+00014680: 726d 696e 6564 2062 7920 7368 6170 656c  rmined by shapel
+00014690: 792e 506f 6c79 676f 6e2e 6973 5f76 616c  y.Polygon.is_val
+000146a0: 6964 2920 7769 7468 2069 7473 2063 6f6e  id) with its con
+000146b0: 7665 7820 6875 6c6c 2e0a 2020 2020 2020  vex hull..      
+000146c0: 2020 2020 2020 7363 616c 653a 204f 7074        scale: Opt
+000146d0: 696f 6e61 6c20 6661 6374 6f72 2062 7920  ional factor by 
+000146e0: 7768 6963 6820 746f 2073 6361 6c65 206d  which to scale m
+000146f0: 6573 6865 7320 6265 666f 7265 2077 7269  eshes before wri
+00014700: 7469 6e67 2e0a 0a20 2020 2020 2020 2022  ting...        "
+00014710: 2222 0a20 2020 2020 2020 2066 726f 6d20  "".        from 
+00014720: 6764 7366 6163 746f 7279 2e65 7870 6f72  gdsfactory.expor
+00014730: 742e 746f 5f73 746c 2069 6d70 6f72 7420  t.to_stl import 
+00014740: 746f 5f73 746c 0a0a 2020 2020 2020 2020  to_stl..        
+00014750: 7265 7475 726e 2074 6f5f 7374 6c28 0a20  return to_stl(. 
+00014760: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00014770: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00014780: 6570 6174 683d 6669 6c65 7061 7468 2c0a  epath=filepath,.
+00014790: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+000147a0: 725f 7374 6163 6b3d 6c61 7965 725f 7374  r_stack=layer_st
+000147b0: 6163 6b2c 0a20 2020 2020 2020 2020 2020  ack,.           
+000147c0: 2065 7863 6c75 6465 5f6c 6179 6572 733d   exclude_layers=
+000147d0: 6578 636c 7564 655f 6c61 7965 7273 2c0a  exclude_layers,.
+000147e0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+000147f0: 6566 2074 6f5f 676d 7368 280a 2020 2020  ef to_gmsh(.    
+00014800: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00014810: 2020 7479 7065 2c0a 2020 2020 2020 2020    type,.        
+00014820: 7a3d 4e6f 6e65 2c0a 2020 2020 2020 2020  z=None,.        
+00014830: 7873 6563 7469 6f6e 5f62 6f75 6e64 733d  xsection_bounds=
+00014840: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c61  None,.        la
+00014850: 7965 725f 7374 6163 6b3d 4e6f 6e65 2c0a  yer_stack=None,.
+00014860: 2020 2020 2020 2020 7761 6665 725f 7061          wafer_pa
+00014870: 6464 696e 673d 302e 302c 0a20 2020 2020  dding=0.0,.     
+00014880: 2020 2077 6166 6572 5f6c 6179 6572 3d4c     wafer_layer=L
+00014890: 4159 4552 2e57 4146 4552 2c0a 2020 2020  AYER.WAFER,.    
+000148a0: 2020 2020 2a61 7267 732c 0a20 2020 2020      *args,.     
+000148b0: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
+000148c0: 2029 3a0a 2020 2020 2020 2020 2222 2252   ):.        """R
+000148d0: 6574 7572 6e73 2061 2067 6d73 6820 6d73  eturns a gmsh ms
+000148e0: 6820 6f66 2074 6865 2063 6f6d 706f 6e65  h of the compone
+000148f0: 6e74 2066 6f72 2066 696e 6974 6520 656c  nt for finite el
+00014900: 656d 656e 7420 7369 6d75 6c61 7469 6f6e  ement simulation
+00014910: 2e0a 0a20 2020 2020 2020 2041 7267 756d  ...        Argum
+00014920: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
+00014930: 2020 7479 7065 3a20 6f6e 6520 6f66 2022    type: one of "
+00014940: 7879 222c 2022 757a 222c 206f 7220 2233  xy", "uz", or "3
+00014950: 4422 2e20 4465 7465 726d 696e 6573 2074  D". Determines t
+00014960: 6865 2074 7970 6520 6f66 206d 6573 6820  he type of mesh 
+00014970: 746f 2072 6574 7572 6e2e 0a20 2020 2020  to return..     
+00014980: 2020 2020 2020 207a 3a20 7573 6564 2074         z: used t
+00014990: 6f20 6465 6669 6e65 207a 2d73 6c69 6365  o define z-slice
+000149a0: 2066 6f72 2078 7920 6d65 7368 696e 670a   for xy meshing.
+000149b0: 2020 2020 2020 2020 2020 2020 7873 6563              xsec
+000149c0: 7469 6f6e 5f62 6f75 6e64 733a 2075 7365  tion_bounds: use
+000149d0: 6420 746f 2064 6566 696e 6520 696e 2d70  d to define in-p
+000149e0: 6c61 6e65 206c 696e 6520 666f 7220 757a  lane line for uz
+000149f0: 206d 6573 6869 6e67 0a20 2020 2020 2020   meshing.       
+00014a00: 2020 2020 2077 6166 6572 5f70 6164 6469       wafer_paddi
+00014a10: 6e67 3a20 7061 6464 696e 6720 6265 796f  ng: padding beyo
+00014a20: 6e64 2062 626f 7820 746f 2061 6464 2074  nd bbox to add t
+00014a30: 6f20 5741 4645 5220 6c61 7965 7273 2e0a  o WAFER layers..
+00014a40: 0a20 2020 2020 2020 204b 6579 776f 7264  .        Keyword
+00014a50: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00014a60: 2020 2041 7267 756d 656e 7473 2066 6f72     Arguments for
+00014a70: 2074 6865 2074 6172 6765 7420 6d65 7368   the target mesh
+00014a80: 696e 6720 6675 6e63 7469 6f6e 2069 6e20  ing function in 
+00014a90: 6764 7366 6163 746f 7279 2e73 696d 756c  gdsfactory.simul
+00014aa0: 6174 696f 6e2e 676d 7368 0a20 2020 2020  ation.gmsh.     
+00014ab0: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+00014ac0: 2041 6464 2057 4146 4552 206c 6179 6572   Add WAFER layer
+00014ad0: 3a0a 2020 2020 2020 2020 7061 6464 6564  :.        padded
+00014ae0: 5f63 6f6d 706f 6e65 6e74 203d 2043 6f6d  _component = Com
+00014af0: 706f 6e65 6e74 2829 0a20 2020 2020 2020  ponent().       
+00014b00: 2070 6164 6465 645f 636f 6d70 6f6e 656e   padded_componen
+00014b10: 7420 3c3c 2073 656c 660a 2020 2020 2020  t << self.      
+00014b20: 2020 2878 6d69 6e2c 2079 6d69 6e29 2c20    (xmin, ymin), 
+00014b30: 2878 6d61 782c 2079 6d61 7829 203d 2073  (xmax, ymax) = s
+00014b40: 656c 662e 6262 6f78 0a20 2020 2020 2020  elf.bbox.       
+00014b50: 2070 6f69 6e74 7320 3d20 5b0a 2020 2020   points = [.    
+00014b60: 2020 2020 2020 2020 5b78 6d69 6e20 2d20          [xmin - 
+00014b70: 7761 6665 725f 7061 6464 696e 672c 2079  wafer_padding, y
+00014b80: 6d69 6e20 2d20 7761 6665 725f 7061 6464  min - wafer_padd
+00014b90: 696e 675d 2c0a 2020 2020 2020 2020 2020  ing],.          
+00014ba0: 2020 5b78 6d61 7820 2b20 7761 6665 725f    [xmax + wafer_
+00014bb0: 7061 6464 696e 672c 2079 6d69 6e20 2d20  padding, ymin - 
+00014bc0: 7761 6665 725f 7061 6464 696e 675d 2c0a  wafer_padding],.
+00014bd0: 2020 2020 2020 2020 2020 2020 5b78 6d61              [xma
+00014be0: 7820 2b20 7761 6665 725f 7061 6464 696e  x + wafer_paddin
+00014bf0: 672c 2079 6d61 7820 2b20 7761 6665 725f  g, ymax + wafer_
+00014c00: 7061 6464 696e 675d 2c0a 2020 2020 2020  padding],.      
+00014c10: 2020 2020 2020 5b78 6d69 6e20 2d20 7761        [xmin - wa
+00014c20: 6665 725f 7061 6464 696e 672c 2079 6d61  fer_padding, yma
+00014c30: 7820 2b20 7761 6665 725f 7061 6464 696e  x + wafer_paddin
+00014c40: 675d 2c0a 2020 2020 2020 2020 5d0a 2020  g],.        ].  
+00014c50: 2020 2020 2020 7061 6464 6564 5f63 6f6d        padded_com
+00014c60: 706f 6e65 6e74 2e61 6464 5f70 6f6c 7967  ponent.add_polyg
+00014c70: 6f6e 2870 6f69 6e74 732c 206c 6179 6572  on(points, layer
+00014c80: 3d77 6166 6572 5f6c 6179 6572 290a 0a20  =wafer_layer).. 
+00014c90: 2020 2020 2020 2069 6620 6c61 7965 725f         if layer_
+00014ca0: 7374 6163 6b20 6973 204e 6f6e 653a 0a20  stack is None:. 
+00014cb0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00014cc0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+00014cd0: 2020 2020 2020 2020 2020 2020 2027 4120               'A 
+00014ce0: 4c61 7965 7253 7461 636b 206d 7573 7420  LayerStack must 
+00014cf0: 6265 2070 726f 7669 6465 6420 7468 726f  be provided thro
+00014d00: 7567 6820 6172 6775 6d65 6e74 2022 6c61  ugh argument "la
+00014d10: 7965 725f 7374 6163 6b22 2e27 0a20 2020  yer_stack".'.   
+00014d20: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00014d30: 2020 2069 6620 7479 7065 203d 3d20 2278     if type == "x
+00014d40: 7922 3a0a 2020 2020 2020 2020 2020 2020  y":.            
+00014d50: 6966 207a 2069 7320 4e6f 6e65 3a0a 2020  if z is None:.  
+00014d60: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00014d70: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+00014d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d90: 2020 2020 2746 6f72 2078 792d 6d65 7368      'For xy-mesh
+00014da0: 696e 672c 2061 207a 2d76 616c 7565 206d  ing, a z-value m
+00014db0: 7573 7420 6265 2070 726f 7669 6465 6420  ust be provided 
+00014dc0: 7669 6120 7468 6520 666c 6f61 7420 6172  via the float ar
+00014dd0: 6775 6d65 6e74 2022 7a22 2e27 0a20 2020  gument "z".'.   
+00014de0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00014df0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
+00014e00: 6764 7366 6163 746f 7279 2e73 696d 756c  gdsfactory.simul
+00014e10: 6174 696f 6e2e 676d 7368 2e78 795f 7873  ation.gmsh.xy_xs
+00014e20: 6563 7469 6f6e 5f6d 6573 6820 696d 706f  ection_mesh impo
+00014e30: 7274 2078 795f 7873 6563 7469 6f6e 5f6d  rt xy_xsection_m
+00014e40: 6573 680a 0a20 2020 2020 2020 2020 2020  esh..           
+00014e50: 2072 6574 7572 6e20 7879 5f78 7365 6374   return xy_xsect
+00014e60: 696f 6e5f 6d65 7368 2870 6164 6465 645f  ion_mesh(padded_
+00014e70: 636f 6d70 6f6e 656e 742c 207a 2c20 6c61  component, z, la
+00014e80: 7965 725f 7374 6163 6b2c 202a 2a6b 7761  yer_stack, **kwa
+00014e90: 7267 7329 0a20 2020 2020 2020 2065 6c69  rgs).        eli
+00014ea0: 6620 7479 7065 203d 3d20 2275 7a22 3a0a  f type == "uz":.
+00014eb0: 2020 2020 2020 2020 2020 2020 6966 2078              if x
+00014ec0: 7365 6374 696f 6e5f 626f 756e 6473 2069  section_bounds i
+00014ed0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00014ee0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00014ef0: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00014f00: 2020 2020 2020 2020 2020 2020 2020 2246                "F
+00014f10: 6f72 2075 7a2d 6d65 7368 696e 672c 2079  or uz-meshing, y
+00014f20: 6f75 206d 7573 7420 7072 6f76 6964 6520  ou must provide 
+00014f30: 6120 6c69 6e65 2069 6e20 7468 6520 7879  a line in the xy
+00014f40: 2d70 6c61 6e65 2022 0a20 2020 2020 2020  -plane ".       
+00014f50: 2020 2020 2020 2020 2020 2020 2022 7669               "vi
+00014f60: 6120 7468 6520 5475 706c 6520 6172 6775  a the Tuple argu
+00014f70: 6d65 6e74 205b 5b78 312c 7931 5d2c 205b  ment [[x1,y1], [
+00014f80: 7832 2c79 325d 5d20 7873 6563 7469 6f6e  x2,y2]] xsection
+00014f90: 5f62 6f75 6e64 732e 220a 2020 2020 2020  _bounds.".      
+00014fa0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014fb0: 2020 2020 2020 2020 6672 6f6d 2067 6473          from gds
+00014fc0: 6661 6374 6f72 792e 7369 6d75 6c61 7469  factory.simulati
+00014fd0: 6f6e 2e67 6d73 682e 757a 5f78 7365 6374  on.gmsh.uz_xsect
+00014fe0: 696f 6e5f 6d65 7368 2069 6d70 6f72 7420  ion_mesh import 
+00014ff0: 757a 5f78 7365 6374 696f 6e5f 6d65 7368  uz_xsection_mesh
+00015000: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00015010: 7475 726e 2075 7a5f 7873 6563 7469 6f6e  turn uz_xsection
+00015020: 5f6d 6573 6828 0a20 2020 2020 2020 2020  _mesh(.         
+00015030: 2020 2020 2020 2070 6164 6465 645f 636f         padded_co
+00015040: 6d70 6f6e 656e 742c 2078 7365 6374 696f  mponent, xsectio
+00015050: 6e5f 626f 756e 6473 2c20 6c61 7965 725f  n_bounds, layer_
+00015060: 7374 6163 6b2c 202a 2a6b 7761 7267 730a  stack, **kwargs.
+00015070: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00015080: 2020 2020 2020 656c 6966 2074 7970 6520        elif type 
+00015090: 3d3d 2022 3344 223a 0a20 2020 2020 2020  == "3D":.       
+000150a0: 2020 2020 2066 726f 6d20 6764 7366 6163       from gdsfac
+000150b0: 746f 7279 2e73 696d 756c 6174 696f 6e2e  tory.simulation.
+000150c0: 676d 7368 2e78 797a 5f6d 6573 6820 696d  gmsh.xyz_mesh im
+000150d0: 706f 7274 2078 797a 5f6d 6573 680a 0a20  port xyz_mesh.. 
+000150e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000150f0: 6e20 7879 7a5f 6d65 7368 2870 6164 6465  n xyz_mesh(padde
+00015100: 645f 636f 6d70 6f6e 656e 742c 206c 6179  d_component, lay
+00015110: 6572 5f73 7461 636b 2c20 2a2a 6b77 6172  er_stack, **kwar
+00015120: 6773 290a 2020 2020 2020 2020 656c 7365  gs).        else
+00015130: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00015140: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015160: 2752 6571 7569 7265 6420 6172 6775 6d65  'Required argume
+00015170: 6e74 2022 7479 7065 2220 6d75 7374 2062  nt "type" must b
+00015180: 6520 6f6e 6520 6f66 2022 7879 222c 2022  e one of "xy", "
+00015190: 757a 222c 206f 7220 2233 4422 2e27 0a20  uz", or "3D".'. 
+000151a0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+000151b0: 2020 6465 6620 6f66 6673 6574 280a 2020    def offset(.  
+000151c0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000151d0: 2020 2020 6469 7374 616e 6365 3a20 666c      distance: fl
+000151e0: 6f61 7420 3d20 302e 312c 0a20 2020 2020  oat = 0.1,.     
+000151f0: 2020 2070 6f6c 7967 6f6e 733d 4e6f 6e65     polygons=None
+00015200: 2c0a 2020 2020 2020 2020 7573 655f 756e  ,.        use_un
+00015210: 696f 6e3a 2062 6f6f 6c20 3d20 5472 7565  ion: bool = True
+00015220: 2c0a 2020 2020 2020 2020 7072 6563 6973  ,.        precis
+00015230: 696f 6e3a 2066 6c6f 6174 203d 2031 652d  ion: float = 1e-
+00015240: 342c 0a20 2020 2020 2020 206a 6f69 6e3a  4,.        join:
+00015250: 2073 7472 203d 2022 6d69 7465 7222 2c0a   str = "miter",.
+00015260: 2020 2020 2020 2020 746f 6c65 7261 6e63          toleranc
+00015270: 653a 2069 6e74 203d 2032 2c0a 2020 2020  e: int = 2,.    
+00015280: 2020 2020 6c61 7965 723a 204c 6179 6572      layer: Layer
+00015290: 5370 6563 203d 2022 5747 222c 0a20 2020  Spec = "WG",.   
+000152a0: 2029 202d 3e20 436f 6d70 6f6e 656e 743a   ) -> Component:
+000152b0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+000152c0: 726e 7320 6e65 7720 436f 6d70 6f6e 656e  rns new Componen
+000152d0: 7420 7769 7468 2070 6f6c 7967 6f6e 7320  t with polygons 
+000152e0: 6572 6f64 6564 206f 7220 6469 6c61 7465  eroded or dilate
+000152f0: 6420 6279 2061 6e20 6f66 6673 6574 2e0a  d by an offset..
+00015300: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00015310: 2020 2020 2020 2020 2020 2064 6973 7461             dista
+00015320: 6e63 653a 2044 6973 7461 6e63 6520 746f  nce: Distance to
+00015330: 206f 6666 7365 7420 706f 6c79 676f 6e73   offset polygons
+00015340: 2e20 506f 7369 7469 7665 2076 616c 7565  . Positive value
+00015350: 7320 6578 7061 6e64 2c20 6e65 6761 7469  s expand, negati
+00015360: 7665 2073 6872 696e 6b2e 0a20 2020 2020  ve shrink..     
+00015370: 2020 2020 2020 2070 7265 6369 7369 6f6e         precision
+00015380: 3a20 4465 7369 7265 6420 7072 6563 6973  : Desired precis
+00015390: 696f 6e20 666f 7220 726f 756e 6469 6e67  ion for rounding
+000153a0: 2076 6572 7465 7820 636f 6f72 6469 6e61   vertex coordina
+000153b0: 7465 732e 0a20 2020 2020 2020 2020 2020  tes..           
+000153c0: 206a 6f69 6e3a 207b 276d 6974 6572 272c   join: {'miter',
+000153d0: 2027 6265 7665 6c27 2c20 2772 6f75 6e64   'bevel', 'round
+000153e0: 277d 2054 7970 6520 6f66 206a 6f69 6e20  '} Type of join 
+000153f0: 7573 6564 2074 6f20 6372 6561 7465 2070  used to create p
+00015400: 6f6c 7967 6f6e 206f 6666 7365 740a 2020  olygon offset.  
+00015410: 2020 2020 2020 2020 2020 746f 6c65 7261            tolera
+00015420: 6e63 653a 2046 6f72 206d 6974 6572 206a  nce: For miter j
+00015430: 6f69 6e74 732c 2074 6869 7320 6e75 6d62  oints, this numb
+00015440: 6572 206d 7573 7420 6265 2061 7420 6c65  er must be at le
+00015450: 6173 7420 3220 7265 7072 6573 656e 7473  ast 2 represents
+00015460: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00015470: 2020 206d 6178 696d 616c 2064 6973 7461     maximal dista
+00015480: 6e63 6520 696e 206d 756c 7469 706c 6573  nce in multiples
+00015490: 206f 6620 6f66 6673 6574 2062 6574 7765   of offset betwe
+000154a0: 656e 206e 6577 2076 6572 7469 6365 7320  en new vertices 
+000154b0: 616e 6420 7468 6569 720a 2020 2020 2020  and their.      
+000154c0: 2020 2020 2020 2020 6f72 6967 696e 616c          original
+000154d0: 2070 6f73 6974 696f 6e20 6265 666f 7265   position before
+000154e0: 2062 6576 656c 696e 6720 746f 2061 766f   beveling to avo
+000154f0: 6964 2073 7069 6b65 7320 6174 2061 6375  id spikes at acu
+00015500: 7465 206a 6f69 6e74 732e 2046 6f72 0a20  te joints. For. 
+00015510: 2020 2020 2020 2020 2020 2020 2072 6f75               rou
+00015520: 6e64 206a 6f69 6e74 732c 2069 7420 696e  nd joints, it in
+00015530: 6469 6361 7465 7320 7468 6520 6375 7276  dicates the curv
+00015540: 6174 7572 6520 7265 736f 6c75 7469 6f6e  ature resolution
+00015550: 2069 6e20 6e75 6d62 6572 206f 660a 2020   in number of.  
+00015560: 2020 2020 2020 2020 2020 2020 706f 696e              poin
+00015570: 7473 2070 6572 2066 756c 6c20 6369 7263  ts per full circ
+00015580: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
+00015590: 6c61 7965 723a 2053 7065 6369 6669 6320  layer: Specific 
+000155a0: 6c61 7965 7220 666f 7220 6e65 7720 706f  layer for new po
+000155b0: 6c79 676f 6e73 2e0a 0a20 2020 2020 2020  lygons...       
+000155c0: 2022 2222 0a20 2020 2020 2020 2069 6d70   """.        imp
+000155d0: 6f72 7420 6764 7366 6163 746f 7279 2061  ort gdsfactory a
+000155e0: 7320 6766 0a0a 2020 2020 2020 2020 6764  s gf..        gd
+000155f0: 735f 6c61 7965 722c 2067 6473 5f64 6174  s_layer, gds_dat
+00015600: 6174 7970 6520 3d20 6766 2e67 6574 5f6c  atype = gf.get_l
+00015610: 6179 6572 286c 6179 6572 290a 2020 2020  ayer(layer).    
+00015620: 2020 2020 7020 3d20 6764 7374 6b2e 6f66      p = gdstk.of
+00015630: 6673 6574 280a 2020 2020 2020 2020 2020  fset(.          
+00015640: 2020 706f 6c79 676f 6e73 206f 7220 7365    polygons or se
+00015650: 6c66 2e67 6574 5f70 6f6c 7967 6f6e 7328  lf.get_polygons(
+00015660: 292c 0a20 2020 2020 2020 2020 2020 2064  ),.            d
+00015670: 6973 7461 6e63 653d 6469 7374 616e 6365  istance=distance
+00015680: 2c0a 2020 2020 2020 2020 2020 2020 6a6f  ,.            jo
+00015690: 696e 3d6a 6f69 6e2c 0a20 2020 2020 2020  in=join,.       
+000156a0: 2020 2020 2074 6f6c 6572 616e 6365 3d74       tolerance=t
+000156b0: 6f6c 6572 616e 6365 2c0a 2020 2020 2020  olerance,.      
+000156c0: 2020 2020 2020 7072 6563 6973 696f 6e3d        precision=
+000156d0: 7072 6563 6973 696f 6e2c 0a20 2020 2020  precision,.     
+000156e0: 2020 2020 2020 2075 7365 5f75 6e69 6f6e         use_union
+000156f0: 3d75 7365 5f75 6e69 6f6e 2c0a 2020 2020  =use_union,.    
+00015700: 2020 2020 2020 2020 6c61 7965 723d 6764          layer=gd
+00015710: 735f 6c61 7965 722c 0a20 2020 2020 2020  s_layer,.       
+00015720: 2020 2020 2064 6174 6174 7970 653d 6764       datatype=gd
+00015730: 735f 6461 7461 7479 7065 2c0a 2020 2020  s_datatype,.    
+00015740: 2020 2020 290a 0a20 2020 2020 2020 2063      )..        c
+00015750: 6f6d 706f 6e65 6e74 203d 2067 662e 436f  omponent = gf.Co
+00015760: 6d70 6f6e 656e 7428 290a 2020 2020 2020  mponent().      
+00015770: 2020 636f 6d70 6f6e 656e 742e 6164 645f    component.add_
+00015780: 706f 6c79 676f 6e28 702c 206c 6179 6572  polygon(p, layer
+00015790: 3d6c 6179 6572 290a 2020 2020 2020 2020  =layer).        
+000157a0: 7265 7475 726e 2063 6f6d 706f 6e65 6e74  return component
+000157b0: 0a0a 0a64 6566 2063 6f70 7928 0a20 2020  ...def copy(.   
+000157c0: 2044 3a20 436f 6d70 6f6e 656e 742c 0a20   D: Component,. 
+000157d0: 2020 2072 6566 6572 656e 6365 733d 4e6f     references=No
+000157e0: 6e65 2c0a 2020 2020 706f 7274 733d 4e6f  ne,.    ports=No
+000157f0: 6e65 2c0a 2020 2020 706f 6c79 676f 6e73  ne,.    polygons
+00015800: 3d4e 6f6e 652c 0a20 2020 2070 6174 6873  =None,.    paths
+00015810: 3d4e 6f6e 652c 0a20 2020 206e 616d 653d  =None,.    name=
+00015820: 4e6f 6e65 2c0a 2020 2020 6c61 6265 6c73  None,.    labels
+00015830: 3d4e 6f6e 652c 0a29 202d 3e20 436f 6d70  =None,.) -> Comp
+00015840: 6f6e 656e 743a 0a20 2020 2022 2222 5265  onent:.    """Re
+00015850: 7475 726e 7320 6120 436f 6d70 6f6e 656e  turns a Componen
+00015860: 7420 636f 7079 2e0a 0a20 2020 2041 7267  t copy...    Arg
+00015870: 733a 0a20 2020 2020 2020 2044 3a20 636f  s:.        D: co
+00015880: 6d70 6f6e 656e 7420 746f 2063 6f70 792e  mponent to copy.
+00015890: 0a20 2020 2022 2222 0a20 2020 2044 5f63  .    """.    D_c
+000158a0: 6f70 7920 3d20 436f 6d70 6f6e 656e 7428  opy = Component(
+000158b0: 290a 2020 2020 445f 636f 7079 2e69 6e66  ).    D_copy.inf
+000158c0: 6f20 3d20 442e 696e 666f 0a20 2020 2023  o = D.info.    #
+000158d0: 2044 5f63 6f70 792e 5f63 656c 6c20 3d20   D_copy._cell = 
+000158e0: 442e 5f63 656c 6c2e 636f 7079 286e 616d  D._cell.copy(nam
+000158f0: 653d 445f 636f 7079 2e6e 616d 6529 0a0a  e=D_copy.name)..
+00015900: 2020 2020 666f 7220 7265 6620 696e 2072      for ref in r
+00015910: 6566 6572 656e 6365 7320 6966 2072 6566  eferences if ref
+00015920: 6572 656e 6365 7320 6973 206e 6f74 204e  erences is not N
+00015930: 6f6e 6520 656c 7365 2044 2e72 6566 6572  one else D.refer
+00015940: 656e 6365 733a 0a20 2020 2020 2020 2044  ences:.        D
+00015950: 5f63 6f70 792e 6164 6428 636f 7079 5f72  _copy.add(copy_r
+00015960: 6566 6572 656e 6365 2872 6566 2929 0a20  eference(ref)). 
+00015970: 2020 2066 6f72 2070 6f72 7420 696e 2028     for port in (
+00015980: 706f 7274 7320 6966 2070 6f72 7473 2069  ports if ports i
+00015990: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+000159a0: 442e 706f 7274 7329 2e76 616c 7565 7328  D.ports).values(
+000159b0: 293a 0a20 2020 2020 2020 2044 5f63 6f70  ):.        D_cop
+000159c0: 792e 6164 645f 706f 7274 2870 6f72 743d  y.add_port(port=
+000159d0: 706f 7274 290a 2020 2020 666f 7220 706f  port).    for po
+000159e0: 6c79 2069 6e20 706f 6c79 676f 6e73 2069  ly in polygons i
+000159f0: 6620 706f 6c79 676f 6e73 2069 7320 6e6f  f polygons is no
+00015a00: 7420 4e6f 6e65 2065 6c73 6520 442e 706f  t None else D.po
+00015a10: 6c79 676f 6e73 3a0a 2020 2020 2020 2020  lygons:.        
+00015a20: 445f 636f 7079 2e61 6464 5f70 6f6c 7967  D_copy.add_polyg
+00015a30: 6f6e 2870 6f6c 7929 0a20 2020 2066 6f72  on(poly).    for
+00015a40: 2070 6174 6820 696e 2070 6174 6873 2069   path in paths i
+00015a50: 6620 7061 7468 7320 6973 206e 6f74 204e  f paths is not N
+00015a60: 6f6e 6520 656c 7365 2044 2e70 6174 6873  one else D.paths
+00015a70: 3a0a 2020 2020 2020 2020 445f 636f 7079  :.        D_copy
+00015a80: 2e61 6464 2870 6174 6829 0a20 2020 2066  .add(path).    f
+00015a90: 6f72 206c 6162 656c 2069 6e20 6c61 6265  or label in labe
+00015aa0: 6c73 2069 6620 6c61 6265 6c73 2069 7320  ls if labels is 
+00015ab0: 6e6f 7420 4e6f 6e65 2065 6c73 6520 442e  not None else D.
+00015ac0: 6c61 6265 6c73 3a0a 2020 2020 2020 2020  labels:.        
+00015ad0: 445f 636f 7079 2e61 6464 5f6c 6162 656c  D_copy.add_label
+00015ae0: 280a 2020 2020 2020 2020 2020 2020 7465  (.            te
+00015af0: 7874 3d6c 6162 656c 2e74 6578 742c 0a20  xt=label.text,. 
+00015b00: 2020 2020 2020 2020 2020 2070 6f73 6974             posit
+00015b10: 696f 6e3d 6c61 6265 6c2e 6f72 6967 696e  ion=label.origin
+00015b20: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
+00015b30: 7965 723d 286c 6162 656c 2e6c 6179 6572  yer=(label.layer
+00015b40: 2c20 6c61 6265 6c2e 7465 7874 7479 7065  , label.texttype
+00015b50: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00015b60: 2020 6966 206e 616d 6520 6973 206e 6f74    if name is not
+00015b70: 204e 6f6e 653a 0a20 2020 2020 2020 2044   None:.        D
+00015b80: 5f63 6f70 792e 6e61 6d65 203d 206e 616d  _copy.name = nam
+00015b90: 650a 0a20 2020 2072 6574 7572 6e20 445f  e..    return D_
+00015ba0: 636f 7079 0a0a 0a64 6566 2063 6f70 795f  copy...def copy_
+00015bb0: 7265 6665 7265 6e63 6528 0a20 2020 2072  reference(.    r
+00015bc0: 6566 2c0a 2020 2020 7061 7265 6e74 3d4e  ef,.    parent=N
+00015bd0: 6f6e 652c 0a20 2020 2063 6f6c 756d 6e73  one,.    columns
+00015be0: 3d4e 6f6e 652c 0a20 2020 2072 6f77 733d  =None,.    rows=
+00015bf0: 4e6f 6e65 2c0a 2020 2020 7370 6163 696e  None,.    spacin
+00015c00: 673d 4e6f 6e65 2c0a 2020 2020 6f72 6967  g=None,.    orig
+00015c10: 696e 3d4e 6f6e 652c 0a20 2020 2072 6f74  in=None,.    rot
+00015c20: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
+00015c30: 6d61 676e 6966 6963 6174 696f 6e3d 4e6f  magnification=No
+00015c40: 6e65 2c0a 2020 2020 785f 7265 666c 6563  ne,.    x_reflec
+00015c50: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 206e  tion=None,.    n
+00015c60: 616d 653d 4e6f 6e65 2c0a 2020 2020 7631  ame=None,.    v1
+00015c70: 3d4e 6f6e 652c 0a20 2020 2076 323d 4e6f  =None,.    v2=No
+00015c80: 6e65 2c0a 2920 2d3e 2043 6f6d 706f 6e65  ne,.) -> Compone
+00015c90: 6e74 5265 6665 7265 6e63 653a 0a20 2020  ntReference:.   
+00015ca0: 2072 6574 7572 6e20 436f 6d70 6f6e 656e   return Componen
+00015cb0: 7452 6566 6572 656e 6365 280a 2020 2020  tReference(.    
+00015cc0: 2020 2020 636f 6d70 6f6e 656e 743d 7061      component=pa
+00015cd0: 7265 6e74 206f 7220 7265 662e 7061 7265  rent or ref.pare
+00015ce0: 6e74 2c0a 2020 2020 2020 2020 636f 6c75  nt,.        colu
+00015cf0: 6d6e 733d 636f 6c75 6d6e 7320 6f72 2072  mns=columns or r
+00015d00: 6566 2e63 6f6c 756d 6e73 2c0a 2020 2020  ef.columns,.    
+00015d10: 2020 2020 726f 7773 3d72 6f77 7320 6f72      rows=rows or
+00015d20: 2072 6566 2e72 6f77 732c 0a20 2020 2020   ref.rows,.     
+00015d30: 2020 2073 7061 6369 6e67 3d73 7061 6369     spacing=spaci
+00015d40: 6e67 206f 7220 7265 662e 7370 6163 696e  ng or ref.spacin
+00015d50: 672c 0a20 2020 2020 2020 206f 7269 6769  g,.        origi
+00015d60: 6e3d 6f72 6967 696e 206f 7220 7265 662e  n=origin or ref.
+00015d70: 6f72 6967 696e 2c0a 2020 2020 2020 2020  origin,.        
+00015d80: 726f 7461 7469 6f6e 3d72 6f74 6174 696f  rotation=rotatio
+00015d90: 6e20 6f72 2072 6566 2e72 6f74 6174 696f  n or ref.rotatio
+00015da0: 6e2c 0a20 2020 2020 2020 206d 6167 6e69  n,.        magni
+00015db0: 6669 6361 7469 6f6e 3d6d 6167 6e69 6669  fication=magnifi
+00015dc0: 6361 7469 6f6e 206f 7220 7265 662e 6d61  cation or ref.ma
+00015dd0: 676e 6966 6963 6174 696f 6e2c 0a20 2020  gnification,.   
+00015de0: 2020 2020 2078 5f72 6566 6c65 6374 696f       x_reflectio
+00015df0: 6e3d 785f 7265 666c 6563 7469 6f6e 206f  n=x_reflection o
+00015e00: 7220 7265 662e 785f 7265 666c 6563 7469  r ref.x_reflecti
+00015e10: 6f6e 2c0a 2020 2020 2020 2020 6e61 6d65  on,.        name
+00015e20: 3d6e 616d 6520 6f72 2072 6566 2e6e 616d  =name or ref.nam
+00015e30: 652c 0a20 2020 2020 2020 2076 313d 7631  e,.        v1=v1
+00015e40: 206f 7220 7265 662e 7631 2c0a 2020 2020   or ref.v1,.    
+00015e50: 2020 2020 7632 3d76 3220 6f72 2072 6566      v2=v2 or ref
+00015e60: 2e76 322c 0a20 2020 2029 0a0a 0a64 6566  .v2,.    )...def
+00015e70: 2074 6573 745f 6765 745f 6c61 7965 7273   test_get_layers
+00015e80: 2829 202d 3e20 436f 6d70 6f6e 656e 743a  () -> Component:
+00015e90: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
+00015ea0: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
+00015eb0: 2020 6331 203d 2067 662e 636f 6d70 6f6e    c1 = gf.compon
+00015ec0: 656e 7473 2e73 7472 6169 6768 7428 0a20  ents.straight(. 
+00015ed0: 2020 2020 2020 206c 656e 6774 683d 3130         length=10
+00015ee0: 2c0a 2020 2020 2020 2020 7769 6474 683d  ,.        width=
+00015ef0: 302e 352c 0a20 2020 2020 2020 206c 6179  0.5,.        lay
+00015f00: 6572 3d28 322c 2030 292c 0a20 2020 2020  er=(2, 0),.     
+00015f10: 2020 2062 626f 785f 6c61 7965 7273 3d5b     bbox_layers=[
+00015f20: 2831 3131 2c20 3029 5d2c 0a20 2020 2020  (111, 0)],.     
+00015f30: 2020 2062 626f 785f 6f66 6673 6574 733d     bbox_offsets=
+00015f40: 5b33 5d2c 0a20 2020 2020 2020 2077 6974  [3],.        wit
+00015f50: 685f 6262 6f78 3d54 7275 652c 0a20 2020  h_bbox=True,.   
+00015f60: 2020 2020 2063 6c61 6464 696e 675f 6c61       cladding_la
+00015f70: 7965 7273 3d4e 6f6e 652c 0a20 2020 2020  yers=None,.     
+00015f80: 2020 2061 6464 5f70 696e 733d 4e6f 6e65     add_pins=None
+00015f90: 2c0a 2020 2020 2020 2020 6164 645f 6262  ,.        add_bb
+00015fa0: 6f78 3d4e 6f6e 652c 0a20 2020 2029 0a20  ox=None,.    ). 
+00015fb0: 2020 2061 7373 6572 7420 6331 2e67 6574     assert c1.get
+00015fc0: 5f6c 6179 6572 7328 2920 3d3d 207b 2832  _layers() == {(2
+00015fd0: 2c20 3029 2c20 2831 3131 2c20 3029 7d2c  , 0), (111, 0)},
+00015fe0: 2063 312e 6765 745f 6c61 7965 7273 2829   c1.get_layers()
+00015ff0: 0a20 2020 2023 2072 6574 7572 6e20 6331  .    # return c1
+00016000: 0a20 2020 2063 3220 3d20 6331 2e72 656d  .    c2 = c1.rem
+00016010: 6f76 655f 6c61 7965 7273 285b 2831 3131  ove_layers([(111
+00016020: 2c20 3029 5d29 0a20 2020 2061 7373 6572  , 0)]).    asser
+00016030: 7420 6332 2e67 6574 5f6c 6179 6572 7328  t c2.get_layers(
+00016040: 2920 3d3d 207b 2832 2c20 3029 7d2c 2063  ) == {(2, 0)}, c
+00016050: 322e 6765 745f 6c61 7965 7273 2829 0a20  2.get_layers(). 
+00016060: 2020 2072 6574 7572 6e20 6332 0a0a 0a64     return c2...d
+00016070: 6566 205f 6669 6c74 6572 5f70 6f6c 7973  ef _filter_polys
+00016080: 2870 6f6c 7967 6f6e 732c 206c 6179 6572  (polygons, layer
+00016090: 735f 6578 636c 293a 0a20 2020 2072 6574  s_excl):.    ret
+000160a0: 7572 6e20 5b0a 2020 2020 2020 2020 706f  urn [.        po
+000160b0: 6c79 676f 6e0a 2020 2020 2020 2020 666f  lygon.        fo
+000160c0: 7220 706f 6c79 676f 6e2c 206c 6179 6572  r polygon, layer
+000160d0: 2c20 6461 7461 7479 7065 2069 6e20 7a69  , datatype in zi
+000160e0: 7028 0a20 2020 2020 2020 2020 2020 2070  p(.            p
+000160f0: 6f6c 7967 6f6e 732e 706f 6c79 676f 6e73  olygons.polygons
+00016100: 2c20 706f 6c79 676f 6e73 2e6c 6179 6572  , polygons.layer
+00016110: 732c 2070 6f6c 7967 6f6e 732e 6461 7461  s, polygons.data
+00016120: 7479 7065 730a 2020 2020 2020 2020 290a  types.        ).
+00016130: 2020 2020 2020 2020 6966 2028 6c61 7965          if (laye
+00016140: 722c 2064 6174 6174 7970 6529 206e 6f74  r, datatype) not
+00016150: 2069 6e20 6c61 7965 7273 5f65 7863 6c0a   in layers_excl.
+00016160: 2020 2020 5d0a 0a0a 6465 6620 7265 6375      ]...def recu
+00016170: 7273 655f 7374 7275 6374 7572 6573 280a  rse_structures(.
+00016180: 2020 2020 636f 6d70 6f6e 656e 743a 2043      component: C
+00016190: 6f6d 706f 6e65 6e74 2c0a 2020 2020 6967  omponent,.    ig
+000161a0: 6e6f 7265 5f63 6f6d 706f 6e65 6e74 735f  nore_components_
+000161b0: 7072 6566 6978 3a20 4f70 7469 6f6e 616c  prefix: Optional
+000161c0: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
+000161d0: 6e65 2c0a 2020 2020 6967 6e6f 7265 5f66  ne,.    ignore_f
+000161e0: 756e 6374 696f 6e73 5f70 7265 6669 783a  unctions_prefix:
+000161f0: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00016200: 7472 5d5d 203d 204e 6f6e 652c 0a29 202d  tr]] = None,.) -
+00016210: 3e20 4469 6374 5b73 7472 2c20 416e 795d  > Dict[str, Any]
+00016220: 3a0a 2020 2020 2222 2252 6563 7572 7365  :.    """Recurse
+00016230: 2063 6f6d 706f 6e65 6e74 2061 6e64 2063   component and c
+00016240: 6f6d 706f 6e65 6e74 7320 7265 6665 7265  omponents refere
+00016250: 6e63 6573 2072 6563 7572 7369 7665 6c79  nces recursively
+00016260: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00016270: 2020 2020 2063 6f6d 706f 6e65 6e74 3a20       component: 
+00016280: 636f 6d70 6f6e 656e 7420 746f 2072 6563  component to rec
+00016290: 7572 7365 2e0a 2020 2020 2020 2020 6967  urse..        ig
+000162a0: 6e6f 7265 5f63 6f6d 706f 6e65 6e74 735f  nore_components_
+000162b0: 7072 6566 6978 3a20 6c69 7374 206f 6620  prefix: list of 
+000162c0: 7072 6566 6978 2074 6f20 6967 6e6f 7265  prefix to ignore
+000162d0: 2e0a 2020 2020 2020 2020 6967 6e6f 7265  ..        ignore
+000162e0: 5f66 756e 6374 696f 6e73 5f70 7265 6669  _functions_prefi
+000162f0: 783a 206c 6973 7420 6f66 2070 7265 6669  x: list of prefi
+00016300: 7820 746f 2069 676e 6f72 652e 0a20 2020  x to ignore..   
+00016310: 2022 2222 0a20 2020 2069 676e 6f72 655f   """.    ignore_
+00016320: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
+00016330: 203d 2069 676e 6f72 655f 6675 6e63 7469   = ignore_functi
+00016340: 6f6e 735f 7072 6566 6978 206f 7220 5b5d  ons_prefix or []
+00016350: 0a20 2020 2069 676e 6f72 655f 636f 6d70  .    ignore_comp
+00016360: 6f6e 656e 7473 5f70 7265 6669 7820 3d20  onents_prefix = 
+00016370: 6967 6e6f 7265 5f63 6f6d 706f 6e65 6e74  ignore_component
+00016380: 735f 7072 6566 6978 206f 7220 5b5d 0a0a  s_prefix or []..
+00016390: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+000163a0: 2068 6173 6174 7472 2863 6f6d 706f 6e65   hasattr(compone
+000163b0: 6e74 2c20 2266 756e 6374 696f 6e5f 6e61  nt, "function_na
+000163c0: 6d65 2229 0a20 2020 2020 2020 2061 6e64  me").        and
+000163d0: 2063 6f6d 706f 6e65 6e74 2e66 756e 6374   component.funct
+000163e0: 696f 6e5f 6e61 6d65 2069 6e20 6967 6e6f  ion_name in igno
+000163f0: 7265 5f66 756e 6374 696f 6e73 5f70 7265  re_functions_pre
+00016400: 6669 780a 2020 2020 293a 0a20 2020 2020  fix.    ):.     
+00016410: 2020 2072 6574 7572 6e20 7b7d 0a0a 2020     return {}..  
+00016420: 2020 6966 2068 6173 6174 7472 2863 6f6d    if hasattr(com
+00016430: 706f 6e65 6e74 2c20 226e 616d 6522 2920  ponent, "name") 
+00016440: 616e 6420 616e 7928 0a20 2020 2020 2020  and any(.       
+00016450: 2063 6f6d 706f 6e65 6e74 2e6e 616d 652e   component.name.
+00016460: 7374 6172 7473 7769 7468 2869 2920 666f  startswith(i) fo
+00016470: 7220 6920 696e 2069 676e 6f72 655f 636f  r i in ignore_co
+00016480: 6d70 6f6e 656e 7473 5f70 7265 6669 780a  mponents_prefix.
+00016490: 2020 2020 293a 0a20 2020 2020 2020 2072      ):.        r
+000164a0: 6574 7572 6e20 7b7d 0a0a 2020 2020 6f75  eturn {}..    ou
+000164b0: 7470 7574 203d 207b 636f 6d70 6f6e 656e  tput = {componen
+000164c0: 742e 6e61 6d65 3a20 6469 6374 2863 6f6d  t.name: dict(com
+000164d0: 706f 6e65 6e74 2e73 6574 7469 6e67 7329  ponent.settings)
+000164e0: 7d0a 2020 2020 666f 7220 7265 6665 7265  }.    for refere
+000164f0: 6e63 6520 696e 2063 6f6d 706f 6e65 6e74  nce in component
+00016500: 2e72 6566 6572 656e 6365 733a 0a20 2020  .references:.   
+00016510: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00016520: 2020 2020 2020 6973 696e 7374 616e 6365        isinstance
+00016530: 2872 6566 6572 656e 6365 2c20 436f 6d70  (reference, Comp
+00016540: 6f6e 656e 7452 6566 6572 656e 6365 290a  onentReference).
+00016550: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00016560: 7265 6665 7265 6e63 652e 7265 665f 6365  reference.ref_ce
+00016570: 6c6c 2e6e 616d 6520 6e6f 7420 696e 206f  ll.name not in o
+00016580: 7574 7075 740a 2020 2020 2020 2020 293a  utput.        ):
+00016590: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000165a0: 7075 742e 7570 6461 7465 2872 6563 7572  put.update(recur
+000165b0: 7365 5f73 7472 7563 7475 7265 7328 7265  se_structures(re
+000165c0: 6665 7265 6e63 652e 7265 665f 6365 6c6c  ference.ref_cell
+000165d0: 2929 0a0a 2020 2020 7265 7475 726e 206f  ))..    return o
+000165e0: 7574 7075 740a 0a0a 6465 6620 666c 6174  utput...def flat
+000165f0: 7465 6e5f 696e 7661 6c69 645f 7265 6673  ten_invalid_refs
+00016600: 5f72 6563 7572 7369 7665 280a 2020 2020  _recursive(.    
+00016610: 636f 6d70 6f6e 656e 743a 2043 6f6d 706f  component: Compo
+00016620: 6e65 6e74 2c0a 2020 2020 6772 6964 5f73  nent,.    grid_s
+00016630: 697a 653a 204f 7074 696f 6e61 6c5b 666c  ize: Optional[fl
+00016640: 6f61 745d 203d 204e 6f6e 652c 0a20 2020  oat] = None,.   
+00016650: 2075 7064 6174 6564 5f63 6f6d 706f 6e65   updated_compone
+00016660: 6e74 733d 4e6f 6e65 2c0a 2020 2020 7472  nts=None,.    tr
+00016670: 6176 6572 7365 645f 636f 6d70 6f6e 656e  aversed_componen
+00016680: 7473 3d4e 6f6e 652c 0a29 3a0a 2020 2020  ts=None,.):.    
+00016690: 2222 2252 6563 7572 7369 7665 6c79 2066  """Recursively f
+000166a0: 6c61 7474 656e 7320 636f 6d70 6f6e 656e  lattens componen
+000166b0: 7420 7265 6665 7265 6e63 6573 2077 6869  t references whi
+000166c0: 6368 2068 6176 6520 696e 7661 6c69 6420  ch have invalid 
+000166d0: 7472 616e 7366 6f72 6d61 7469 6f6e 7320  transformations 
+000166e0: 2869 2e65 2e20 6e6f 6e2d 3930 2064 6567  (i.e. non-90 deg
+000166f0: 2072 6f74 6174 696f 6e73 206f 7220 7375   rotations or su
+00016700: 622d 6772 6964 2074 7261 6e73 6c61 7469  b-grid translati
+00016710: 6f6e 7329 2061 6e64 2072 6574 7572 6e73  ons) and returns
+00016720: 2061 2063 6f70 7920 6966 2061 6e79 2073   a copy if any s
+00016730: 7562 6365 6c6c 7320 6861 7665 2062 6565  ubcells have bee
+00016740: 6e20 6d6f 6469 6669 6564 2e0a 0a20 2020  n modified...   
+00016750: 2057 4152 4e49 4e47 3a20 7468 6973 2066   WARNING: this f
+00016760: 756e 6374 696f 6e20 7769 6c6c 2070 726f  unction will pro
+00016770: 6475 6365 2073 616d 652d 6e61 6d65 2063  duce same-name c
+00016780: 6f70 6965 7320 6f66 2063 656c 6c73 2e20  opies of cells. 
+00016790: 4974 2069 7320 7374 7269 6374 6c79 206d  It is strictly m
+000167a0: 6561 6e74 2074 6f20 6265 2075 7365 6420  eant to be used 
+000167b0: 6f6e 2077 7269 7465 206f 6620 7468 6520  on write of the 
+000167c0: 4744 5320 6669 6c65 2061 6e64 0a20 2020  GDS file and.   
+000167d0: 2073 686f 756c 6420 6e6f 7420 6265 206d   should not be m
+000167e0: 6978 6564 2077 6974 6820 6f74 6865 7220  ixed with other 
+000167f0: 6365 6c6c 732c 206f 7220 796f 7520 7769  cells, or you wi
+00016800: 6c6c 206c 696b 656c 7920 6578 7065 7269  ll likely experi
+00016810: 656e 6365 2069 7373 7565 7320 7769 7468  ence issues with
+00016820: 2064 7570 6c69 6361 7465 2063 656c 6c73   duplicate cells
+00016830: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00016840: 2020 2020 636f 6d70 6f6e 656e 743a 2074      component: t
+00016850: 6865 2063 6f6d 706f 6e65 6e74 2074 6f20  he component to 
+00016860: 6669 7820 2869 6e20 706c 6163 6529 2e0a  fix (in place)..
+00016870: 2020 2020 2020 2020 6772 6964 5f73 697a          grid_siz
+00016880: 653a 2074 6865 2047 4453 2067 7269 6420  e: the GDS grid 
+00016890: 7369 7a65 2c20 696e 2075 6d2c 2064 6566  size, in um, def
+000168a0: 6175 6c74 7320 746f 2061 6374 6976 6520  aults to active 
+000168b0: 5044 4b2e 6765 745f 6772 6964 5f73 697a  PDK.get_grid_siz
+000168c0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000168d0: 616e 7920 7472 616e 736c 6174 696f 6e73  any translations
+000168e0: 2077 6974 6820 6869 6768 6572 2072 6573   with higher res
+000168f0: 6f6c 7574 696f 6e20 7468 616e 2074 6869  olution than thi
+00016900: 7320 6172 6520 636f 6e73 6964 6572 6564  s are considered
+00016910: 2069 6e76 616c 6964 2e0a 2020 2020 2020   invalid..      
+00016920: 2020 7570 6461 7465 645f 636f 6d70 6f6e    updated_compon
+00016930: 656e 7473 3a20 7468 6520 7275 6e6e 696e  ents: the runnin
+00016940: 6720 6469 6374 696f 6e61 7279 206f 6620  g dictionary of 
+00016950: 636f 6d70 6f6e 656e 7473 2077 6869 6368  components which
+00016960: 2068 6176 6520 6265 656e 206d 6f64 6966   have been modif
+00016970: 6965 6420 6279 2074 6869 7320 7472 616e  ied by this tran
+00016980: 7366 6f72 6d61 7469 6f6e 2e20 5368 6f75  sformation. Shou
+00016990: 6c64 2061 6c77 6179 7320 6265 204e 6f6e  ld always be Non
+000169a0: 652c 2065 7863 6570 7420 666f 7220 7265  e, except for re
+000169b0: 6375 7273 6976 6520 696e 766f 6361 7469  cursive invocati
+000169c0: 6f6e 732e 0a20 2020 2020 2020 2074 7261  ons..        tra
+000169d0: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
+000169e0: 733a 2074 6865 2073 6574 206f 6620 636f  s: the set of co
+000169f0: 6d70 6f6e 656e 7420 6e61 6d65 7320 7768  mponent names wh
+00016a00: 6963 6820 6861 7665 2062 6565 6e20 7472  ich have been tr
+00016a10: 6176 6572 7365 642e 2053 686f 756c 6420  aversed. Should 
+00016a20: 616c 7761 7973 2062 6520 4e6f 6e65 2c20  always be None, 
+00016a30: 6578 6365 7074 2066 6f72 2072 6563 7572  except for recur
+00016a40: 7369 7665 2069 6e76 6f63 6174 696f 6e73  sive invocations
+00016a50: 2e0a 2020 2020 2222 220a 2020 2020 6672  ..    """.    fr
+00016a60: 6f6d 2067 6473 6661 6374 6f72 792e 6465  om gdsfactory.de
+00016a70: 636f 7261 746f 7273 2069 6d70 6f72 7420  corators import 
+00016a80: 6973 5f69 6e76 616c 6964 5f72 6566 0a0a  is_invalid_ref..
+00016a90: 2020 2020 696e 7661 6c69 645f 7265 6673      invalid_refs
+00016aa0: 203d 205b 5d0a 2020 2020 7265 6673 203d   = [].    refs =
+00016ab0: 2063 6f6d 706f 6e65 6e74 2e72 6566 6572   component.refer
+00016ac0: 656e 6365 730a 2020 2020 7375 6263 656c  ences.    subcel
+00016ad0: 6c5f 6d6f 6469 6669 6564 203d 2046 616c  l_modified = Fal
+00016ae0: 7365 0a20 2020 2069 6620 7570 6461 7465  se.    if update
+00016af0: 645f 636f 6d70 6f6e 656e 7473 2069 7320  d_components is 
+00016b00: 4e6f 6e65 3a0a 2020 2020 2020 2020 7570  None:.        up
+00016b10: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
+00016b20: 203d 207b 7d0a 2020 2020 6966 2074 7261   = {}.    if tra
+00016b30: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
+00016b40: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+00016b50: 2020 2074 7261 7665 7273 6564 5f63 6f6d     traversed_com
+00016b60: 706f 6e65 6e74 7320 3d20 7365 7428 290a  ponents = set().
+00016b70: 2020 2020 666f 7220 7265 6620 696e 2072      for ref in r
+00016b80: 6566 733a 0a20 2020 2020 2020 2023 206d  efs:.        # m
+00016b90: 6172 6b20 616e 7920 696e 7661 6c69 6420  ark any invalid 
+00016ba0: 7265 6673 2066 6f72 2066 6c61 7474 656e  refs for flatten
+00016bb0: 696e 670a 2020 2020 2020 2020 2320 6f74  ing.        # ot
+00016bc0: 6865 7277 6973 652c 2063 6865 636b 2069  herwise, check i
+00016bd0: 6620 7468 6572 6520 6172 6520 616e 7920  f there are any 
+00016be0: 6d6f 6469 6669 6564 2063 656c 6c73 2062  modified cells b
+00016bf0: 656e 6561 7468 2028 7765 206e 6565 6420  eneath (we need 
+00016c00: 6e6f 7420 646f 2074 6869 7320 6966 2074  not do this if t
+00016c10: 6865 2072 6566 2077 696c 6c20 6265 2066  he ref will be f
+00016c20: 6c61 7474 656e 6564 2061 6e79 7761 7973  lattened anyways
+00016c30: 290a 2020 2020 2020 2020 6966 2069 735f  ).        if is_
+00016c40: 696e 7661 6c69 645f 7265 6628 7265 662c  invalid_ref(ref,
+00016c50: 2067 7269 645f 7369 7a65 293a 0a20 2020   grid_size):.   
+00016c60: 2020 2020 2020 2020 2069 6e76 616c 6964           invalid
+00016c70: 5f72 6566 732e 6170 7065 6e64 2872 6566  _refs.append(ref
+00016c80: 2e6e 616d 6529 0a20 2020 2020 2020 2065  .name).        e
+00016c90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00016ca0: 2023 206f 7468 6572 7769 7365 2c20 7265   # otherwise, re
+00016cb0: 6375 7273 6976 656c 7920 666c 6174 7465  cursively flatte
+00016cc0: 6e20 7265 6673 2069 6620 7468 6520 7375  n refs if the su
+00016cd0: 6263 656c 6c20 6861 7320 6e6f 7420 616c  bcell has not al
+00016ce0: 7265 6164 7920 6265 656e 2074 7261 7665  ready been trave
+00016cf0: 7273 6564 0a20 2020 2020 2020 2020 2020  rsed.           
+00016d00: 2069 6620 7265 662e 7061 7265 6e74 2e6e   if ref.parent.n
+00016d10: 616d 6520 6e6f 7420 696e 2074 7261 7665  ame not in trave
+00016d20: 7273 6564 5f63 6f6d 706f 6e65 6e74 733a  rsed_components:
+00016d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d40: 2066 6c61 7474 656e 5f69 6e76 616c 6964   flatten_invalid
+00016d50: 5f72 6566 735f 7265 6375 7273 6976 6528  _refs_recursive(
+00016d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d70: 2020 2020 2072 6566 2e70 6172 656e 742c       ref.parent,
+00016d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d90: 2020 2020 2067 7269 645f 7369 7a65 3d67       grid_size=g
+00016da0: 7269 645f 7369 7a65 2c0a 2020 2020 2020  rid_size,.      
+00016db0: 2020 2020 2020 2020 2020 2020 2020 7570                up
+00016dc0: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
+00016dd0: 3d75 7064 6174 6564 5f63 6f6d 706f 6e65  =updated_compone
+00016de0: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
+00016df0: 2020 2020 2020 2020 2074 7261 7665 7273           travers
+00016e00: 6564 5f63 6f6d 706f 6e65 6e74 733d 7472  ed_components=tr
+00016e10: 6176 6572 7365 645f 636f 6d70 6f6e 656e  aversed_componen
+00016e20: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+00016e30: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00016e40: 2020 2320 6e6f 772c 2069 6620 7468 6520    # now, if the 
+00016e50: 7265 6627 7320 6365 6c6c 2062 6565 6e20  ref's cell been 
+00016e60: 6d6f 6469 6669 6564 2c20 6d61 726b 2069  modified, mark i
+00016e70: 7420 6173 2073 7563 680a 2020 2020 2020  t as such.      
+00016e80: 2020 2020 2020 6966 2072 6566 2e70 6172        if ref.par
+00016e90: 656e 742e 6e61 6d65 2069 6e20 7570 6461  ent.name in upda
+00016ea0: 7465 645f 636f 6d70 6f6e 656e 7473 3a0a  ted_components:.
+00016eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ec0: 7375 6263 656c 6c5f 6d6f 6469 6669 6564  subcell_modified
+00016ed0: 203d 2054 7275 650a 2020 2020 6966 2069   = True.    if i
+00016ee0: 6e76 616c 6964 5f72 6566 7320 6f72 2073  nvalid_refs or s
+00016ef0: 7562 6365 6c6c 5f6d 6f64 6966 6965 643a  ubcell_modified:
+00016f00: 0a20 2020 2020 2020 206e 6577 5f63 6f6d  .        new_com
+00016f10: 706f 6e65 6e74 203d 2063 6f6d 706f 6e65  ponent = compone
+00016f20: 6e74 2e63 6f70 7928 290a 2020 2020 2020  nt.copy().      
+00016f30: 2020 6e65 775f 636f 6d70 6f6e 656e 742e    new_component.
+00016f40: 6e61 6d65 203d 2063 6f6d 706f 6e65 6e74  name = component
+00016f50: 2e6e 616d 650a 2020 2020 2020 2020 2320  .name.        # 
+00016f60: 6d61 6b65 2073 7572 6520 616c 6c20 6d6f  make sure all mo
+00016f70: 6469 6669 6564 2063 656c 6c73 2068 6176  dified cells hav
+00016f80: 6520 7468 6569 7220 7265 6665 7265 6e63  e their referenc
+00016f90: 6573 2075 7064 6174 6564 0a20 2020 2020  es updated.     
+00016fa0: 2020 206e 6577 5f72 6566 7320 3d20 6e65     new_refs = ne
+00016fb0: 775f 636f 6d70 6f6e 656e 742e 7265 6665  w_component.refe
+00016fc0: 7265 6e63 6573 2e63 6f70 7928 290a 2020  rences.copy().  
+00016fd0: 2020 2020 2020 666f 7220 7265 6620 696e        for ref in
+00016fe0: 206e 6577 5f72 6566 733a 0a20 2020 2020   new_refs:.     
+00016ff0: 2020 2020 2020 2069 6620 7265 662e 6e61         if ref.na
+00017000: 6d65 2069 6e20 696e 7661 6c69 645f 7265  me in invalid_re
+00017010: 6673 3a0a 2020 2020 2020 2020 2020 2020  fs:.            
+00017020: 2020 2020 6e65 775f 636f 6d70 6f6e 656e      new_componen
+00017030: 742e 666c 6174 7465 6e5f 7265 6665 7265  t.flatten_refere
+00017040: 6e63 6528 7265 6629 0a20 2020 2020 2020  nce(ref).       
+00017050: 2020 2020 2065 6c69 6620 280a 2020 2020       elif (.    
+00017060: 2020 2020 2020 2020 2020 2020 7265 662e              ref.
+00017070: 7061 7265 6e74 2e6e 616d 6520 696e 2075  parent.name in u
+00017080: 7064 6174 6564 5f63 6f6d 706f 6e65 6e74  pdated_component
+00017090: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000170a0: 2020 616e 6420 7265 662e 7061 7265 6e74    and ref.parent
+000170b0: 2069 7320 6e6f 7420 7570 6461 7465 645f   is not updated_
+000170c0: 636f 6d70 6f6e 656e 7473 5b72 6566 2e70  components[ref.p
+000170d0: 6172 656e 742e 6e61 6d65 5d0a 2020 2020  arent.name].    
+000170e0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+000170f0: 2020 2020 2020 2020 2020 2072 6566 2e70             ref.p
+00017100: 6172 656e 7420 3d20 7570 6461 7465 645f  arent = updated_
+00017110: 636f 6d70 6f6e 656e 7473 5b72 6566 2e70  components[ref.p
+00017120: 6172 656e 742e 6e61 6d65 5d0a 2020 2020  arent.name].    
+00017130: 2020 2020 636f 6d70 6f6e 656e 7420 3d20      component = 
+00017140: 6e65 775f 636f 6d70 6f6e 656e 740a 2020  new_component.  
+00017150: 2020 2020 2020 7570 6461 7465 645f 636f        updated_co
+00017160: 6d70 6f6e 656e 7473 5b63 6f6d 706f 6e65  mponents[compone
+00017170: 6e74 2e6e 616d 655d 203d 206e 6577 5f63  nt.name] = new_c
+00017180: 6f6d 706f 6e65 6e74 0a20 2020 2074 7261  omponent.    tra
+00017190: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
+000171a0: 732e 6164 6428 636f 6d70 6f6e 656e 742e  s.add(component.
+000171b0: 6e61 6d65 290a 2020 2020 7265 7475 726e  name).    return
+000171c0: 2063 6f6d 706f 6e65 6e74 0a0a 0a64 6566   component...def
+000171d0: 205f 6368 6563 6b5f 756e 6361 6368 6564   _check_uncached
+000171e0: 5f63 6f6d 706f 6e65 6e74 7328 636f 6d70  _components(comp
+000171f0: 6f6e 656e 742c 206d 6f64 6529 3a0a 2020  onent, mode):.  
+00017200: 2020 7661 6c69 645f 6d6f 6465 7320 3d20    valid_modes = 
+00017210: 5b22 7761 726e 222c 2022 6572 726f 7222  ["warn", "error"
+00017220: 2c20 2269 676e 6f72 6522 5d0a 0a20 2020  , "ignore"]..   
+00017230: 2069 6620 6d6f 6465 203d 3d20 2269 676e   if mode == "ign
+00017240: 6f72 6522 3a0a 2020 2020 2020 2020 7265  ore":.        re
+00017250: 7475 726e 0a20 2020 2065 6c69 6620 6d6f  turn.    elif mo
+00017260: 6465 206e 6f74 2069 6e20 7661 6c69 645f  de not in valid_
+00017270: 6d6f 6465 733a 0a20 2020 2020 2020 2072  modes:.        r
+00017280: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00017290: 0a20 2020 2020 2020 2020 2020 2066 227b  .            f"{
+000172a0: 6d6f 6465 7d20 6973 206e 6f74 2061 2076  mode} is not a v
+000172b0: 616c 6964 2076 616c 7565 2066 6f72 206f  alid value for o
+000172c0: 6e5f 756e 6361 6368 6564 5f63 6f6d 706f  n_uncached_compo
+000172d0: 6e65 6e74 2e20 5472 7920 6f6e 6520 6f66  nent. Try one of
+000172e0: 2074 6865 7365 3a20 7b76 616c 6964 5f6d   these: {valid_m
+000172f0: 6f64 6573 7d2e 220a 2020 2020 2020 2020  odes}.".        
+00017300: 290a 0a20 2020 2066 6f72 2073 7562 5f63  )..    for sub_c
+00017310: 6f6d 706f 6e65 6e74 2069 6e20 636f 6d70  omponent in comp
+00017320: 6f6e 656e 742e 6765 745f 6465 7065 6e64  onent.get_depend
+00017330: 656e 6369 6573 2872 6563 7572 7369 7665  encies(recursive
+00017340: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
+00017350: 6966 206e 6f74 2073 7562 5f63 6f6d 706f  if not sub_compo
+00017360: 6e65 6e74 2e5f 6c6f 636b 6564 3a0a 2020  nent._locked:.  
+00017370: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00017380: 6520 3d20 280a 2020 2020 2020 2020 2020  e = (.          
+00017390: 2020 2020 2020 6622 436f 6d70 6f6e 656e        f"Componen
+000173a0: 7420 7b73 7562 5f63 6f6d 706f 6e65 6e74  t {sub_component
+000173b0: 2e6e 616d 6521 727d 2077 6173 204e 4f54  .name!r} was NOT
+000173c0: 2070 726f 7065 726c 7920 6c6f 636b 6564   properly locked
+000173d0: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
+000173e0: 2020 2020 2259 6f75 206e 6565 6420 746f      "You need to
+000173f0: 2077 7269 7465 2069 7420 696e 746f 2061   write it into a
+00017400: 2066 756e 6374 696f 6e20 7468 6174 2068   function that h
+00017410: 6173 2074 6865 2040 6365 6c6c 2064 6563  as the @cell dec
+00017420: 6f72 6174 6f72 2e22 0a20 2020 2020 2020  orator.".       
+00017430: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00017440: 2020 2069 6620 6d6f 6465 203d 3d20 2277     if mode == "w
+00017450: 6172 6e22 3a0a 2020 2020 2020 2020 2020  arn":.          
+00017460: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+00017470: 6172 6e28 6d65 7373 6167 652c 2055 6e63  arn(message, Unc
+00017480: 6163 6865 6443 6f6d 706f 6e65 6e74 5761  achedComponentWa
+00017490: 726e 696e 6729 0a0a 2020 2020 2020 2020  rning)..        
+000174a0: 2020 2020 656c 6966 206d 6f64 6520 3d3d      elif mode ==
+000174b0: 2022 6572 726f 7222 3a0a 2020 2020 2020   "error":.      
+000174c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000174d0: 556e 6361 6368 6564 436f 6d70 6f6e 656e  UncachedComponen
+000174e0: 7445 7272 6f72 286d 6573 7361 6765 290a  tError(message).
+000174f0: 0a0a 6465 6620 7465 7374 5f73 616d 655f  ..def test_same_
+00017500: 7569 6428 2920 2d3e 204e 6f6e 653a 0a20  uid() -> None:. 
+00017510: 2020 2069 6d70 6f72 7420 6764 7366 6163     import gdsfac
+00017520: 746f 7279 2061 7320 6766 0a0a 2020 2020  tory as gf..    
+00017530: 6320 3d20 436f 6d70 6f6e 656e 7428 290a  c = Component().
+00017540: 2020 2020 6320 3c3c 2067 662e 636f 6d70      c << gf.comp
+00017550: 6f6e 656e 7473 2e72 6563 7461 6e67 6c65  onents.rectangle
+00017560: 2829 0a20 2020 2063 203c 3c20 6766 2e63  ().    c << gf.c
+00017570: 6f6d 706f 6e65 6e74 732e 7265 6374 616e  omponents.rectan
+00017580: 676c 6528 290a 0a20 2020 2072 3120 3d20  gle()..    r1 = 
+00017590: 632e 7265 6665 7265 6e63 6573 5b30 5d2e  c.references[0].
+000175a0: 7061 7265 6e74 0a20 2020 2072 3220 3d20  parent.    r2 = 
+000175b0: 632e 7265 6665 7265 6e63 6573 5b31 5d2e  c.references[1].
+000175c0: 7061 7265 6e74 0a0a 2020 2020 6173 7365  parent..    asse
+000175d0: 7274 2072 312e 7569 6420 3d3d 2072 322e  rt r1.uid == r2.
+000175e0: 7569 642c 2066 227b 7231 2e75 6964 7d20  uid, f"{r1.uid} 
+000175f0: 6d75 7374 2065 7175 616c 207b 7232 2e75  must equal {r2.u
+00017600: 6964 7d22 0a0a 0a64 6566 2074 6573 745f  id}"...def test_
+00017610: 6e65 746c 6973 745f 7369 6d70 6c65 2829  netlist_simple()
+00017620: 202d 3e20 4e6f 6e65 3a0a 2020 2020 696d   -> None:.    im
+00017630: 706f 7274 2067 6473 6661 6374 6f72 7920  port gdsfactory 
+00017640: 6173 2067 660a 0a20 2020 2063 203d 2067  as gf..    c = g
+00017650: 662e 436f 6d70 6f6e 656e 7428 290a 2020  f.Component().  
+00017660: 2020 6331 203d 2063 203c 3c20 6766 2e63    c1 = c << gf.c
+00017670: 6f6d 706f 6e65 6e74 732e 7374 7261 6967  omponents.straig
+00017680: 6874 286c 656e 6774 683d 312c 2077 6964  ht(length=1, wid
+00017690: 7468 3d32 290a 2020 2020 6332 203d 2063  th=2).    c2 = c
+000176a0: 203c 3c20 6766 2e63 6f6d 706f 6e65 6e74   << gf.component
+000176b0: 732e 7374 7261 6967 6874 286c 656e 6774  s.straight(lengt
+000176c0: 683d 322c 2077 6964 7468 3d32 290a 2020  h=2, width=2).  
+000176d0: 2020 6332 2e63 6f6e 6e65 6374 2870 6f72    c2.connect(por
+000176e0: 743d 226f 3122 2c20 6465 7374 696e 6174  t="o1", destinat
+000176f0: 696f 6e3d 6331 2e70 6f72 7473 5b22 6f32  ion=c1.ports["o2
+00017700: 225d 290a 2020 2020 632e 6164 645f 706f  "]).    c.add_po
+00017710: 7274 2822 6f31 222c 2070 6f72 743d 6331  rt("o1", port=c1
+00017720: 2e70 6f72 7473 5b22 6f31 225d 290a 2020  .ports["o1"]).  
+00017730: 2020 632e 6164 645f 706f 7274 2822 6f32    c.add_port("o2
+00017740: 222c 2070 6f72 743d 6332 2e70 6f72 7473  ", port=c2.ports
+00017750: 5b22 6f32 225d 290a 2020 2020 6e65 746c  ["o2"]).    netl
+00017760: 6973 7420 3d20 632e 6765 745f 6e65 746c  ist = c.get_netl
+00017770: 6973 7428 290a 2020 2020 2320 7072 696e  ist().    # prin
+00017780: 7428 6e65 746c 6973 742e 7072 6574 7479  t(netlist.pretty
+00017790: 2829 290a 2020 2020 6173 7365 7274 206c  ()).    assert l
+000177a0: 656e 286e 6574 6c69 7374 5b22 696e 7374  en(netlist["inst
+000177b0: 616e 6365 7322 5d29 203d 3d20 320a 0a0a  ances"]) == 2...
+000177c0: 6465 6620 7465 7374 5f6e 6574 6c69 7374  def test_netlist
+000177d0: 5f73 696d 706c 655f 7769 6474 685f 6d69  _simple_width_mi
+000177e0: 736d 6174 6368 5f74 6872 6f77 735f 6572  smatch_throws_er
+000177f0: 726f 7228 2920 2d3e 204e 6f6e 653a 0a20  ror() -> None:. 
+00017800: 2020 2069 6d70 6f72 7420 7079 7465 7374     import pytest
+00017810: 0a0a 2020 2020 696d 706f 7274 2067 6473  ..    import gds
+00017820: 6661 6374 6f72 7920 6173 2067 660a 0a20  factory as gf.. 
+00017830: 2020 2063 203d 2067 662e 436f 6d70 6f6e     c = gf.Compon
+00017840: 656e 7428 290a 2020 2020 6331 203d 2063  ent().    c1 = c
+00017850: 203c 3c20 6766 2e63 6f6d 706f 6e65 6e74   << gf.component
+00017860: 732e 7374 7261 6967 6874 286c 656e 6774  s.straight(lengt
+00017870: 683d 312c 2077 6964 7468 3d31 290a 2020  h=1, width=1).  
+00017880: 2020 6332 203d 2063 203c 3c20 6766 2e63    c2 = c << gf.c
+00017890: 6f6d 706f 6e65 6e74 732e 7374 7261 6967  omponents.straig
+000178a0: 6874 286c 656e 6774 683d 322c 2077 6964  ht(length=2, wid
+000178b0: 7468 3d32 290a 2020 2020 6332 2e63 6f6e  th=2).    c2.con
+000178c0: 6e65 6374 2870 6f72 743d 226f 3122 2c20  nect(port="o1", 
+000178d0: 6465 7374 696e 6174 696f 6e3d 6331 2e70  destination=c1.p
+000178e0: 6f72 7473 5b22 6f32 225d 290a 2020 2020  orts["o2"]).    
+000178f0: 632e 6164 645f 706f 7274 2822 6f31 222c  c.add_port("o1",
+00017900: 2070 6f72 743d 6331 2e70 6f72 7473 5b22   port=c1.ports["
+00017910: 6f31 225d 290a 2020 2020 632e 6164 645f  o1"]).    c.add_
+00017920: 706f 7274 2822 6f32 222c 2070 6f72 743d  port("o2", port=
+00017930: 6332 2e70 6f72 7473 5b22 6f32 225d 290a  c2.ports["o2"]).
+00017940: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
+00017950: 7261 6973 6573 2856 616c 7565 4572 726f  raises(ValueErro
+00017960: 7229 3a0a 2020 2020 2020 2020 632e 6765  r):.        c.ge
+00017970: 745f 6e65 746c 6973 7428 290a 0a0a 6465  t_netlist()...de
+00017980: 6620 7465 7374 5f6e 6574 6c69 7374 5f63  f test_netlist_c
+00017990: 6f6d 706c 6578 2829 202d 3e20 4e6f 6e65  omplex() -> None
+000179a0: 3a0a 2020 2020 696d 706f 7274 2067 6473  :.    import gds
+000179b0: 6661 6374 6f72 7920 6173 2067 660a 0a20  factory as gf.. 
+000179c0: 2020 2063 203d 2067 662e 636f 6d70 6f6e     c = gf.compon
+000179d0: 656e 7473 2e6d 7a69 5f61 726d 7328 290a  ents.mzi_arms().
+000179e0: 2020 2020 6e65 746c 6973 7420 3d20 632e      netlist = c.
+000179f0: 6765 745f 6e65 746c 6973 7428 290a 2020  get_netlist().  
+00017a00: 2020 2320 7072 696e 7428 6e65 746c 6973    # print(netlis
+00017a10: 742e 7072 6574 7479 2829 290a 2020 2020  t.pretty()).    
+00017a20: 6173 7365 7274 206c 656e 286e 6574 6c69  assert len(netli
+00017a30: 7374 5b22 696e 7374 616e 6365 7322 5d29  st["instances"])
+00017a40: 203d 3d20 342c 206c 656e 286e 6574 6c69   == 4, len(netli
+00017a50: 7374 5b22 696e 7374 616e 6365 7322 5d29  st["instances"])
+00017a60: 0a0a 0a64 6566 2074 6573 745f 6578 7472  ...def test_extr
+00017a70: 6163 7428 2920 2d3e 2043 6f6d 706f 6e65  act() -> Compone
+00017a80: 6e74 3a0a 2020 2020 696d 706f 7274 2067  nt:.    import g
+00017a90: 6473 6661 6374 6f72 7920 6173 2067 660a  dsfactory as gf.
+00017aa0: 0a20 2020 2063 203d 2067 662e 636f 6d70  .    c = gf.comp
+00017ab0: 6f6e 656e 7473 2e73 7472 6169 6768 7428  onents.straight(
+00017ac0: 0a20 2020 2020 2020 206c 656e 6774 683d  .        length=
+00017ad0: 3130 2c0a 2020 2020 2020 2020 7769 6474  10,.        widt
+00017ae0: 683d 302e 352c 0a20 2020 2020 2020 2062  h=0.5,.        b
+00017af0: 626f 785f 6c61 7965 7273 3d5b 6766 2e4c  box_layers=[gf.L
+00017b00: 4159 4552 2e57 4743 4c41 445d 2c0a 2020  AYER.WGCLAD],.  
+00017b10: 2020 2020 2020 6262 6f78 5f6f 6666 7365        bbox_offse
+00017b20: 7473 3d5b 335d 2c0a 2020 2020 2020 2020  ts=[3],.        
+00017b30: 7769 7468 5f62 626f 783d 5472 7565 2c0a  with_bbox=True,.
+00017b40: 2020 2020 2020 2020 636c 6164 6469 6e67          cladding
+00017b50: 5f6c 6179 6572 733d 4e6f 6e65 2c0a 2020  _layers=None,.  
+00017b60: 2020 2020 2020 6164 645f 7069 6e73 3d4e        add_pins=N
+00017b70: 6f6e 652c 0a20 2020 2020 2020 2061 6464  one,.        add
+00017b80: 5f62 626f 783d 4e6f 6e65 2c0a 2020 2020  _bbox=None,.    
+00017b90: 290a 2020 2020 6332 203d 2063 2e65 7874  ).    c2 = c.ext
+00017ba0: 7261 6374 286c 6179 6572 733d 5b67 662e  ract(layers=[gf.
+00017bb0: 4c41 5945 522e 5747 434c 4144 5d29 0a0a  LAYER.WGCLAD])..
+00017bc0: 2020 2020 6173 7365 7274 206c 656e 2863      assert len(c
+00017bd0: 2e70 6f6c 7967 6f6e 7329 203d 3d20 322c  .polygons) == 2,
+00017be0: 206c 656e 2863 2e70 6f6c 7967 6f6e 7329   len(c.polygons)
+00017bf0: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
+00017c00: 6332 2e70 6f6c 7967 6f6e 7329 203d 3d20  c2.polygons) == 
+00017c10: 312c 206c 656e 2863 322e 706f 6c79 676f  1, len(c2.polygo
+00017c20: 6e73 290a 2020 2020 6173 7365 7274 2067  ns).    assert g
+00017c30: 662e 4c41 5945 522e 5747 434c 4144 2069  f.LAYER.WGCLAD i
+00017c40: 6e20 6332 2e6c 6179 6572 730a 2020 2020  n c2.layers.    
+00017c50: 7265 7475 726e 2063 320a 0a0a 6465 6620  return c2...def 
+00017c60: 6861 7368 5f66 696c 6528 6669 6c65 7061  hash_file(filepa
+00017c70: 7468 293a 0a20 2020 206d 6435 203d 2068  th):.    md5 = h
+00017c80: 6173 686c 6962 2e6d 6435 2829 0a20 2020  ashlib.md5().   
+00017c90: 206d 6435 2e75 7064 6174 6528 6669 6c65   md5.update(file
+00017ca0: 7061 7468 2e72 6561 645f 6279 7465 7328  path.read_bytes(
+00017cb0: 2929 0a20 2020 2072 6574 7572 6e20 6d64  )).    return md
+00017cc0: 352e 6865 7864 6967 6573 7428 290a 0a0a  5.hexdigest()...
+00017cd0: 6465 6620 7465 7374 5f62 626f 785f 7265  def test_bbox_re
+00017ce0: 6665 7265 6e63 6528 2920 2d3e 2043 6f6d  ference() -> Com
+00017cf0: 706f 6e65 6e74 3a0a 2020 2020 696d 706f  ponent:.    impo
+00017d00: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
+00017d10: 2067 660a 0a20 2020 2063 203d 2067 662e   gf..    c = gf.
+00017d20: 436f 6d70 6f6e 656e 7428 2263 6f6d 706f  Component("compo
+00017d30: 6e65 6e74 5f77 6974 685f 6f66 6667 7269  nent_with_offgri
+00017d40: 645f 706f 6c79 676f 6e73 2229 0a20 2020  d_polygons").   
+00017d50: 2063 3120 3d20 6320 3c3c 2067 662e 636f   c1 = c << gf.co
+00017d60: 6d70 6f6e 656e 7473 2e72 6563 7461 6e67  mponents.rectang
+00017d70: 6c65 2873 697a 653d 2831 2e35 652d 332c  le(size=(1.5e-3,
+00017d80: 2031 2e35 652d 3329 2c20 706f 7274 5f74   1.5e-3), port_t
+00017d90: 7970 653d 4e6f 6e65 290a 2020 2020 6332  ype=None).    c2
+00017da0: 203d 2063 203c 3c20 6766 2e63 6f6d 706f   = c << gf.compo
+00017db0: 6e65 6e74 732e 7265 6374 616e 676c 6528  nents.rectangle(
+00017dc0: 7369 7a65 3d28 312e 3565 2d33 2c20 312e  size=(1.5e-3, 1.
+00017dd0: 3565 2d33 292c 2070 6f72 745f 7479 7065  5e-3), port_type
+00017de0: 3d4e 6f6e 6529 0a20 2020 2063 322e 786d  =None).    c2.xm
+00017df0: 696e 203d 2063 312e 786d 6178 0a0a 2020  in = c1.xmax..  
+00017e00: 2020 6173 7365 7274 2063 322e 7873 697a    assert c2.xsiz
+00017e10: 6520 3d3d 2032 652d 330a 2020 2020 7265  e == 2e-3.    re
+00017e20: 7475 726e 2063 320a 0a0a 6465 6620 7465  turn c2...def te
+00017e30: 7374 5f62 626f 785f 636f 6d70 6f6e 656e  st_bbox_componen
+00017e40: 7428 2920 2d3e 204e 6f6e 653a 0a20 2020  t() -> None:.   
+00017e50: 2069 6d70 6f72 7420 6764 7366 6163 746f   import gdsfacto
+00017e60: 7279 2061 7320 6766 0a0a 2020 2020 6320  ry as gf..    c 
+00017e70: 3d20 6766 2e63 6f6d 706f 6e65 6e74 732e  = gf.components.
+00017e80: 7265 6374 616e 676c 6528 7369 7a65 3d28  rectangle(size=(
+00017e90: 312e 3565 2d33 2c20 312e 3565 2d33 292c  1.5e-3, 1.5e-3),
+00017ea0: 2070 6f72 745f 7479 7065 3d4e 6f6e 6529   port_type=None)
+00017eb0: 0a20 2020 2061 7373 6572 7420 632e 7873  .    assert c.xs
+00017ec0: 697a 6520 3d3d 2032 652d 330a 0a0a 6465  ize == 2e-3...de
+00017ed0: 6620 7465 7374 5f72 656d 6170 5f6c 6179  f test_remap_lay
+00017ee0: 6572 7328 2920 2d3e 204e 6f6e 653a 0a20  ers() -> None:. 
+00017ef0: 2020 2069 6d70 6f72 7420 6764 7366 6163     import gdsfac
+00017f00: 746f 7279 2061 7320 6766 0a0a 2020 2020  tory as gf..    
+00017f10: 6320 3d20 6766 2e63 6f6d 706f 6e65 6e74  c = gf.component
+00017f20: 732e 7374 7261 6967 6874 286c 6179 6572  s.straight(layer
+00017f30: 3d28 322c 2030 2929 0a20 2020 2072 656d  =(2, 0)).    rem
+00017f40: 6170 203d 2063 2e72 656d 6170 5f6c 6179  ap = c.remap_lay
+00017f50: 6572 7328 6c61 7965 726d 6170 3d7b 2832  ers(layermap={(2
+00017f60: 2c20 3029 3a20 6766 2e4c 4159 4552 2e57  , 0): gf.LAYER.W
+00017f70: 474e 7d29 0a20 2020 2068 6173 685f 6765  GN}).    hash_ge
+00017f80: 6f6d 6574 7279 203d 2022 3833 6662 6336  ometry = "83fbc6
+00017f90: 6138 3238 3935 3035 6561 6564 3361 3265  a8289505eaed3a2e
+00017fa0: 3361 6232 3739 6363 3033 6635 6534 6430  3ab279cc03f5e4d0
+00017fb0: 3063 220a 0a20 2020 2061 7373 6572 7420  0c"..    assert 
+00017fc0: 280a 2020 2020 2020 2020 7265 6d61 702e  (.        remap.
+00017fd0: 6861 7368 5f67 656f 6d65 7472 7928 2920  hash_geometry() 
+00017fe0: 3d3d 2068 6173 685f 6765 6f6d 6574 7279  == hash_geometry
+00017ff0: 0a20 2020 2029 2c20 6622 6861 7368 5f67  .    ), f"hash_g
+00018000: 656f 6d65 7472 7920 3d20 7b72 656d 6170  eometry = {remap
+00018010: 2e68 6173 685f 6765 6f6d 6574 7279 2829  .hash_geometry()
+00018020: 2172 7d22 0a0a 0a64 6566 2074 6573 745f  !r}"...def test_
+00018030: 7265 6d6f 7665 5f6c 6162 656c 7328 2920  remove_labels() 
+00018040: 2d3e 204e 6f6e 653a 0a20 2020 2069 6d70  -> None:.    imp
+00018050: 6f72 7420 6764 7366 6163 746f 7279 2061  ort gdsfactory a
+00018060: 7320 6766 0a0a 2020 2020 6320 3d20 6766  s gf..    c = gf
+00018070: 2e63 2e73 7472 6169 6768 7428 290a 2020  .c.straight().  
+00018080: 2020 632e 7265 6d6f 7665 5f6c 6162 656c    c.remove_label
+00018090: 7328 290a 0a20 2020 2061 7373 6572 7420  s()..    assert 
+000180a0: 6c65 6e28 632e 6c61 6265 6c73 2920 3d3d  len(c.labels) ==
+000180b0: 2030 0a0a 0a64 6566 2074 6573 745f 696d   0...def test_im
+000180c0: 706f 7274 5f67 6473 5f73 6574 7469 6e67  port_gds_setting
+000180d0: 7328 293a 0a20 2020 2069 6d70 6f72 7420  s():.    import 
+000180e0: 6764 7366 6163 746f 7279 2061 7320 6766  gdsfactory as gf
+000180f0: 0a0a 2020 2020 6320 3d20 6766 2e63 6f6d  ..    c = gf.com
+00018100: 706f 6e65 6e74 732e 6d7a 6928 290a 2020  ponents.mzi().  
+00018110: 2020 6764 7370 6174 6820 3d20 632e 7772    gdspath = c.wr
+00018120: 6974 655f 6764 735f 7769 7468 5f6d 6574  ite_gds_with_met
+00018130: 6164 6174 6128 290a 2020 2020 6332 203d  adata().    c2 =
+00018140: 2067 662e 696d 706f 7274 5f67 6473 2867   gf.import_gds(g
+00018150: 6473 7061 7468 2c20 6e61 6d65 3d22 6d7a  dspath, name="mz
+00018160: 695f 7361 6d70 6c65 222c 2072 6561 645f  i_sample", read_
+00018170: 6d65 7461 6461 7461 3d54 7275 6529 0a20  metadata=True). 
+00018180: 2020 2063 3320 3d20 6766 2e72 6f75 7469     c3 = gf.routi
+00018190: 6e67 2e61 6464 5f66 6962 6572 5f73 696e  ng.add_fiber_sin
+000181a0: 676c 6528 6332 290a 2020 2020 6173 7365  gle(c2).    asse
+000181b0: 7274 2063 330a 0a0a 6465 6620 7465 7374  rt c3...def test
+000181c0: 5f66 6c61 7474 656e 5f69 6e76 616c 6964  _flatten_invalid
+000181d0: 5f72 6566 735f 7265 6375 7273 6976 6528  _refs_recursive(
+000181e0: 293a 0a20 2020 2069 6d70 6f72 7420 6764  ):.    import gd
+000181f0: 7366 6163 746f 7279 2061 7320 6766 0a20  sfactory as gf. 
+00018200: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
+00018210: 7279 2e64 6966 6674 6573 7420 696d 706f  ry.difftest impo
+00018220: 7274 2072 756e 5f78 6f72 0a20 2020 2066  rt run_xor.    f
+00018230: 726f 6d20 6764 7366 6163 746f 7279 2e72  rom gdsfactory.r
+00018240: 6f75 7469 6e67 2e61 6c6c 5f61 6e67 6c65  outing.all_angle
+00018250: 2069 6d70 6f72 7420 6765 745f 6275 6e64   import get_bund
+00018260: 6c65 5f61 6c6c 5f61 6e67 6c65 0a0a 2020  le_all_angle..  
+00018270: 2020 4067 662e 6365 6c6c 0a20 2020 2064    @gf.cell.    d
+00018280: 6566 2066 6c61 7428 293a 0a20 2020 2020  ef flat():.     
+00018290: 2020 2063 203d 2067 662e 436f 6d70 6f6e     c = gf.Compon
+000182a0: 656e 7428 290a 2020 2020 2020 2020 6d6d  ent().        mm
+000182b0: 6931 203d 2028 6320 3c3c 2067 662e 636f  i1 = (c << gf.co
+000182c0: 6d70 6f6e 656e 7473 2e6d 6d69 3178 3228  mponents.mmi1x2(
+000182d0: 2929 2e6d 6f76 6528 2830 2c20 2d31 2e30  )).move((0, -1.0
+000182e0: 3030 3529 290a 2020 2020 2020 2020 6d6d  005)).        mm
+000182f0: 6932 203d 2028 6320 3c3c 2067 662e 636f  i2 = (c << gf.co
+00018300: 6d70 6f6e 656e 7473 2e6d 6d69 3178 3228  mponents.mmi1x2(
+00018310: 2929 2e72 6f74 6174 6528 3830 290a 2020  )).rotate(80).  
+00018320: 2020 2020 2020 6d6d 6932 2e6d 6f76 6528        mmi2.move(
+00018330: 2834 302c 2032 3029 290a 2020 2020 2020  (40, 20)).      
+00018340: 2020 6275 6e64 6c65 203d 2067 6574 5f62    bundle = get_b
+00018350: 756e 646c 655f 616c 6c5f 616e 676c 6528  undle_all_angle(
+00018360: 5b6d 6d69 312e 706f 7274 735b 226f 3222  [mmi1.ports["o2"
+00018370: 5d5d 2c20 5b6d 6d69 322e 706f 7274 735b  ]], [mmi2.ports[
+00018380: 226f 3122 5d5d 290a 2020 2020 2020 2020  "o1"]]).        
+00018390: 666f 7220 726f 7574 6520 696e 2062 756e  for route in bun
+000183a0: 646c 653a 0a20 2020 2020 2020 2020 2020  dle:.           
+000183b0: 2063 2e61 6464 2872 6f75 7465 2e72 6566   c.add(route.ref
+000183c0: 6572 656e 6365 7329 0a20 2020 2020 2020  erences).       
+000183d0: 2072 6574 7572 6e20 630a 0a20 2020 2040   return c..    @
+000183e0: 6766 2e63 656c 6c0a 2020 2020 6465 6620  gf.cell.    def 
+000183f0: 6869 6572 6172 6368 7928 293a 0a20 2020  hierarchy():.   
+00018400: 2020 2020 2063 203d 2067 662e 436f 6d70       c = gf.Comp
+00018410: 6f6e 656e 7428 290a 2020 2020 2020 2020  onent().        
+00018420: 2863 203c 3c20 666c 6174 2829 292e 726f  (c << flat()).ro
+00018430: 7461 7465 2833 3329 0a20 2020 2020 2020  tate(33).       
+00018440: 2028 6320 3c3c 2066 6c61 7428 2929 2e72   (c << flat()).r
+00018450: 6f74 6174 6528 3333 292e 6d6f 7665 2828  otate(33).move((
+00018460: 302c 2031 3030 2929 0a20 2020 2020 2020  0, 100)).       
+00018470: 2028 6320 3c3c 2066 6c61 7428 2929 2e6d   (c << flat()).m
+00018480: 6f76 6528 2831 3030 2c20 3029 290a 2020  ove((100, 0)).  
+00018490: 2020 2020 2020 7265 7475 726e 2063 0a0a        return c..
+000184a0: 2020 2020 635f 6f72 6967 203d 2068 6965      c_orig = hie
+000184b0: 7261 7263 6879 2829 0a20 2020 2063 5f6e  rarchy().    c_n
+000184c0: 6577 203d 2066 6c61 7474 656e 5f69 6e76  ew = flatten_inv
+000184d0: 616c 6964 5f72 6566 735f 7265 6375 7273  alid_refs_recurs
+000184e0: 6976 6528 635f 6f72 6967 290a 2020 2020  ive(c_orig).    
+000184f0: 6173 7365 7274 2063 5f6e 6577 2069 7320  assert c_new is 
+00018500: 6e6f 7420 635f 6f72 6967 0a20 2020 2069  not c_orig.    i
+00018510: 6e76 616c 6964 5f72 6566 735f 6669 6c65  nvalid_refs_file
+00018520: 6e61 6d65 203d 2022 696e 7661 6c69 645f  name = "invalid_
+00018530: 7265 6673 2e67 6473 220a 2020 2020 696e  refs.gds".    in
+00018540: 7661 6c69 645f 7265 6673 5f66 6978 6564  valid_refs_fixed
+00018550: 5f66 696c 656e 616d 6520 3d20 2269 6e76  _filename = "inv
+00018560: 616c 6964 5f72 6566 735f 6669 7865 642e  alid_refs_fixed.
+00018570: 6764 7322 0a20 2020 2023 2067 6473 2066  gds".    # gds f
+00018580: 696c 6573 2073 686f 756c 6420 7374 696c  iles should stil
+00018590: 6c20 6265 2073 616d 6520 746f 2031 6e6d  l be same to 1nm
+000185a0: 2074 6f6c 6572 616e 6365 0a20 2020 2063   tolerance.    c
+000185b0: 5f6f 7269 672e 7772 6974 655f 6764 7328  _orig.write_gds(
+000185c0: 696e 7661 6c69 645f 7265 6673 5f66 696c  invalid_refs_fil
+000185d0: 656e 616d 6529 0a20 2020 2063 5f6e 6577  ename).    c_new
+000185e0: 2e77 7269 7465 5f67 6473 2869 6e76 616c  .write_gds(inval
+000185f0: 6964 5f72 6566 735f 6669 7865 645f 6669  id_refs_fixed_fi
+00018600: 6c65 6e61 6d65 290a 2020 2020 7275 6e5f  lename).    run_
+00018610: 786f 7228 696e 7661 6c69 645f 7265 6673  xor(invalid_refs
+00018620: 5f66 696c 656e 616d 652c 2069 6e76 616c  _filename, inval
+00018630: 6964 5f72 6566 735f 6669 7865 645f 6669  id_refs_fixed_fi
+00018640: 6c65 6e61 6d65 290a 0a0a 6966 205f 5f6e  lename)...if __n
+00018650: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+00018660: 5f5f 223a 0a20 2020 2069 6d70 6f72 7420  __":.    import 
+00018670: 6764 7366 6163 746f 7279 2061 7320 6766  gdsfactory as gf
+00018680: 0a0a 2020 2020 6320 3d20 6766 2e43 6f6d  ..    c = gf.Com
+00018690: 706f 6e65 6e74 2829 0a20 2020 2070 203d  ponent().    p =
+000186a0: 2063 2e61 6464 5f70 6f6c 7967 6f6e 280a   c.add_polygon(.
+000186b0: 2020 2020 2020 2020 5b28 2d38 2c20 362c          [(-8, 6,
+000186c0: 2037 2c20 3929 2c20 282d 362c 2038 2c20   7, 9), (-6, 8, 
+000186d0: 3137 2c20 3529 5d2c 206c 6179 6572 3d28  17, 5)], layer=(
+000186e0: 312c 2030 290a 2020 2020 2920 2023 2047  1, 0).    )  # G
+000186f0: 4453 206c 6179 6572 7320 6172 6520 7475  DS layers are tu
+00018700: 706c 6573 206f 6620 696e 7473 2028 6275  ples of ints (bu
+00018710: 7420 6966 2077 6520 7573 6520 6f6e 6c79  t if we use only
+00018720: 206f 6e65 206e 756d 6265 7220 6974 2061   one number it a
+00018730: 7373 756d 6573 2074 6865 206f 7468 6572  ssumes the other
+00018740: 206e 756d 6265 7220 6973 2030 290a 0a20   number is 0).. 
+00018750: 2020 2023 2063 3220 3d20 6766 2e43 6f6d     # c2 = gf.Com
+00018760: 706f 6e65 6e74 2829 0a20 2020 2023 2063  ponent().    # c
+00018770: 203d 2067 662e 636f 6d70 6f6e 656e 7473   = gf.components
+00018780: 2e6d 7a69 2829 0a20 2020 2023 2070 7269  .mzi().    # pri
+00018790: 6e74 2863 2e67 6574 5f6c 6179 6572 5f6e  nt(c.get_layer_n
+000187a0: 616d 6573 2829 290a 2020 2020 2320 7220  ames()).    # r 
+000187b0: 3d20 632e 7265 6628 290a 2020 2020 2320  = c.ref().    # 
+000187c0: 6332 2e63 6f70 795f 6368 696c 645f 696e  c2.copy_child_in
+000187d0: 666f 2863 2e6e 616d 6564 5f72 6566 6572  fo(c.named_refer
+000187e0: 656e 6365 735b 2273 7874 225d 290a 2020  ences["sxt"]).  
+000187f0: 2020 2320 7465 7374 5f72 656d 6170 5f6c    # test_remap_l
+00018800: 6179 6572 7328 290a 2020 2020 2320 6320  ayers().    # c 
+00018810: 3d20 7465 7374 5f67 6574 5f6c 6179 6572  = test_get_layer
+00018820: 7328 290a 2020 2020 2320 632e 706c 6f74  s().    # c.plot
+00018830: 5f71 7428 290a 2020 2020 2320 632e 706c  _qt().    # c.pl
+00018840: 6f74 6828 290a 2020 2020 2320 6320 3d20  oth().    # c = 
+00018850: 7465 7374 5f65 7874 7261 6374 2829 0a20  test_extract(). 
+00018860: 2020 2023 2067 6473 7061 7468 203d 2063     # gdspath = c
+00018870: 2e77 7269 7465 5f67 6473 2829 0a20 2020  .write_gds().   
+00018880: 2023 2067 662e 7368 6f77 2867 6473 7061   # gf.show(gdspa
+00018890: 7468 290a 2020 2020 2320 632e 7368 6f77  th).    # c.show
+000188a0: 2873 686f 775f 706f 7274 733d 5472 7565  (show_ports=True
+000188b0: 290a 2020 2020 632e 7368 6f77 2829 0a    ).    c.show().
```

### Comparing `gdsfactory-6.92.2/gdsfactory/component_layout.py` & `gdsfactory-6.93.0/gdsfactory/component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/component_reference.py` & `gdsfactory-6.93.0/gdsfactory/component_reference.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/C.py` & `gdsfactory-6.93.0/gdsfactory/components/C.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/L.py` & `gdsfactory-6.93.0/gdsfactory/components/L.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/__init__.py` & `gdsfactory-6.93.0/gdsfactory/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/add_fiducials.py` & `gdsfactory-6.93.0/gdsfactory/components/add_fiducials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/add_grating_couplers.py` & `gdsfactory-6.93.0/gdsfactory/components/add_grating_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/add_trenches.py` & `gdsfactory-6.93.0/gdsfactory/components/add_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/align.py` & `gdsfactory-6.93.0/gdsfactory/components/align.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/array_component.py` & `gdsfactory-6.93.0/gdsfactory/components/array_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/array_with_fanout.py` & `gdsfactory-6.93.0/gdsfactory/components/array_with_fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/array_with_via.py` & `gdsfactory-6.93.0/gdsfactory/components/array_with_via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/awg.py` & `gdsfactory-6.93.0/gdsfactory/components/awg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/bbox.py` & `gdsfactory-6.93.0/gdsfactory/components/bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/bend_circular.py` & `gdsfactory-6.93.0/gdsfactory/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/bend_circular_heater.py` & `gdsfactory-6.93.0/gdsfactory/components/bend_circular_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/bend_euler.py` & `gdsfactory-6.93.0/gdsfactory/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/bend_port.py` & `gdsfactory-6.93.0/gdsfactory/components/bend_port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/bend_s.py` & `gdsfactory-6.93.0/gdsfactory/components/bend_s.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/bezier.py` & `gdsfactory-6.93.0/gdsfactory/components/bezier.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cavity.py` & `gdsfactory-6.93.0/gdsfactory/components/cavity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cdc.py` & `gdsfactory-6.93.0/gdsfactory/components/cdc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cdsem_all.py` & `gdsfactory-6.93.0/gdsfactory/components/cdsem_all.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cdsem_bend180.py` & `gdsfactory-6.93.0/gdsfactory/components/cdsem_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cdsem_coupler.py` & `gdsfactory-6.93.0/gdsfactory/components/cdsem_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cdsem_straight.py` & `gdsfactory-6.93.0/gdsfactory/components/cdsem_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cdsem_straight_density.py` & `gdsfactory-6.93.0/gdsfactory/components/cdsem_straight_density.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/circle.py` & `gdsfactory-6.93.0/gdsfactory/components/circle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coh_rx_dual_pol.py` & `gdsfactory-6.93.0/gdsfactory/components/coh_rx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coh_rx_single_pol.py` & `gdsfactory-6.93.0/gdsfactory/components/coh_rx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coh_tx_dual_pol.py` & `gdsfactory-6.93.0/gdsfactory/components/coh_tx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coh_tx_single_pol.py` & `gdsfactory-6.93.0/gdsfactory/components/coh_tx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/compass.py` & `gdsfactory-6.93.0/gdsfactory/components/compass.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/component_lattice.py` & `gdsfactory-6.93.0/gdsfactory/components/component_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/component_sequence.py` & `gdsfactory-6.93.0/gdsfactory/components/component_sequence.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/copy_layers.py` & `gdsfactory-6.93.0/gdsfactory/components/copy_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler90.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler90.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler90bend.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler90bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler_adiabatic.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler_asymmetric.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler_full.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler_full.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler_ring.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler_straight.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler_straight_asymmetric.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler_straight_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/coupler_symmetric.py` & `gdsfactory-6.93.0/gdsfactory/components/coupler_symmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cross.py` & `gdsfactory-6.93.0/gdsfactory/components/cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/crossing_waveguide.py` & `gdsfactory-6.93.0/gdsfactory/components/crossing_waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv` & `gdsfactory-6.93.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv` & `gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv` & `gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv` & `gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv` & `gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv` & `gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv` & `gdsfactory-6.93.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cutback_2x2.py` & `gdsfactory-6.93.0/gdsfactory/components/cutback_2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cutback_bend.py` & `gdsfactory-6.93.0/gdsfactory/components/cutback_bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cutback_component.py` & `gdsfactory-6.93.0/gdsfactory/components/cutback_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/cutback_splitter.py` & `gdsfactory-6.93.0/gdsfactory/components/cutback_splitter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/dbr.py` & `gdsfactory-6.93.0/gdsfactory/components/dbr.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/dbr_tapered.py` & `gdsfactory-6.93.0/gdsfactory/components/dbr_tapered.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/delay_snake.py` & `gdsfactory-6.93.0/gdsfactory/components/delay_snake.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/delay_snake2.py` & `gdsfactory-6.93.0/gdsfactory/components/delay_snake2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/delay_snake3.py` & `gdsfactory-6.93.0/gdsfactory/components/delay_snake3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/delay_snake_sbend.py` & `gdsfactory-6.93.0/gdsfactory/components/delay_snake_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/dicing_lane.py` & `gdsfactory-6.93.0/gdsfactory/components/dicing_lane.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/die.py` & `gdsfactory-6.93.0/gdsfactory/components/die.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/die_bbox.py` & `gdsfactory-6.93.0/gdsfactory/components/die_bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/die_bbox_frame.py` & `gdsfactory-6.93.0/gdsfactory/components/die_bbox_frame.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/disk.py` & `gdsfactory-6.93.0/gdsfactory/components/disk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/edge_coupler_array.py` & `gdsfactory-6.93.0/gdsfactory/components/edge_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ellipse.py` & `gdsfactory-6.93.0/gdsfactory/components/ellipse.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/extend_ports_list.py` & `gdsfactory-6.93.0/gdsfactory/components/extend_ports_list.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/extension.py` & `gdsfactory-6.93.0/gdsfactory/components/extension.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/fiber.py` & `gdsfactory-6.93.0/gdsfactory/components/fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/fiber_array.py` & `gdsfactory-6.93.0/gdsfactory/components/fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/fiducial_squares.py` & `gdsfactory-6.93.0/gdsfactory/components/fiducial_squares.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ge_detector_straight_si_contacts.py` & `gdsfactory-6.93.0/gdsfactory/components/ge_detector_straight_si_contacts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_array.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_dual_pol.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_elliptical.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_elliptical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_elliptical_arbitrary.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_elliptical_lumerical.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_elliptical_trenches.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_elliptical_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_functions.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_loss.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_loss.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_loss_fiber_single.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_loss_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_rectangular.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_rectangular_arbitrary.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/grating_coupler_tree.py` & `gdsfactory-6.93.0/gdsfactory/components/grating_coupler_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/greek_cross.py` & `gdsfactory-6.93.0/gdsfactory/components/greek_cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/hline.py` & `gdsfactory-6.93.0/gdsfactory/components/hline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/interdigital_capacitor.py` & `gdsfactory-6.93.0/gdsfactory/components/interdigital_capacitor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/litho_calipers.py` & `gdsfactory-6.93.0/gdsfactory/components/litho_calipers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/litho_ruler.py` & `gdsfactory-6.93.0/gdsfactory/components/litho_ruler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/litho_steps.py` & `gdsfactory-6.93.0/gdsfactory/components/litho_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/logo.py` & `gdsfactory-6.93.0/gdsfactory/components/logo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/loop_mirror.py` & `gdsfactory-6.93.0/gdsfactory/components/loop_mirror.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mmi1x2.py` & `gdsfactory-6.93.0/gdsfactory/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mmi1x2_with_sbend.py` & `gdsfactory-6.93.0/gdsfactory/components/mmi1x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mmi2x2.py` & `gdsfactory-6.93.0/gdsfactory/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mmi2x2_with_sbend.py` & `gdsfactory-6.93.0/gdsfactory/components/mmi2x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mmi_90degree_hybrid.py` & `gdsfactory-6.93.0/gdsfactory/components/mmi_90degree_hybrid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mode_converter.py` & `gdsfactory-6.93.0/gdsfactory/components/mode_converter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mzi.py` & `gdsfactory-6.93.0/gdsfactory/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mzi_arm.py` & `gdsfactory-6.93.0/gdsfactory/components/mzi_arm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mzi_arms.py` & `gdsfactory-6.93.0/gdsfactory/components/mzi_arms.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mzi_lattice.py` & `gdsfactory-6.93.0/gdsfactory/components/mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mzi_pads_center.py` & `gdsfactory-6.93.0/gdsfactory/components/mzi_pads_center.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mzi_phase_shifter.py` & `gdsfactory-6.93.0/gdsfactory/components/mzi_phase_shifter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mzit.py` & `gdsfactory-6.93.0/gdsfactory/components/mzit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mzit_lattice.py` & `gdsfactory-6.93.0/gdsfactory/components/mzit_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/mzm.py` & `gdsfactory-6.93.0/gdsfactory/components/mzm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/nxn.py` & `gdsfactory-6.93.0/gdsfactory/components/nxn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/optimal_90deg.py` & `gdsfactory-6.93.0/gdsfactory/components/optimal_90deg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/optimal_hairpin.py` & `gdsfactory-6.93.0/gdsfactory/components/optimal_hairpin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/optimal_step.py` & `gdsfactory-6.93.0/gdsfactory/components/optimal_step.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/pack_doe.py` & `gdsfactory-6.93.0/gdsfactory/components/pack_doe.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/pad.py` & `gdsfactory-6.93.0/gdsfactory/components/pad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/pad_gsg.py` & `gdsfactory-6.93.0/gdsfactory/components/pad_gsg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/pads_shorted.py` & `gdsfactory-6.93.0/gdsfactory/components/pads_shorted.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/polarization_splitter_rotator.py` & `gdsfactory-6.93.0/gdsfactory/components/polarization_splitter_rotator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ramp.py` & `gdsfactory-6.93.0/gdsfactory/components/ramp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/rectangle.py` & `gdsfactory-6.93.0/gdsfactory/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/rectangle_with_slits.py` & `gdsfactory-6.93.0/gdsfactory/components/rectangle_with_slits.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/regular_polygon.py` & `gdsfactory-6.93.0/gdsfactory/components/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/resistance_meander.py` & `gdsfactory-6.93.0/gdsfactory/components/resistance_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/resistance_sheet.py` & `gdsfactory-6.93.0/gdsfactory/components/resistance_sheet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring.py` & `gdsfactory-6.93.0/gdsfactory/components/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_crow.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_crow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_crow_couplers.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_crow_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_double.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_double_heater.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_double_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_double_pn.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_double_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_section_based.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_section_based.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_single.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_single_array.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_single_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_single_bend_coupler.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_single_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_single_dut.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_single_dut.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_single_heater.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_single_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/ring_single_pn.py` & `gdsfactory-6.93.0/gdsfactory/components/ring_single_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/seal_ring.py` & `gdsfactory-6.93.0/gdsfactory/components/seal_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/snspd.py` & `gdsfactory-6.93.0/gdsfactory/components/snspd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/spiral_double.py` & `gdsfactory-6.93.0/gdsfactory/components/spiral_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/spiral_external_io.py` & `gdsfactory-6.93.0/gdsfactory/components/spiral_external_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/spiral_heater.py` & `gdsfactory-6.93.0/gdsfactory/components/spiral_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/spiral_inner_io.py` & `gdsfactory-6.93.0/gdsfactory/components/spiral_inner_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/splitter_chain.py` & `gdsfactory-6.93.0/gdsfactory/components/splitter_chain.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/splitter_tree.py` & `gdsfactory-6.93.0/gdsfactory/components/splitter_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight.py` & `gdsfactory-6.93.0/gdsfactory/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight_array.py` & `gdsfactory-6.93.0/gdsfactory/components/straight_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight_heater_doped_rib.py` & `gdsfactory-6.93.0/gdsfactory/components/straight_heater_doped_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight_heater_doped_strip.py` & `gdsfactory-6.93.0/gdsfactory/components/straight_heater_doped_strip.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight_heater_meander.py` & `gdsfactory-6.93.0/gdsfactory/components/straight_heater_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight_heater_meander_doped.py` & `gdsfactory-6.93.0/gdsfactory/components/straight_heater_meander_doped.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight_heater_metal.py` & `gdsfactory-6.93.0/gdsfactory/components/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight_pin.py` & `gdsfactory-6.93.0/gdsfactory/components/straight_pin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight_pin_slot.py` & `gdsfactory-6.93.0/gdsfactory/components/straight_pin_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/straight_rib.py` & `gdsfactory-6.93.0/gdsfactory/components/straight_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/switch_tree.py` & `gdsfactory-6.93.0/gdsfactory/components/switch_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/taper.py` & `gdsfactory-6.93.0/gdsfactory/components/taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/taper_adiabatic.py` & `gdsfactory-6.93.0/gdsfactory/components/taper_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/taper_cross_section.py` & `gdsfactory-6.93.0/gdsfactory/components/taper_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/taper_from_csv.py` & `gdsfactory-6.93.0/gdsfactory/components/taper_from_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/taper_parabolic.py` & `gdsfactory-6.93.0/gdsfactory/components/taper_parabolic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/terminator.py` & `gdsfactory-6.93.0/gdsfactory/components/terminator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/text.py` & `gdsfactory-6.93.0/gdsfactory/components/text.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/text_freetype.py` & `gdsfactory-6.93.0/gdsfactory/components/text_freetype.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/text_rectangular.py` & `gdsfactory-6.93.0/gdsfactory/components/text_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/text_rectangular_font.py` & `gdsfactory-6.93.0/gdsfactory/components/text_rectangular_font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/triangles.py` & `gdsfactory-6.93.0/gdsfactory/components/triangles.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/verniers.py` & `gdsfactory-6.93.0/gdsfactory/components/verniers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/version_stamp.py` & `gdsfactory-6.93.0/gdsfactory/components/version_stamp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/via.py` & `gdsfactory-6.93.0/gdsfactory/components/via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/via_corner.py` & `gdsfactory-6.93.0/gdsfactory/components/via_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/via_cutback.py` & `gdsfactory-6.93.0/gdsfactory/components/via_cutback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/via_stack.py` & `gdsfactory-6.93.0/gdsfactory/components/via_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/via_stack_slot.py` & `gdsfactory-6.93.0/gdsfactory/components/via_stack_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/via_stack_with_offset.py` & `gdsfactory-6.93.0/gdsfactory/components/via_stack_with_offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/wafer.py` & `gdsfactory-6.93.0/gdsfactory/components/wafer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/wire.py` & `gdsfactory-6.93.0/gdsfactory/components/wire.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/components/wire_sbend.py` & `gdsfactory-6.93.0/gdsfactory/components/wire_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/config.py` & `gdsfactory-6.93.0/gdsfactory/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from loguru import logger
 import omegaconf
 from omegaconf import OmegaConf
 
 from rich.console import Console
 from rich.table import Table
 
-__version__ = "6.92.2"
+__version__ = "6.93.0"
 PathType = Union[str, pathlib.Path]
 
 home = pathlib.Path.home()
 cwd = pathlib.Path.cwd()
 module_path = pathlib.Path(__file__).parent.absolute()
 repo_path = module_path.parent
 home_path = pathlib.Path.home() / ".gdsfactory"
```

### Comparing `gdsfactory-6.92.2/gdsfactory/constants.py` & `gdsfactory-6.93.0/gdsfactory/constants.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/containers.py` & `gdsfactory-6.93.0/gdsfactory/containers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/cross_section.py` & `gdsfactory-6.93.0/gdsfactory/cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/decorators.py` & `gdsfactory-6.93.0/gdsfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/difftest.py` & `gdsfactory-6.93.0/gdsfactory/difftest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/events.py` & `gdsfactory-6.93.0/gdsfactory/events.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/export/to_3d.py` & `gdsfactory-6.93.0/gdsfactory/export/to_3d.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/export/to_np.py` & `gdsfactory-6.93.0/gdsfactory/export/to_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/export/to_stl.py` & `gdsfactory-6.93.0/gdsfactory/export/to_stl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/export/write_gerbers.py` & `gdsfactory-6.93.0/gdsfactory/export/write_gerbers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/filestorage.py` & `gdsfactory-6.93.0/gdsfactory/filestorage.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/fill.py` & `gdsfactory-6.93.0/gdsfactory/fill.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/font.py` & `gdsfactory-6.93.0/gdsfactory/font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/functions.py` & `gdsfactory-6.93.0/gdsfactory/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/gdsdiff/gds_diff_git.py` & `gdsfactory-6.93.0/gdsfactory/gdsdiff/gds_diff_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/gdsdiff/gdsdiff.py` & `gdsfactory-6.93.0/gdsfactory/gdsdiff/gdsdiff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/gdsdiff/install.py` & `gdsfactory-6.93.0/gdsfactory/gdsdiff/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/gdsdiff/test_xor.py` & `gdsfactory-6.93.0/gdsfactory/gdsdiff/test_xor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/README.md` & `gdsfactory-6.93.0/gdsfactory/generic_tech/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/__init__.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/get_klayout_pyxs.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/get_klayout_pyxs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/errors.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/generic.drc` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/generic.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/generic.lydrc` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/generic.lydrc`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/drc/write_drc.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/drc/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/grain.xml`

 * *Files 2% similar despite different names*

#### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>gdsfactory</name>
   <token/>
   <hidden>false</hidden>
-  <version>6.92.2</version>
+  <version>6.93.0</version>
   <api-version/>
   <title>gdsfactory</title>
   <doc>EDA tool to layout integrated circuits</doc>
   <doc-url>https://gdsfactory.github.io/gdsfactory/</doc-url>
   <url>https://github.com/gdsfactory/gdsfactory</url>
   <license>MIT</license>
   <author>Joaquin Matres</author>
```

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/icon_128x128.png` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/icon_64x64.png` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/README.md` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/run_lvs.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,8 +75,9 @@
     c9_mk.center = c9.center
     c10_mk.center = c10.center
     return c
 
 
 if __name__ == "__main__":
     c = heater_lvs()
+    c.write_gds("straight_heater_metal.gds")
     c.show()
```

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

 * *Files 16% similar despite different names*

#### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>gdsfactory.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;6.92.2&quot;
+__version__ = &quot;6.93.0&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;gdsfactory&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/generic.layerstack` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

 * *Files 0% similar despite different names*

#### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

```diff
@@ -333,15 +333,15 @@
     <valid>true</valid>
     <visible>false</visible>
     <transparent>false</transparent>
     <width>1</width>
     <marked>false</marked>
     <xfill>false</xfill>
     <animation>0</animation>
-    <name>WGNCLAD 36/0</name>
+    <name>WGclad_material 36/0</name>
     <source>36/0@1</source>
   </properties>
   <properties>
     <frame-color>#ff00ff</frame-color>
     <fill-color>#ff00ff</fill-color>
     <frame-brightness>0</frame-brightness>
     <fill-brightness>0</fill-brightness>
```

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyt` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyt`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs` & `gdsfactory-6.93.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/layer_map.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/layer_stack.py` & `gdsfactory-6.93.0/gdsfactory/generic_tech/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/generic_tech/layer_views.yaml` & `gdsfactory-6.93.0/gdsfactory/generic_tech/layer_views.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
   WGN_Nitride:
     layer: [34, 0]
     layer_in_name: true
     hatch_pattern: left-hatched
     transparent: true
     width: 1
     color: "#ff8000"
-  WGNCLAD:
+  WGclad_material:
     layer: [36, 0]
     layer_in_name: true
     hatch_pattern: coarsely dotted
     visible: false
     width: 1
     color: "silver"
   GE:
```

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/__init__.py` & `gdsfactory-6.93.0/gdsfactory/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/boolean.py` & `gdsfactory-6.93.0/gdsfactory/geometry/boolean.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/boolean_klayout.py` & `gdsfactory-6.93.0/gdsfactory/geometry/boolean_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/boolean_polygons.py` & `gdsfactory-6.93.0/gdsfactory/geometry/boolean_polygons.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/check_duplicated_cells.py` & `gdsfactory-6.93.0/gdsfactory/geometry/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/check_exclusion.py` & `gdsfactory-6.93.0/gdsfactory/geometry/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/check_inclusion.py` & `gdsfactory-6.93.0/gdsfactory/geometry/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/check_space.py` & `gdsfactory-6.93.0/gdsfactory/geometry/check_space.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/check_width.py` & `gdsfactory-6.93.0/gdsfactory/geometry/check_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/fill_klayout.py` & `gdsfactory-6.93.0/gdsfactory/geometry/fill_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/fill_tiled.py` & `gdsfactory-6.93.0/gdsfactory/geometry/fill_tiled.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/fillet.py` & `gdsfactory-6.93.0/gdsfactory/geometry/fillet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/functions.py` & `gdsfactory-6.93.0/gdsfactory/geometry/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/invert.py` & `gdsfactory-6.93.0/gdsfactory/geometry/invert.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/layer_priority.py` & `gdsfactory-6.93.0/gdsfactory/geometry/layer_priority.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/manhattanize.py` & `gdsfactory-6.93.0/gdsfactory/geometry/manhattanize.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/maskprep.py` & `gdsfactory-6.93.0/gdsfactory/geometry/maskprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/maskprep_flat.py` & `gdsfactory-6.93.0/gdsfactory/geometry/maskprep_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/offset.py` & `gdsfactory-6.93.0/gdsfactory/geometry/offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/outline.py` & `gdsfactory-6.93.0/gdsfactory/geometry/outline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/trim.py` & `gdsfactory-6.93.0/gdsfactory/geometry/trim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/union.py` & `gdsfactory-6.93.0/gdsfactory/geometry/union.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/write_drc.py` & `gdsfactory-6.93.0/gdsfactory/geometry/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/geometry/xor_diff.py` & `gdsfactory-6.93.0/gdsfactory/geometry/xor_diff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/get_factories.py` & `gdsfactory-6.93.0/gdsfactory/get_factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/get_netlist.py` & `gdsfactory-6.93.0/gdsfactory/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/get_netlist_flat.py` & `gdsfactory-6.93.0/gdsfactory/get_netlist_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/get_netlist_klayout.py` & `gdsfactory-6.93.0/gdsfactory/get_netlist_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/grid.py` & `gdsfactory-6.93.0/gdsfactory/grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/install.py` & `gdsfactory-6.93.0/gdsfactory/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/klive.py` & `gdsfactory-6.93.0/gdsfactory/klive.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/labels/__init__.py` & `gdsfactory-6.93.0/gdsfactory/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/labels/add_label_yaml.py` & `gdsfactory-6.93.0/gdsfactory/labels/add_label_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/labels/ehva.py` & `gdsfactory-6.93.0/gdsfactory/labels/ehva.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/labels/merge_test_metadata.py` & `gdsfactory-6.93.0/gdsfactory/labels/merge_test_metadata.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/labels/siepic.py` & `gdsfactory-6.93.0/gdsfactory/labels/siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/labels/write_labels.py` & `gdsfactory-6.93.0/gdsfactory/labels/write_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/materials.py` & `gdsfactory-6.93.0/gdsfactory/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/name.py` & `gdsfactory-6.93.0/gdsfactory/name.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/pack.py` & `gdsfactory-6.93.0/gdsfactory/pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/path.py` & `gdsfactory-6.93.0/gdsfactory/path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/pdk.py` & `gdsfactory-6.93.0/gdsfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/picmodel.py` & `gdsfactory-6.93.0/gdsfactory/picmodel.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/pixelate.py` & `gdsfactory-6.93.0/gdsfactory/pixelate.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/plugins/dagster/workflow.py` & `gdsfactory-6.93.0/gdsfactory/plugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/plugins/database/README.md` & `gdsfactory-6.93.0/gdsfactory/plugins/database/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/plugins/database/db_upload.py` & `gdsfactory-6.93.0/gdsfactory/plugins/database/db_upload.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/plugins/database/models.py` & `gdsfactory-6.93.0/gdsfactory/plugins/database/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/port.py` & `gdsfactory-6.93.0/gdsfactory/port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/quickplotter.py` & `gdsfactory-6.93.0/gdsfactory/quickplotter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/read/__init__.py` & `gdsfactory-6.93.0/gdsfactory/read/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/read/from_dphox.py` & `gdsfactory-6.93.0/gdsfactory/read/from_dphox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/read/from_gdspaths.py` & `gdsfactory-6.93.0/gdsfactory/read/from_gdspaths.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/read/from_np.py` & `gdsfactory-6.93.0/gdsfactory/read/from_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/read/from_phidl.py` & `gdsfactory-6.93.0/gdsfactory/read/from_phidl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/read/from_yaml.py` & `gdsfactory-6.93.0/gdsfactory/read/from_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/read/from_yaml_template.py` & `gdsfactory-6.93.0/gdsfactory/read/from_yaml_template.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/read/import_gds.py` & `gdsfactory-6.93.0/gdsfactory/read/import_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/read/labels.py` & `gdsfactory-6.93.0/gdsfactory/read/labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/__init__.py` & `gdsfactory-6.93.0/gdsfactory/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/add_electrical_pads_shortest.py` & `gdsfactory-6.93.0/gdsfactory/routing/add_electrical_pads_shortest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/add_electrical_pads_top.py` & `gdsfactory-6.93.0/gdsfactory/routing/add_electrical_pads_top.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/add_electrical_pads_top_dc.py` & `gdsfactory-6.93.0/gdsfactory/routing/add_electrical_pads_top_dc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/add_fiber_array.py` & `gdsfactory-6.93.0/gdsfactory/routing/add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/add_fiber_single.py` & `gdsfactory-6.93.0/gdsfactory/routing/add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/add_pads.py` & `gdsfactory-6.93.0/gdsfactory/routing/add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/all_angle.py` & `gdsfactory-6.93.0/gdsfactory/routing/all_angle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/auto_taper.py` & `gdsfactory-6.93.0/gdsfactory/routing/auto_taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/factories.py` & `gdsfactory-6.93.0/gdsfactory/routing/factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/fanout.py` & `gdsfactory-6.93.0/gdsfactory/routing/fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/fanout2x2.py` & `gdsfactory-6.93.0/gdsfactory/routing/fanout2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_bundle.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_bundle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_bundle_corner.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_bundle_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_bundle_from_steps.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_bundle_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_bundle_from_waypoints.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_bundle_from_waypoints.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_bundle_path_length_match.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_bundle_path_length_match.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_bundle_sbend.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_bundle_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_bundle_u.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_bundle_u.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_input_labels.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_input_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_route.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_route.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_route_astar.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_route_astar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_route_from_steps.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_route_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_route_sbend.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_route_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_routes_bend180.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_routes_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/get_routes_straight.py` & `gdsfactory-6.93.0/gdsfactory/routing/get_routes_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/manhattan.py` & `gdsfactory-6.93.0/gdsfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/path_length_matching.py` & `gdsfactory-6.93.0/gdsfactory/routing/path_length_matching.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/route_fiber_array.py` & `gdsfactory-6.93.0/gdsfactory/routing/route_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/route_fiber_single.py` & `gdsfactory-6.93.0/gdsfactory/routing/route_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/route_ports_to_side.py` & `gdsfactory-6.93.0/gdsfactory/routing/route_ports_to_side.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/route_quad.py` & `gdsfactory-6.93.0/gdsfactory/routing/route_quad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/route_sharp.py` & `gdsfactory-6.93.0/gdsfactory/routing/route_sharp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/route_south.py` & `gdsfactory-6.93.0/gdsfactory/routing/route_south.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/sort_ports.py` & `gdsfactory-6.93.0/gdsfactory/routing/sort_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/routing/utils.py` & `gdsfactory-6.93.0/gdsfactory/routing/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/01_component_pcell.py` & `gdsfactory-6.93.0/gdsfactory/samples/01_component_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/01_component_pcell/test_straight_wide.yml` & `gdsfactory-6.93.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/01_component_pcell_with_pins.py` & `gdsfactory-6.93.0/gdsfactory/samples/01_component_pcell_with_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml` & `gdsfactory-6.93.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/03_move.py` & `gdsfactory-6.93.0/gdsfactory/samples/03_move.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/04_connect.py` & `gdsfactory-6.93.0/gdsfactory/samples/04_connect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/05_remove_layers.py` & `gdsfactory-6.93.0/gdsfactory/samples/05_remove_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/06_remapping_layers.py` & `gdsfactory-6.93.0/gdsfactory/samples/06_remapping_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/07_flattening_device.py` & `gdsfactory-6.93.0/gdsfactory/samples/07_flattening_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/11_component_layout.py` & `gdsfactory-6.93.0/gdsfactory/samples/11_component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/12_component_refs.py` & `gdsfactory-6.93.0/gdsfactory/samples/12_component_refs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/13_component_netlist.py` & `gdsfactory-6.93.0/gdsfactory/samples/13_component_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/14_component_connectivity.py` & `gdsfactory-6.93.0/gdsfactory/samples/14_component_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/15_component_sequence1.py` & `gdsfactory-6.93.0/gdsfactory/samples/15_component_sequence1.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/16_component_sequence2.py` & `gdsfactory-6.93.0/gdsfactory/samples/16_component_sequence2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/17_ports.py` & `gdsfactory-6.93.0/gdsfactory/samples/17_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/20_components.py` & `gdsfactory-6.93.0/gdsfactory/samples/20_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/22_add_pads.py` & `gdsfactory-6.93.0/gdsfactory/samples/22_add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/23_reticle.py` & `gdsfactory-6.93.0/gdsfactory/samples/23_reticle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/23_reticle_passives.py` & `gdsfactory-6.93.0/gdsfactory/samples/23_reticle_passives.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/24_doe_2.py` & `gdsfactory-6.93.0/gdsfactory/samples/24_doe_2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/24_doe_3.py` & `gdsfactory-6.93.0/gdsfactory/samples/24_doe_3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/30_lidar.py` & `gdsfactory-6.93.0/gdsfactory/samples/30_lidar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/30_lidar_pcell.py` & `gdsfactory-6.93.0/gdsfactory/samples/30_lidar_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/30_lidar_with_pads.py` & `gdsfactory-6.93.0/gdsfactory/samples/30_lidar_with_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing.py` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/big_device.py` & `gdsfactory-6.93.0/gdsfactory/samples/big_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/demo/benchmark/fill_demo.py` & `gdsfactory-6.93.0/gdsfactory/samples/demo/benchmark/fill_demo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/demo/circuits/mask.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/demo/circuits/mask.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml` & `gdsfactory-6.93.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/demo/drc_errors.py` & `gdsfactory-6.93.0/gdsfactory/samples/demo/drc_errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/demo/drc_write.py` & `gdsfactory-6.93.0/gdsfactory/samples/demo/drc_write.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/demo/layers.py` & `gdsfactory-6.93.0/gdsfactory/samples/demo/layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/demo/lvs.py` & `gdsfactory-6.93.0/gdsfactory/samples/demo/lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/demo/pcell.py` & `gdsfactory-6.93.0/gdsfactory/samples/demo/pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/netlists/mzi.yml` & `gdsfactory-6.93.0/gdsfactory/samples/netlists/mzi.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/netlists/mzi_full.yml` & `gdsfactory-6.93.0/gdsfactory/samples/netlists/mzi_full.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/fab_c.py` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/fab_d/phase_shifters.py` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c.py` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     layer:
     - 1
     - 0
     layer_slab:
     - 2
     - 0
     n_periods: 30
-    nclad: 1.443
+    clad_material: 1.443
     neff: 2.638
     polarization: te
     slab_offset: 2
     slab_xmin: -1
     spiked: true
     taper_angle: 40
     taper_length: 16.6
@@ -45,15 +45,15 @@
     fiber_marker_width: 11
     grating_line_width: 0.6
     layer:
     - 34
     - 0
     layer_slab: null
     n_periods: 30
-    nclad: 1.443
+    clad_material: 1.443
     neff: 2.638
     polarization: te
     slab_offset: 2
     slab_xmin: -1
     spiked: true
     taper_angle: 40
     taper_length: 16.6
```

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml` & `gdsfactory-6.93.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/schematic_editor.py` & `gdsfactory-6.93.0/gdsfactory/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/serialization.py` & `gdsfactory-6.93.0/gdsfactory/serialization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/show.py` & `gdsfactory-6.93.0/gdsfactory/show.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/add_simulation_markers.py` & `gdsfactory-6.93.0/gdsfactory/simulation/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/convert_sparameters.py` & `gdsfactory-6.93.0/gdsfactory/simulation/convert_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/devsim/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/devsim/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/devsim/doping.py` & `gdsfactory-6.93.0/gdsfactory/simulation/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/devsim/get_simulation.py` & `gdsfactory-6.93.0/gdsfactory/simulation/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/devsim/get_simulation_xsection.py` & `gdsfactory-6.93.0/gdsfactory/simulation/devsim/get_simulation_xsection.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 
 class PINWaveguide(BaseModel):
     """Silicon PIN junction waveguide Model.
 
     Parameters:
         wg_width: waveguide width.
-        wg_thickness: thickness waveguide (um).
+        core_thickness: thickness waveguide (um).
         p_offset: offset between waveguide center and P-doping in um
             negative to push toward n-side.
         n_offset: offset between waveguide center and N-doping in um
             negative to push toward p-side).
         ppp_offset: offset between waveguide center and Ppp-doping in um
             negative to push toward n-side) NOT IMPLEMENTED.
         npp_offset: offset between waveguide center and Npp-doping in um
@@ -123,28 +123,28 @@
             xmargin          width            xmargin
            <------>       <---------->        <------>
                    ppp_offset        npp_offset
                      <--->             <---->
                         p_offset n_offset
                              <-> <->
          xcontact          _____|_____ _ _ _ _ _ _ _ _ _
-          <---->          |  |     |  |                | wg_thickness
+          <---->          |  |     |  |                | core_thickness
           ======__________|  |     |  |__________======| _
           |          |       |     |         |         | |
           |  Ppp+P   |   P   |  i  |    N    |  Npp+N  | | slab_thickness
           |__________|_______|_____|_________|_________| |
           ^          ^       ^     ^         ^         ^
       pp_res_x   pp_p_res     pn_res      pp_p_res  pp_res_x
           <-------------------------------------------->
                                w_sim
 
     """
 
     wg_width: float
-    wg_thickness: float
+    core_thickness: float
     p_offset: float = 0.0
     n_offset: float = 0.0
     ppp_offset: float = 0.5 * um
     npp_offset: float = 0.5 * um
     slab_thickness: float
     t_box: float = 2.0 * um
     t_clad: float = 2.0 * um
@@ -167,28 +167,28 @@
     class Config:
         """Enable adding new."""
 
         extra = Extra.allow
 
     # @property
     # def t_sim(self):
-    #     return self.t_box + self.wg_thickness + self.t_clad
+    #     return self.t_box + self.core_thickness + self.t_clad
 
     # @property
     # def w_sim(self):
     #     return 2 * self.xmargin + self.ppp_offset + self.npp_offset
 
     def create_2d_mesh(self, device) -> None:
         """Creates a 2D mesh."""
         xmin = (-self.xmargin - self.ppp_offset - self.wg_width / 2) / cm
         xmax = (self.xmargin + self.npp_offset + self.wg_width / 2) / cm
         self.xppp = -self.ppp_offset - self.wg_width / 2
         self.xnpp = self.npp_offset + self.wg_width / 2
         ymin = 0 / cm
-        ymax = (self.wg_thickness) / cm
+        ymax = (self.core_thickness) / cm
         xmin_waveguide = (-self.wg_width / 2) / cm
         xmax_waveguide = (self.wg_width / 2) / cm
         yslab = (self.slab_thickness) / cm
 
         devsim.create_2d_mesh(mesh="dio")
         devsim.add_2d_mesh_line(mesh="dio", dir="x", pos=xmin, ps=self.pp_res_x / cm)
         devsim.add_2d_mesh_line(
@@ -484,16 +484,16 @@
         resolution: int = 200,
         perturb: bool = True,
         nmodes: int = 4,
         bend_radius: Optional[float] = None,
         cache: bool = False,
         precision: Precision = "double",
         filter_pol: Optional[FilterPol] = None,
-        ncore: MaterialSpec = "si",
-        nclad: MaterialSpec = "sio2",
+        core_material: MaterialSpec = "si",
+        clad_material: MaterialSpec = "sio2",
     ) -> Waveguide:
         """Converts the FEM model to a Waveguide object.
 
         - Rescales lengths to um
         - Adjusts origin to match Waveguide object convention
 
         Args:
@@ -558,33 +558,33 @@
             else None
         )
 
         # Create perturbed waveguide, handle like regular mode
         return Waveguide(
             wavelength=wavelength,
             wg_width=self.wg_width / um,
-            wg_thickness=self.wg_thickness / um,
+            core_thickness=self.core_thickness / um,
             slab_thickness=self.slab_thickness / um,
             t_box=t_box,
             t_clad=t_clad,
             xmargin=(self.ppp_offset + self.xmargin) / um,
             resolution=resolution,
             dn_dict=dn_dict,
             precision=precision,
             filter_pol=filter_pol,
-            ncore=ncore,
-            nclad=nclad,
+            core_material=core_material,
+            clad_material=clad_material,
             cache=cache,
         )
 
 
 if __name__ == "__main__":
     c = PINWaveguide(
         wg_width=500 * nm,
-        wg_thickness=220 * nm,
+        core_thickness=220 * nm,
         slab_thickness=90 * nm,
     )
     c.ddsolver()
     c.save_device("test.dat")
 
     import os
     import shutil
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/devsim/get_solver.py` & `gdsfactory-6.93.0/gdsfactory/simulation/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/devsim/test_devsim.py` & `gdsfactory-6.93.0/gdsfactory/simulation/devsim/test_devsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def test_pin_waveguide():
     """Test reverse bias waveguide."""
     nm = 1e-9
     c = get_simulation_xsection.PINWaveguide(
         wg_width=500 * nm,
-        wg_thickness=220 * nm,
+        core_thickness=220 * nm,
         slab_thickness=90 * nm,
     )
     c.ddsolver()
     n_dist = {}
     neffs = {}
 
     vmin = 0
@@ -35,15 +35,15 @@
     assert np.isclose(dn.real, -0.00011342135795189279), dn.real
 
 
 if __name__ == "__main__":
     nm = 1e-9
     c = get_simulation_xsection.PINWaveguide(
         wg_width=500 * nm,
-        wg_thickness=220 * nm,
+        core_thickness=220 * nm,
         slab_thickness=90 * nm,
     )
     c.ddsolver()
     n_dist = {}
     neffs = {}
 
     vmin = 0
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/eme/meow_eme.py` & `gdsfactory-6.93.0/gdsfactory/simulation/eme/meow_eme.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/eme/test_meow_simulation.py` & `gdsfactory-6.93.0/gdsfactory/simulation/eme/test_meow_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/fem/mode_solver.py` & `gdsfactory-6.93.0/gdsfactory/simulation/fem/mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/fem/test_mode_solver.py` & `gdsfactory-6.93.0/gdsfactory/simulation/fem/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/get_effective_indices.py` & `gdsfactory-6.93.0/gdsfactory/simulation/get_effective_indices.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import numpy as np
 from scipy.optimize import fsolve
 from typing_extensions import Literal
 
 
 def get_effective_indices(
-    ncore: float,
+    core_material: float,
     nsubstrate: float,
-    ncladding: float,
+    clad_materialding: float,
     thickness: float,
     wavelength: float,
     polarization: Literal["te", "tm"],
 ) -> List[float]:
     """Returns the effective refractive indices for a 1D mode.
 
     Args:
@@ -26,37 +26,37 @@
         thickness: Thickness of the film in um.
         wavelength: Wavelength in um.
         polarization: Either "te" or "tm".
 
     .. code::
 
         -----------------      |
-        ncladding             inf
+        clad_materialding             inf
         -----------------      |
-        ncore              thickness
+        core_material              thickness
         -----------------      |
         nsubstrate            inf
         -----------------      |
 
     .. code::
 
         import gdsfactory.simulation as sim
 
         neffs = sim.get_effective_indices(
-            ncore=3.4777,
-            ncladding=1.444,
+            core_material=3.4777,
+            clad_materialding=1.444,
             nsubstrate=1.444,
             thickness=0.22,
             wavelength=1.55,
             polarization="te",
         )
 
     """
-    epsilon_core = ncore**2
-    epsilon_cladding = ncladding**2
+    epsilon_core = core_material**2
+    epsilon_cladding = clad_materialding**2
     epsilon_substrate = nsubstrate**2
 
     thickness *= 1e-6
     wavelength *= 1e-6
 
     if polarization == "te":
         tm = False
@@ -101,28 +101,28 @@
             indices.append(index)
 
     return np.sqrt(indices).tolist()
 
 
 def test_effective_index():
     neff = get_effective_indices(
-        ncore=3.4777,
-        ncladding=1.444,
+        core_material=3.4777,
+        clad_materialding=1.444,
         nsubstrate=1.444,
         thickness=0.22,
         wavelength=1.55,
         polarization="te",
     )
     assert np.isclose(neff[0], 2.8494636999424405)
 
 
 if __name__ == "__main__":
     print(
         get_effective_indices(
-            ncore=3.4777,
-            ncladding=1.444,
+            core_material=3.4777,
+            clad_materialding=1.444,
             nsubstrate=1.444,
             thickness=0.22,
             wavelength=1.55,
             polarization="te",
         )
     )
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/get_modes_path.py` & `gdsfactory-6.93.0/gdsfactory/simulation/get_modes_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/get_sparameters_path.py` & `gdsfactory-6.93.0/gdsfactory/simulation/get_sparameters_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from __future__ import annotations
 
-import meep as mp
+try:
+    import meep as mp
+except ModuleNotFoundError as e:
+    print("You need to 'conda install -c conda-forge pymeep=*=mpi_mpich_* nlopt -y'")
+    raise e
 
 from gdsfactory.config import logger
 from gdsfactory.simulation import plot, port_symmetries
 from gdsfactory.simulation.get_sparameters_path import get_sparameters_data_meep
 from gdsfactory.simulation.gmeep.get_simulation import get_simulation
 from gdsfactory.simulation.gmeep.meep_adjoint_optimization import (
     get_meep_adjoint_optimizer,
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_material.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_material.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_meep_geometry.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_port_eigenmode.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_simulation.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,65 +17,65 @@
 from gdsfactory.typings import Floats
 
 nm = 1e-3
 nSi = 3.48
 nSiO2 = 1.44
 
 
-def fiber_ncore(fiber_numerical_aperture, fiber_nclad):
-    return (fiber_numerical_aperture**2 + fiber_nclad**2) ** 0.5
+def fiber_core_material(fiber_numerical_aperture, fiber_clad_material):
+    return (fiber_numerical_aperture**2 + fiber_clad_material**2) ** 0.5
 
 
 def get_simulation_grating_farfield(
     period: float = 0.66,
     fill_factor: float = 0.5,
     n_periods: int = 30,
     widths: Optional[Floats] = None,
     gaps: Optional[Floats] = None,
     etch_depth: float = 70 * nm,
     fiber_angle_deg: float = 20.0,
     fiber_xposition: float = 1.0,
     fiber_core_diameter: float = 10.4,
     fiber_numerical_aperture: float = 0.14,
-    fiber_nclad: float = nSiO2,
-    ncore: float = nSi,
-    nclad: float = nSiO2,
+    fiber_clad_material: float = nSiO2,
+    core_material: float = nSi,
+    clad_material: float = nSiO2,
     nsubstrate: float = nSi,
     pml_thickness: float = 1,
     box_thickness: float = 2.0,
     clad_thickness: float = 2.0,
     core_thickness: float = 220 * nm,
     resolution: int = 64,  # pixels/um
     wavelength_min: float = 1.5,
     wavelength_max: float = 1.6,
     wavelength_points: int = 50,
 ) -> Dict[str, Any]:
     """Returns grating coupler far field simulation.
 
     FIXME! needs some more work.
 
-    na**2 = ncore**2 - nclad**2
-    ncore = sqrt(na**2 + ncore**2)
+    na**2 = core_material**2 - clad_material**2
+    core_material = sqrt(na**2 + core_material**2)
 
     Args:
         period: fiber grating period.
         fill_factor: fraction of the grating period
             filled with the grating material.
         n_periods: number of periods
         widths: Optional list of widths.
             Overrides period, fill_factor, n_periods.
         gaps: Optional list of gaps. Overrides period, fill_factor, n_periods.
         etch_depth: grating etch depth.
         fiber_angle_deg: fiber angle in degrees.
         fiber_xposition: xposition.
         fiber_core_diameter: fiber diameter.
         fiber_numerical_aperture: NA.
-        fiber_nclad: fiber cladding index.
-        ncore: fiber index core.
-        nclad: top cladding index.
+        fiber_clad_material: fiber cladding index.
+        core_material: fiber index core.
+        clad_material: top cladding index.
         nbox: box index bottom.
         nsubstrate: index substrate.
         pml_thickness: pml_thickness (um).
         substrate_thickness: substrate_thickness (um).
         box_thickness: thickness for bottom cladding (um).
         core_thickness: core_thickness (um).
         top_clad_thickness: thickness of the top cladding.
@@ -99,18 +99,18 @@
     settings = dict(
         period=period,
         fill_factor=fill_factor,
         fiber_angle_deg=fiber_angle_deg,
         fiber_xposition=fiber_xposition,
         fiber_core_diameter=fiber_core_diameter,
         fiber_numerical_aperture=fiber_core_diameter,
-        fiber_nclad=fiber_nclad,
+        fiber_clad_material=fiber_clad_material,
         resolution=resolution,
-        ncore=ncore,
-        nclad=nclad,
+        core_material=core_material,
+        clad_material=clad_material,
         nsubstrate=nsubstrate,
         n_periods=n_periods,
         box_thickness=box_thickness,
         clad_thickness=clad_thickness,
         etch_depth=etch_depth,
         wavelength_min=wavelength_min,
         wavelength_max=wavelength_max,
@@ -118,16 +118,16 @@
         widths=widths,
         gaps=gaps,
     )
     length_grating = np.sum(widths) + np.sum(gaps)
 
     substrate_thickness = 1.0
     hair = 4
-    core_material = mp.Medium(index=ncore)
-    clad_material = mp.Medium(index=nclad)
+    core_material = mp.Medium(index=core_material)
+    clad_material = mp.Medium(index=clad_material)
     fiber_angle = np.radians(fiber_angle_deg)
 
     y_offset = 0
     x_offset = 0
 
     # Minimally-parametrized computational cell
     # Could be further optimized
@@ -178,17 +178,19 @@
     waveguide_port_size = mp.Vector3(0, 2 * clad_thickness - 0.2)
     waveguide_port_direction = mp.X
 
     # Geometry
     fiber_clad = 120
     hfiber_geom = 100  # Some large number to make fiber extend into PML
 
-    fiber_ncore = (fiber_numerical_aperture**2 + fiber_nclad**2) ** 0.5
-    fiber_clad_material = mp.Medium(index=fiber_nclad)
-    fiber_core_material = mp.Medium(index=fiber_ncore)
+    fiber_core_material = (
+        fiber_numerical_aperture**2 + fiber_clad_material**2
+    ) ** 0.5
+    fiber_clad_material = mp.Medium(index=fiber_clad_material)
+    fiber_core_material = mp.Medium(index=fiber_core_material)
 
     geometry = [
         mp.Block(
             material=fiber_clad_material,
             center=mp.Vector3(
                 x=grating_start + fiber_xposition - fiber_offset_from_angle
             ),
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,38 +21,38 @@
 from gdsfactory.typings import Floats
 
 nm = 1e-3
 nSi = 3.47
 nSiO2 = 1.44
 
 
-def fiber_ncore(fiber_numerical_aperture, fiber_nclad):
-    return (fiber_numerical_aperture**2 + fiber_nclad**2) ** 0.5
+def fiber_core_material(fiber_numerical_aperture, fiber_clad_material):
+    return (fiber_numerical_aperture**2 + fiber_clad_material**2) ** 0.5
 
 
 def get_simulation_grating_fiber(
     period: float = 0.66,
     fill_factor: float = 0.5,
     n_periods: int = 30,
     widths: Optional[Floats] = None,
     gaps: Optional[Floats] = None,
     fiber_angle_deg: float = 20.0,
     fiber_xposition: float = 1.0,
     fiber_core_diameter: float = 10.4,
     fiber_numerical_aperture: float = 0.14,
-    fiber_nclad: float = nSiO2,
+    fiber_clad_material: float = nSiO2,
     nwg: float = nSi,
     nslab: Optional[float] = None,
-    nclad: float = nSiO2,
+    clad_material: float = nSiO2,
     nbox: float = nSiO2,
     nsubstrate: float = nSi,
     pml_thickness: float = 1.0,
     substrate_thickness: float = 1.0,
     box_thickness: float = 2.0,
-    wg_thickness: float = 220 * nm,
+    core_thickness: float = 220 * nm,
     slab_thickness: float = 150 * nm,
     top_clad_thickness: float = 2.0,
     air_gap_thickness: float = 1.0,
     fiber_thickness: float = 2.0,
     resolution: int = 64,  # pixels/um
     wavelength_start: float = 1.4,
     wavelength_stop: float = 1.7,
@@ -62,38 +62,38 @@
     fiber_port_y_offset_from_air: float = 1,
     waveguide_port_x_offset_from_grating_start: float = 10,
     fiber_port_x_size: Optional[float] = None,
     xmargin: float = 10.0,
 ) -> Dict[str, Any]:
     r"""Returns simulation results from grating coupler with fiber.
 
-    na**2 = ncore**2 - nclad**2
-    ncore = sqrt(na**2 + ncore**2)
+    na**2 = core_material**2 - clad_material**2
+    core_material = sqrt(na**2 + core_material**2)
 
     Args:
         period: fiber grating period in um.
         fill_factor: fraction of the grating period filled with the grating material.
         n_periods: number of periods.
         widths: Optional list of widths. Overrides period, fill_factor, n_periods.
         gaps: Optional list of gaps. Overrides period, fill_factor, n_periods.
         fiber_angle_deg: fiber angle in degrees.
         fiber_xposition: xposition.
         fiber_core_diameter: fiber diameter. 10.4 for Cband and 9.2um for Oband.
         fiber_numerical_aperture: NA.
-        fiber_nclad: fiber cladding index.
+        fiber_clad_material: fiber cladding index.
         nwg: waveguide index.
         nslab: slab refractive index.
-        nclad: top cladding index.
+        clad_material: top cladding index.
         nbox: box index bottom.
         nsubstrate: index substrate.
         pml_thickness: pml_thickness (um).
         substrate_thickness: substrate_thickness (um).
         box_thickness: thickness for bottom cladding (um).
-        wg_thickness: wg_thickness (um).
-        slab_thickness: slab thickness (um). etch_depth=wg_thickness-slab_thickness.
+        core_thickness: core_thickness (um).
+        slab_thickness: slab thickness (um). etch_depth=core_thickness-slab_thickness.
         top_clad_thickness: thickness of the top cladding.
         air_gap_thickness: air gap thickness.
         fiber_thickness: fiber_thickness.
         resolution: resolution pixels/um.
         wavelength_start: min wavelength (um).
         wavelength_stop: max wavelength (um).
         wavelength_points: wavelength points.
@@ -112,19 +112,19 @@
              /     /  /     /       |
             /     /  /     /        | fiber_thickness
            /     /  /     /    _ _ _| _ _ _ _ _ _  _
                                     |
                                     | air_gap_thickness
                                _ _ _| _ _ _ _ _ _  _
                                     |
-                   nclad            | top_clad_thickness
+                   clad_material            | top_clad_thickness
                 _   _   _      _ _ _| _ _ _ _ _ _  _
           nwg _| |_| |_| |__________|              _
                                     |               |
-                 nslab              |wg_thickness   | slab_thickness
+                 nslab              |core_thickness   | slab_thickness
                 ______________ _ _ _|_ _ _ _ _ _ _ _|
                                     |
                  nbox               |box_thickness
                 ______________ _ _ _|_ _ _ _ _ _ _ _
                                     |
                  nsubstrate         |substrate_thickness
                 ______________ _ _ _|
@@ -145,23 +145,23 @@
         gaps=gaps,
         n_periods=n_periods,
         nslab=nslab,
         fiber_angle_deg=fiber_angle_deg,
         fiber_xposition=fiber_xposition,
         fiber_core_diameter=fiber_core_diameter,
         fiber_numerical_aperture=fiber_numerical_aperture,
-        fiber_nclad=fiber_nclad,
+        fiber_clad_material=fiber_clad_material,
         nwg=nwg,
-        nclad=nclad,
+        clad_material=clad_material,
         nbox=nbox,
         nsubstrate=nsubstrate,
         pml_thickness=pml_thickness,
         substrate_thickness=substrate_thickness,
         box_thickness=box_thickness,
-        wg_thickness=wg_thickness,
+        core_thickness=core_thickness,
         top_clad_thickness=top_clad_thickness,
         air_gap_thickness=air_gap_thickness,
         fiber_thickness=fiber_thickness,
         resolution=resolution,
         wavelength_start=wavelength_start,
         wavelength_stop=wavelength_stop,
         wavelength_points=wavelength_points,
@@ -178,25 +178,25 @@
     fiber_angle = np.radians(fiber_angle_deg)
 
     # Z (Y)-domain
     sz = (
         +pml_thickness
         + substrate_thickness
         + box_thickness
-        + wg_thickness
+        + core_thickness
         + top_clad_thickness
         + air_gap_thickness
         + fiber_thickness
         + pml_thickness
     )
     # XY (X)-domain
     # Assume fiber port dominates
     fiber_port_y = (
         -sz / 2
-        + wg_thickness
+        + core_thickness
         + top_clad_thickness
         + air_gap_thickness
         + fiber_port_y_offset_from_air
     )
     fiber_port_x_offset_from_angle = np.abs(fiber_port_y * np.tan(fiber_angle))
     length_grating = np.sum(widths) + np.sum(gaps)
     sxy = (
@@ -205,67 +205,69 @@
         + 2 * fiber_port_x_offset_from_angle
         + length_grating
     )
 
     # Materials from indices
     slab_material = mp.Medium(index=nslab)
     wg_material = mp.Medium(index=nwg)
-    top_clad_material = mp.Medium(index=nclad)
+    top_clad_material = mp.Medium(index=clad_material)
     bottom_clad_material = mp.Medium(index=nbox)
-    fiber_ncore = (fiber_numerical_aperture**2 + fiber_nclad**2) ** 0.5
-    fiber_clad_material = mp.Medium(index=fiber_nclad)
-    fiber_core_material = mp.Medium(index=fiber_ncore)
+    fiber_core_material = (
+        fiber_numerical_aperture**2 + fiber_clad_material**2
+    ) ** 0.5
+    fiber_clad_material = mp.Medium(index=fiber_clad_material)
+    fiber_core_material = mp.Medium(index=fiber_core_material)
 
     # Useful reference point
     grating_start = (
         -fiber_xposition
     )  # Since fiber dominates, keep it centered and offset the grating
 
     # Initialize domain x-z plane simulation
     cell_size = mp.Vector3(sxy, sz)
 
     # Ports (position, sizes, directions)
     fiber_port_y = -sz / 2 + (
         +pml_thickness
         + substrate_thickness
         + box_thickness
-        + wg_thickness
+        + core_thickness
         + top_clad_thickness
         + air_gap_thickness
         + fiber_port_y_offset_from_air
     )
     fiber_port_center = mp.Vector3(fiber_port_x_offset_from_angle, fiber_port_y)
     fiber_port_x_size = fiber_port_x_size or 3.5 * fiber_core_diameter
     fiber_port_size = mp.Vector3(fiber_port_x_size, 0, 0)
     # fiber_port_direction = mp.Vector3(y=-1).rotate(mp.Vector3(z=1), -1 * fiber_angle)
 
     waveguide_port_y = -sz / 2 + (
         +pml_thickness
         + substrate_thickness
         + box_thickness / 2
-        + wg_thickness / 2
+        + core_thickness / 2
         + top_clad_thickness / 2
     )
     waveguide_port_x = grating_start - waveguide_port_x_offset_from_grating_start
     waveguide_port_center = mp.Vector3(
         waveguide_port_x, waveguide_port_y
     )  # grating_start - dtaper, 0)
     waveguide_port_size = mp.Vector3(
-        0, box_thickness + wg_thickness / 2 + top_clad_thickness
+        0, box_thickness + core_thickness / 2 + top_clad_thickness
     )
     waveguide_port_direction = mp.X
 
     # Geometry
     fiber_clad = 120
     hfiber_geom = 200  # Some large number to make fiber extend into PML
 
     geometry = [
         mp.Block(
             material=fiber_clad_material,
-            center=mp.Vector3(0, waveguide_port_y - wg_thickness / 2),
+            center=mp.Vector3(0, waveguide_port_y - core_thickness / 2),
             size=mp.Vector3(fiber_clad, hfiber_geom),
             e1=mp.Vector3(x=1).rotate(mp.Vector3(z=1), -1 * fiber_angle),
             e2=mp.Vector3(y=1).rotate(mp.Vector3(z=1), -1 * fiber_angle),
         )
     ]
 
     geometry.append(
@@ -285,15 +287,15 @@
             center=mp.Vector3(
                 0,
                 -sz / 2
                 + (
                     +pml_thickness
                     + substrate_thickness
                     + box_thickness
-                    + wg_thickness
+                    + core_thickness
                     + top_clad_thickness
                     + air_gap_thickness / 2
                 ),
             ),
             size=mp.Vector3(mp.inf, air_gap_thickness),
         )
     )
@@ -304,19 +306,19 @@
             center=mp.Vector3(
                 0,
                 -sz / 2
                 + (
                     +pml_thickness
                     + substrate_thickness
                     + box_thickness
-                    + wg_thickness / 2
+                    + core_thickness / 2
                     + top_clad_thickness / 2
                 ),
             ),
-            size=mp.Vector3(mp.inf, wg_thickness + top_clad_thickness),
+            size=mp.Vector3(mp.inf, core_thickness + top_clad_thickness),
         )
     )
     # Bottom cladding
     geometry.append(
         mp.Block(
             material=bottom_clad_material,
             center=mp.Vector3(
@@ -341,30 +343,30 @@
                     + slab_thickness / 2
                 ),
             ),
             size=mp.Vector3(mp.inf, slab_thickness),
         )
     )
 
-    etch_depth = wg_thickness - slab_thickness
+    etch_depth = core_thickness - slab_thickness
     x = grating_start
 
     # grating teeth
     for width, gap in zip(widths, gaps):
         geometry.append(
             mp.Block(
                 material=wg_material,
                 center=mp.Vector3(
                     x + gap / 2,
                     -sz / 2
                     + (
                         +pml_thickness
                         + substrate_thickness
                         + box_thickness
-                        + wg_thickness
+                        + core_thickness
                         - etch_depth / 2
                     ),
                 ),
                 size=mp.Vector3(width, etch_depth),
             )
         )
         x += width + gap
@@ -376,15 +378,15 @@
             center=mp.Vector3(
                 -sxy / 2,
                 -sz / 2
                 + (
                     +pml_thickness
                     + substrate_thickness
                     + box_thickness
-                    + wg_thickness
+                    + core_thickness
                     - etch_depth / 2
                 ),
             ),
             size=mp.Vector3(sxy, etch_depth),
         )
     )
 
@@ -556,25 +558,25 @@
         fill_factor=0.5,
         n_periods=30,
         # fiber parameters,
         fiber_angle_deg=20.0,
         fiber_xposition=0.0,
         fiber_core_diameter=9,
         fiber_numerical_aperture=fiber_na,
-        fiber_nclad=nSiO2,
+        fiber_clad_material=nSiO2,
         # material parameters
         nwg=3.47,
-        nclad=1.44,
+        clad_material=1.44,
         nbox=1.44,
         nsubstrate=3.47,
         # stack parameters
         pml_thickness=1.0,
         substrate_thickness=1.0,
         box_thickness=2.0,
-        wg_thickness=220 * nm,
+        core_thickness=220 * nm,
         top_clad_thickness=2.0,
         air_gap_thickness=1.0,
         fiber_thickness=2.0,
         # simulation parameters
         resolution=50,
     )
     plot(sim_dict["sim"], eps_parameters=eps_parameters)
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_eigenmode.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_materials.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/write_sparameters_grating.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 nm = 1e-3
 nSi = 3.48
 nSiO2 = 1.44
 
 Floats = Tuple[float, ...]
 
 
-def fiber_ncore(fiber_numerical_aperture, fiber_nclad):
-    return (fiber_numerical_aperture**2 + fiber_nclad**2) ** 0.5
+def fiber_core_material(fiber_numerical_aperture, fiber_clad_material):
+    return (fiber_numerical_aperture**2 + fiber_clad_material**2) ** 0.5
 
 
 def write_sparameters_grating(
     plot: bool = False,
     plot_contour: bool = False,
     animate: bool = False,
     overwrite: bool = False,
@@ -56,37 +56,37 @@
         plot: plot simulation (do not run).
         plot_contour: show contours.
         animate: create animation.
         overwrite: overwrites simulation if found.
         dirpath: directory path.
         decay_by: field decay to stop simulation.
         verbosity: print messages.
-        ncores: number of cores.
+        core_materials: number of cores.
 
     Keyword Args:
         period: fiber grating period in um.
         fill_factor: fraction of the grating period filled with the grating material.
         n_periods: number of periods.
         widths: Optional list of widths. Overrides period, fill_factor, n_periods.
         gaps: Optional list of gaps. Overrides period, fill_factor, n_periods.
         fiber_angle_deg: fiber angle in degrees.
         fiber_xposition: xposition.
         fiber_core_diameter: fiber diameter.
         fiber_numerical_aperture: NA.
-        fiber_nclad: fiber cladding index.
+        fiber_clad_material: fiber cladding index.
         nwg: waveguide index.
         nslab: slab refractive index.
-        nclad: top cladding index.
+        clad_material: top cladding index.
         nbox: box index bottom.
         nsubstrate: index substrate.
         pml_thickness: pml_thickness (um).
         substrate_thickness: substrate_thickness (um).
         box_thickness: thickness for bottom cladding (um).
-        wg_thickness: wg_thickness (um).
-        slab_thickness: slab thickness (um). etch_depth=wg_thickness-slab_thickness.
+        core_thickness: core_thickness (um).
+        slab_thickness: slab thickness (um). etch_depth=core_thickness-slab_thickness.
         top_clad_thickness: thickness of the top cladding.
         air_gap_thickness: air gap thickness.
         fiber_thickness: fiber_thickness.
         resolution: resolution pixels/um.
         wavelength_start: min wavelength (um).
         wavelength_stop: max wavelength (um).
         wavelength_points: wavelength points.
@@ -104,18 +104,18 @@
           /     /  /     /       |
          /     /  /     /        | fiber_thickness
         /     /  /     /    _ _ _| _ _ _ _ _ _  _
                                  |
                                  | air_gap_thickness
                             _ _ _| _ _ _ _ _ _  _
                                  |
-                nclad            | top_clad_thickness
+                clad_material            | top_clad_thickness
                             _ _ _| _ _ _ _ _ _  _
              _|-|_|-|_|-|___     |              _| etch_depth
-              ncore        |     |core_thickness
+              core_material        |     |core_thickness
              ______________|_ _ _|_ _ _ _ _ _ _ _
                                  |
               nbox               |box_thickness
              ______________ _ _ _|_ _ _ _ _ _ _ _
                                  |
               nsubstrate         |substrate_thickness
              ______________ _ _ _|
@@ -264,15 +264,15 @@
     # Save the component object to simulation for later retrieval
     temp_dir = temp_dir or pathlib.Path(__file__).parent / "temp"
     temp_dir = pathlib.Path(temp_dir)
     temp_dir.mkdir(exist_ok=True, parents=True)
     filepath = temp_dir / temp_file_str
 
     # Add parallelism info
-    instance["ncores"] = cores
+    instance["core_materials"] = cores
 
     # Write execution file
     script_lines = [
         "from gdsfactory.simulation.gmeep.write_sparameters_grating import write_sparameters_grating\n\n",
         'if __name__ == "__main__":\n\n',
         "\twrite_sparameters_grating(\n",
     ]
@@ -380,17 +380,17 @@
     #     fill_factor=0.5,
     #     n_periods=50,
     #     etch_depth=70 * nm,
     #     fiber_angle_deg=10.0,
     #     fiber_xposition=0.0,
     #     fiber_core_diameter=9,
     #     fiber_numerical_aperture=fiber_numerical_aperture,
-    #     fiber_nclad=1.43482,
-    #     ncore=3.47,
-    #     nclad=1.44,
+    #     fiber_clad_material=1.43482,
+    #     core_material=3.47,
+    #     clad_material=1.44,
     #     nbox=1.44,
     #     nsubstrate=3.47,
     #     pml_thickness=1.0,
     #     substrate_thickness=1.0,
     #     box_thickness=2.0,
     #     core_thickness=220 * nm,
     #     top_clad_thickness=2.0,
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/write_sparameters_meep.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from gdsfactory.simulation.gmeep.get_simulation import (
     get_simulation,
     settings_get_simulation,
 )
 from gdsfactory.technology import LayerStack
 from gdsfactory.typings import ComponentSpec, PathType, Port, PortSymmetries
 
-ncores = multiprocessing.cpu_count()
+core_materials = multiprocessing.cpu_count()
 
 
 def remove_simulation_kwargs(d: Dict[str, Any]) -> Dict[str, Any]:
     """Returns a copy of dict with only simulation settings.
 
     removes all flags for the simulator itself
     """
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 )
 from gdsfactory.simulation.gmeep.write_sparameters_meep import remove_simulation_kwargs
 from gdsfactory.simulation.gmeep.write_sparameters_meep_mpi import (
     write_sparameters_meep_mpi,
 )
 from gdsfactory.technology import LayerStack
 
-ncores = multiprocessing.cpu_count()
+core_materials = multiprocessing.cpu_count()
 
 temp_dir_default = Path(sparameters_path) / "temp"
 
 
 @pydantic.validate_arguments
 def write_sparameters_meep_batch(
     jobs: List[Dict],
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,29 +25,29 @@
     remove_simulation_kwargs,
     settings_write_sparameters_meep,
 )
 from gdsfactory.technology import LayerStack
 from gdsfactory.typings import ComponentSpec, PathType
 import pickle
 
-ncores = multiprocessing.cpu_count()
+core_materials = multiprocessing.cpu_count()
 
 temp_dir_default = Path(sparameters_path) / "temp"
 
 
 def _python() -> str:
     """Select correct python executable from current activated environment."""
     return sys.executable
 
 
 @pydantic.validate_arguments
 def write_sparameters_meep_mpi(
     component: ComponentSpec,
     layer_stack: Optional[LayerStack] = None,
-    cores: int = ncores,
+    cores: int = core_materials,
     filepath: Optional[PathType] = None,
     dirpath: Optional[PathType] = None,
     temp_dir: Path = temp_dir_default,
     temp_file_str: str = "write_sparameters_meep_mpi",
     live_output: bool = False,
     overwrite: bool = False,
     wait_to_finish: bool = True,
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/break_geometry.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/break_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/mesh.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/meshtracker.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/parse_component.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/parse_gds.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/parse_layerstack.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/parse_layerstack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/refine.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/refine.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/scratch/mesh3D.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/tests/test_meshing.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/uz_xsection_mesh.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/xy_xsection_mesh.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gmsh/xyz_mesh.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gmsh/xyz_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 [tidy3D is a fast GPU based commercial FDTD
 solver](https://simulation.cloud/)
 
 """
 
 from __future__ import annotations
 
-import tidy3d as td
+try:
+    import tidy3d as td
+except ModuleNotFoundError as e:
+    print("You need to 'pip install tidy3d'")
+    raise e
 
 from gdsfactory.config import logger
 from gdsfactory.simulation.gtidy3d import materials, modes, utils
 from gdsfactory.simulation.gtidy3d.get_results import get_results
 from gdsfactory.simulation.gtidy3d.get_simulation import (
     get_simulation,
     plot_simulation,
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/get_results.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/get_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/get_simulation.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                         |/
                  /              /       |
                 /  fiber_mfd   /        |
                /<------------>/    _ _ _| _ _ _ _ _ _ _
                                         |
                    clad_material        | fiber_z
                     _   _   _      _ _ _|_ _ _ _ _ _ _
-                   | | | | | |          ||wg_thickness
+                   | | | | | |          ||core_thickness
                   _| |_| |_| |__________||___
                                         || |
         waveguide            |          || | slab_thickness
               ____________________ _ _ _||_|_
                              |          |
                    box_material         |box_thickness
               _______________|____ _ _ _|_ _ _ _ _ _ _
@@ -282,18 +282,18 @@
 
     component_ref = component_padding.ref()
     component_ref.center = (0, 0)
 
     if len(layer_to_thickness) < 1:
         raise ValueError(f"{component.get_layers()} not in {layer_to_thickness.keys()}")
 
-    wg_thickness = max(layer_to_thickness.values())
+    core_thickness = max(layer_to_thickness.values())
     sim_xsize = component_ref.xsize + 2 * thickness_pml
     sim_zsize = (
-        thickness_pml + box_thickness + wg_thickness + thickness_pml + 2 * zmargin
+        thickness_pml + box_thickness + core_thickness + thickness_pml + 2 * zmargin
     )
     sim_ysize = component_ref.ysize + 2 * thickness_pml if is_3d else 0
     sim_size = [
         sim_xsize,
         sim_ysize,
         sim_zsize,
     ]
@@ -384,21 +384,21 @@
     angle = port.orientation
     width = port.width + 2 * port_margin
     size_x = width * abs(np.sin(angle * np.pi / 180))
     size_y = width * abs(np.cos(angle * np.pi / 180))
     size_x = 0 if size_x < 0.001 else size_x
     size_y = 0 if size_y < 0.001 else size_y
     size_y = size_y if is_3d else td.inf
-    size_z = wg_thickness + zmargin + box_thickness
+    size_z = core_thickness + zmargin + box_thickness
     waveguide_port_size = [size_x, size_y, size_z]
     xy_shifted = move_polar_rad_copy(
         np.array(port.center), angle=angle * np.pi / 180, length=port_waveguide_offset
     )
     waveguide_port_center = xy_shifted.tolist() + [
-        (wg_thickness + zmargin - box_thickness) / 2
+        (core_thickness + zmargin - box_thickness) / 2
     ]  # (x, y, z)
 
     waveguide_monitor = td.ModeMonitor(
         center=waveguide_port_center,
         size=waveguide_port_size,
         freqs=freqs,
         mode_spec=td.ModeSpec(num_modes=1),
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/materials.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/sim_run.yaml` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_results.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_simulation.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/utils.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/write_sparameters.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/lumerical/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/lumerical/interconnect.py` & `gdsfactory-6.93.0/gdsfactory/simulation/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/lumerical/read.py` & `gdsfactory-6.93.0/gdsfactory/simulation/lumerical/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/lumerical/settings.py` & `gdsfactory-6.93.0/gdsfactory/simulation/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/lumerical/test_read_sparameters.py` & `gdsfactory-6.93.0/gdsfactory/simulation/lumerical/test_read_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py` & `gdsfactory-6.93.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py` & `gdsfactory-6.93.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/coupler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/coupler.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,59 +7,59 @@
     find_coupling,
     find_coupling_vs_gap,
 )
 
 PATH = pathlib.Path(__file__).parent.absolute() / "modes"
 
 nm = 1e-3
-wg_thickness = 220 * nm
+core_thickness = 220 * nm
 nitride_thickness = 400 * nm
 slab_thickness = 90 * nm
 strip_width = 500 * nm
 rib_width = 550 * nm
 
 
 find_coupling_strip = gf.partial(
     find_coupling,
-    wg_width=strip_width,
-    wg_thickness=wg_thickness,
+    core_width=strip_width,
+    core_thickness=core_thickness,
     slab_thickness=0.0,
 )
 find_coupling_rib = gf.partial(
     find_coupling,
-    wg_width=rib_width,
-    wg_thickness=wg_thickness,
+    core_width=rib_width,
+    core_thickness=core_thickness,
     slab_thickness=slab_thickness,
 )
 find_coupling_nitride = gf.partial(
     find_coupling,
-    wg_width=1.0,
+    core_width=1.0,
     slab_thickness=0.0,
-    ncore=2.0,
-    wg_thickness=nitride_thickness,
+    core_material=2.0,
+    core_thickness=nitride_thickness,
     sz=4,
     ymargin=4,
 )
 
 
 find_coupling_vs_gap_strip = gf.partial(
     find_coupling_vs_gap,
 )
 find_coupling_vs_gap_rib = gf.partial(
     find_coupling_vs_gap,
-    wg_width=rib_width,
-    wg_thickness=wg_thickness,
+    core_width=rib_width,
+    core_thickness=core_thickness,
     slab_thickness=slab_thickness,
 )
 find_coupling_vs_gap_nitride = gf.partial(
     find_coupling_vs_gap,
-    wg_width=1.0,
+    core_width=1.0,
     slab_thickness=0.0,
-    ncore=2.0,
-    wg_thickness=nitride_thickness,
+    core_material=2.0,
+    core_thickness=nitride_thickness,
     sz=4,
     ymargin=4,
     gap1=300 * nm,
     gap2=600 * nm,
 )
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/find_coupling_vs_gap.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,29 +78,29 @@
         nmodes: number of modes.
         wavelength: wavelength (um).
         parity: for symmetries.
         filepath: optional filepath to cache results on disk.
         overwrite: overwrites results even if found on disk.
 
     Keyword Args:
-        wg_width: wg_width (um) for the symmetric case.
+        core_width: core_width (um) for the symmetric case.
         gap: for the case of only two waveguides.
-        wg_widths: list or tuple of waveguide widths.
+        core_widths: list or tuple of waveguide widths.
         gaps: list or tuple of waveguide gaps.
-        wg_thickness: wg height (um)
+        core_thickness: wg height (um)
         slab_thickness: thickness for the waveguide slab
-        ncore: core material refractive index
-        nclad: clad material refractive index
-        nslab: Optional slab material refractive index. Defaults to ncore.
+        core_material: core material refractive index
+        clad_material: clad material refractive index
+        nslab: Optional slab material refractive index. Defaults to core_material.
         ymargin: margin in y.
         sz: simulation region thickness (um).
         resolution: resolution (pixels/um).
         nmodes: number of modes.
         sidewall_angles: waveguide sidewall angle (radians),
-            tapers from wg_width at top of slab, upwards, to top of waveguide.
+            tapers from core_width at top of slab, upwards, to top of waveguide.
 
     """
     if filepath and not overwrite and pathlib.Path(filepath).exists():
         return pd.read_csv(filepath)
 
     gaps = np.linspace(gap1, gap2, steps)
     ne = []
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/find_mode_dispersion.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/find_mode_dispersion.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         wavelength: center wavelength (um).
         wavelength_step: in um.
         core: core material name.
         clad: clad material name.
         mode_number: mode index to compute (1: fundamental mode).
 
     Keyword Args:
-        wg_thickness: wg height (um).
+        core_thickness: wg height (um).
         sx: supercell width (um).
         sy: supercell height (um).
         resolution: (pixels/um).
         wavelength: wavelength.
         num_bands: mode order.
         plot: if True plots mode.
         logscale: plots in logscale.
@@ -43,36 +43,51 @@
         parity: symmetries mp.ODD_Y mp.EVEN_X for TE, mp.EVEN_Y for TM.
 
     """
     w0 = wavelength - wavelength_step
     wc = wavelength
     w1 = wavelength + wavelength_step
 
-    ncore = partial(get_index, name=core)
-    nclad = partial(get_index, name=clad)
+    core_material = partial(get_index, name=core)
+    clad_material = partial(get_index, name=clad)
 
-    m0 = find_modes_waveguide(wavelength=w0, ncore=ncore(w0), nclad=nclad(w0), **kwargs)
-    mc = find_modes_waveguide(wavelength=wc, ncore=ncore(wc), nclad=nclad(wc), **kwargs)
-    m1 = find_modes_waveguide(wavelength=w1, ncore=ncore(w1), nclad=nclad(w1), **kwargs)
+    m0 = find_modes_waveguide(
+        wavelength=w0,
+        core_material=core_material(w0),
+        clad_material=clad_material(w0),
+        **kwargs,
+    )
+    mc = find_modes_waveguide(
+        wavelength=wc,
+        core_material=core_material(wc),
+        clad_material=clad_material(wc),
+        **kwargs,
+    )
+    m1 = find_modes_waveguide(
+        wavelength=w1,
+        core_material=core_material(w1),
+        clad_material=clad_material(w1),
+        **kwargs,
+    )
 
     n0 = m0[mode_number].neff
     nc = mc[mode_number].neff
     n1 = m1[mode_number].neff
 
     # ng = ncenter - wavelength *dn/ step
     ng = nc - wavelength * (n1 - n0) / (2 * wavelength_step)
     neff = (n0 + nc + n1) / 3
     return Mode(mode_number=mode_number, ng=ng, neff=neff, wavelength=wavelength)
 
 
 if __name__ == "__main__":
-    m = find_mode_dispersion(wg_width=0.45, wg_thickness=0.22)
+    m = find_mode_dispersion(core_width=0.45, core_thickness=0.22)
     print(m.ng)
     # test_ng()
     # print(get_index(name="Si"))
     # ngs = []
     # for wavelength_step in [0.001, 0.01]:
     #     neff, ng = find_modes_waveguide_dispersion(
-    #         wg_width=0.45, wg_thickness=0.22, wavelength_step=wavelength_step
+    #         core_width=0.45, core_thickness=0.22, wavelength_step=wavelength_step
     #     )
     #     ngs.append(ng)
     #     print(wavelength_step, ng)
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/find_modes.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/find_modes.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,20 +49,20 @@
           __________________________
           |
           |
           |         width
           |     <---------->
           |      ___________   _ _ _
           |     |           |       |
-        sz|_____|  ncore    |_______|
-          |                         | wg_thickness
+        sz|_____|           |_______|
+          |     core_material       | core_thickness
           |slab_thickness    nslab  |
           |_________________________|
           |
-          |        nclad
+          |        clad_material
           |__________________________
           <------------------------>
                         sy
 
     single_waveguide=False
 
     ::
@@ -70,21 +70,21 @@
           _____________________________________________________
           |
           |
           |         widths[0]                 widths[1]
           |     <---------->     gaps[0]    <---------->
           |      ___________ <-------------> ___________      _
           |     |           |               |           |     |
-        sz|_____|  ncore    |_______________|           |_____|
-          |                                                   | wg_thickness
+        sz|_____|           |_______________|           |_____|
+          |    core_material                                  | core_thickness
           |slab_thickness        nslab                        |
           |___________________________________________________|
           |
           |<--->                                         <--->
-          |ymargin               nclad                   ymargin
+          |ymargin               clad_material                   ymargin
           |____________________________________________________
           <--------------------------------------------------->
                                    sy
 
     Args:
         mode_solver: function that returns mpb.ModeSolver.
         tol: tolerance when finding modes.
@@ -92,40 +92,40 @@
         mode_number: mode order of the first mode.
         parity: mp.ODD_Y mp.EVEN_X for TE, mp.EVEN_Y for TM.
         cache: directory path to cache modes. None disables the file cache.
         overwrite: forces simulating again.
         kwargs: waveguide settings.
 
     Keyword Args:
-        wg_width: wg_width (um).
-        wg_thickness: wg height (um).
+        core_width: core_width (um).
+        core_thickness: wg height (um).
         slab_thickness: thickness for the waveguide slab.
-        ncore: core material refractive index.
-        nclad: clad material refractive index.
+        core_material: core material refractive index.
+        clad_material: clad material refractive index.
         sy: simulation region width (um).
         sz: simulation region height (um).
         resolution: resolution (pixels/um).
         nmodes: number of modes to compute.
 
     Keyword Args:
-        wg_width: wg_width (um) for the symmetric case.
+        core_width: core_width (um) for the symmetric case.
         gap: for the case of only two waveguides.
-        wg_widths: list or tuple of waveguide widths.
+        core_widths: list or tuple of waveguide widths.
         gaps: list or tuple of waveguide gaps.
-        wg_thickness: wg height (um).
+        core_thickness: wg height (um).
         slab_thickness: thickness for the waveguide slab.
-        ncore: core material refractive index.
-        nclad: clad material refractive index.
-        nslab: Optional slab material refractive index. Defaults to ncore.
+        core_material: core material refractive index.
+        clad_material: clad material refractive index.
+        nslab: Optional slab material refractive index. Defaults to core_material.
         ymargin: margin in y.
         sz: simulation region thickness (um).
         resolution: resolution (pixels/um).
         nmodes: number of modes.
         sidewall_angles: waveguide sidewall angle (radians),
-            tapers from wg_width at top of slab, upwards, to top of waveguide.
+            tapers from core_width at top of slab, upwards, to top of waveguide.
 
     Returns: Dict[mode_number, Mode]
 
     compute mode_number lowest frequencies as a function of k. Also display
     "parities", i.e. whether the mode is symmetric or anti_symmetric
     through the y=0 and z=0 planes.
     mode_solver.run(mpb.display_yparities, mpb.display_zparities)
@@ -219,15 +219,15 @@
     return modes
 
 
 find_modes_coupler = partial(find_modes_waveguide, single_waveguide=False)
 
 
 if __name__ == "__main__":
-    m = find_modes_waveguide(wg_width=0.5)
+    m = find_modes_waveguide(core_width=0.5)
     print(m)
 
     m1 = m[1]
 
     # print(np.shape(m1.y))
     # print(np.shape(m1.z))
     # print(np.shape(m1.E[:, :, 0, 1]))
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/find_modes_cross_section.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/find_modes_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         wavelength: center wavelength (um).
         steps: number of steps to sweep in width and thickness.
         mode_number: mode index to compute (1: fundamental mode).
         core: core material name.
         clad: clad material name.
 
     Keyword Args:
-        wg_thickness: wg height (um).
+        core_thickness: wg height (um).
         sx: supercell width (um).
         sy: supercell height (um).
         resolution: (pixels/um).
         wavelength: wavelength in um.
         num_bands: mode order.
         plot: if True plots mode.
         logscale: plots in logscale.
@@ -76,16 +76,16 @@
     dws = []
 
     for dwi in dw:
         for dhi in dh:
             m = find_mode_dispersion(
                 core=core,
                 clad=clad,
-                wg_width=width + dwi,
-                wg_thickness=thickness + dhi,
+                core_width=width + dwi,
+                core_thickness=thickness + dhi,
                 wavelength=wavelength,
                 mode_number=mode_number,
                 **kwargs,
             )
             neffs.append(m.neff)
             ngs.append(m.ng)
             dws.append(dwi)
@@ -108,15 +108,15 @@
         thickness: waveguide thickness in um.
         wavelength: in um.
         mode_number: 1 is the fundamental first order mode.
 
     """
     filepath = pathlib.Path(PATH.modes / "mpb_dw_dh_dispersion.csv")
     m = find_mode_dispersion(
-        wg_width=width, wg_thickness=thickness, wavelength=wavelength
+        core_width=width, core_thickness=thickness, wavelength=wavelength
     )
     neff0 = m.neff
     ng0 = m.ng
 
     if filepath.exists():
         df = pd.read_csv(filepath)
     else:
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/find_neff_vs_width.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/find_neff_vs_width.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,32 +36,32 @@
         parity: mp.ODD_Y mp.EVEN_X for TE, mp.EVEN_Y for TM.
         filepath: Optional filepath to store the results.
         overwrite: overwrite file even if exists on disk.
 
 
     Keyword Args:
         slab_thickness: thickness for the waveguide slab in um.
-        ncore: core material refractive index.
-        nclad: clad material refractive index.
+        core_material: core material refractive index.
+        clad_material: clad material refractive index.
         sy: simulation region width (um).
         sz: simulation region height (um).
         resolution: resolution (pixels/um).
 
     """
     if filepath and not overwrite and pathlib.Path(filepath).exists():
         return pd.read_csv(filepath)
 
     width = np.linspace(width1, width2, steps)
     neff = {mode_number: [] for mode_number in range(1, nmodes + 1)}
-    for wg_width in tqdm(width):
+    for core_width in tqdm(width):
         modes = find_modes_waveguide(
             wavelength=wavelength,
             parity=parity,
             nmodes=nmodes,
-            wg_width=wg_width,
+            core_width=core_width,
             **kwargs,
         )
         for mode_number in range(1, nmodes + 1):
             mode = modes[mode_number]
             neff[mode_number].append(mode.neff)
 
     df = pd.DataFrame(neff)
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/get_mode_solver_coupler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,120 +15,120 @@
 tmp.mkdir(exist_ok=True)
 
 Floats = Tuple[float, ...]
 
 
 @pydantic.validate_arguments
 def get_mode_solver_coupler(
-    wg_width: float = 0.5,
+    core_width: float = 0.5,
     gap: float = 0.2,
-    wg_widths: Optional[Floats] = None,
+    core_widths: Optional[Floats] = None,
     gaps: Optional[Floats] = None,
-    wg_thickness: float = 0.22,
+    core_thickness: float = 0.22,
     slab_thickness: float = 0.0,
-    ncore: float = 3.47,
-    nclad: float = 1.44,
+    core_material: float = 3.47,
+    clad_material: float = 1.44,
     nslab: Optional[float] = None,
     ymargin: float = 2.0,
     sz: float = 2.0,
     resolution: int = 32,
     nmodes: int = 4,
     sidewall_angles: Union[Tuple[float, ...], float] = None,
 ) -> mpb.ModeSolver:
     """Returns mode_solver simulation.
 
     Args:
-        wg_width: wg_width (um) for the symmetric case.
+        core_width: core_width (um) for the symmetric case.
         gap: for the case of only two waveguides.
-        wg_widths: list or tuple of waveguide widths.
+        core_widths: list or tuple of waveguide widths.
         gaps: list or tuple of waveguide gaps.
-        wg_thickness: wg thickness (um).
+        core_thickness: wg thickness (um).
         slab_thickness: thickness for the waveguide slab.
-        ncore: core material refractive index.
-        nclad: clad material refractive index.
-        nslab: Optional slab material refractive index. Defaults to ncore.
+        core_material: core material refractive index.
+        clad_material: clad material refractive index.
+        nslab: Optional slab material refractive index. Defaults to core_material.
         ymargin: margin in y.
         sz: simulation region thickness (um).
         resolution: resolution (pixels/um).
         nmodes: number of modes.
         sidewall_angles: waveguide sidewall angle (degrees),
-            tapers from wg_width at top of slab, upwards, to top of waveguide
+            tapers from core_width at top of slab, upwards, to top of waveguide
             a sidewall_angle = 10, will have 80 degrees with respect to the substrate.
 
     ::
 
           _____________________________________________________
           |
           |
           |         widths[0]                 widths[1]
           |     <---------->     gaps[0]    <---------->
           |      ___________ <-------------> ___________      _
           |     |           |               |           |     |
-        sz|_____|  ncore    |_______________|           |_____|
-          |                                                   | wg_thickness
+        sz|_____|  core_material    |_______________|           |_____|
+          |                                                   | core_thickness
           |slab_thickness        nslab                        |
           |___________________________________________________|
           |
           |<--->                                         <--->
-          |ymargin               nclad                   ymargin
+          |ymargin               clad_material                   ymargin
           |____________________________________________________
           <--------------------------------------------------->
                                    sy
 
     """
-    wg_widths = wg_widths or (wg_width, wg_width)
+    core_widths = core_widths or (core_width, core_width)
     gaps = gaps or (gap,)
-    material_core = mp.Medium(index=ncore)
-    material_clad = mp.Medium(index=nclad)
-    material_slab = mp.Medium(index=nslab or ncore)
+    material_core = mp.Medium(index=core_material)
+    material_clad = mp.Medium(index=clad_material)
+    material_slab = mp.Medium(index=nslab or core_material)
 
     # Define the computational cell.  We'll make x the propagation direction.
     # the other cell sizes should be big enough so that the boundaries are
     # far away from the mode field.
 
-    sy = np.sum(wg_widths) + np.sum(gaps) + 2 * ymargin
+    sy = np.sum(core_widths) + np.sum(gaps) + 2 * ymargin
     geometry_lattice = mp.Lattice(size=mp.Vector3(0, sy, sz))
 
     geometry = []
 
     y = -sy / 2 + ymargin
 
     gaps = list(gaps) + [0]
-    for i, wg_width in enumerate(wg_widths):
+    for i, core_width in enumerate(core_widths):
         if sidewall_angles:
             geometry.append(
                 mp.Prism(
                     vertices=[
                         mp.Vector3(y=y, z=slab_thickness),
-                        mp.Vector3(y=y + wg_width, z=slab_thickness),
-                        mp.Vector3(x=1, y=y + wg_width, z=slab_thickness),
+                        mp.Vector3(y=y + core_width, z=slab_thickness),
+                        mp.Vector3(x=1, y=y + core_width, z=slab_thickness),
                         mp.Vector3(x=1, y=y, z=slab_thickness),
                     ],
-                    height=wg_thickness - slab_thickness,
+                    height=core_thickness - slab_thickness,
                     center=mp.Vector3(
-                        y=y + wg_width / 2,
-                        z=slab_thickness + (wg_thickness - slab_thickness) / 2,
+                        y=y + core_width / 2,
+                        z=slab_thickness + (core_thickness - slab_thickness) / 2,
                     ),
                     # If only 1 angle is specified, use it for all waveguides
                     sidewall_angle=np.deg2rad(sidewall_angles)
                     if len(np.unique(sidewall_angles)) == 1
                     else np.deg2rad(sidewall_angles[i]),
                     material=material_core,
                 )
             )
         else:
             geometry.append(
                 mp.Block(
-                    size=mp.Vector3(mp.inf, wg_width, wg_thickness),
+                    size=mp.Vector3(mp.inf, core_width, core_thickness),
                     material=material_core,
-                    center=mp.Vector3(y=y + wg_width / 2, z=wg_thickness / 2),
+                    center=mp.Vector3(y=y + core_width / 2, z=core_thickness / 2),
                 )
             )
 
-        y += gaps[i] + wg_width
+        y += gaps[i] + core_width
 
     # define the 2D blocks for the strip and substrate
     geometry += [
         mp.Block(
             size=mp.Vector3(mp.inf, mp.inf, slab_thickness),
             material=material_slab,
             center=mp.Vector3(z=slab_thickness / 2),
@@ -143,37 +143,37 @@
     k_points = mp.interpolate(num_k, [mp.Vector3(k_min), mp.Vector3(k_max)])
 
     # Increase this to see more modes.  (The guided ones are the ones below the
     # light line, i.e. those with frequencies < kmag / 1.45, where kmag
     # is the corresponding column in the output if you grep for "freqs:".)
     # use this prefix for output files
 
-    wg_widths_str = "_".join([str(i) for i in wg_widths])
+    core_widths_str = "_".join([str(i) for i in core_widths])
     gaps_str = "_".join([str(i) for i in gaps])
     filename_prefix = (
-        tmp / f"coupler_{wg_widths_str}_{gaps_str}_{wg_thickness}_{slab_thickness}"
+        tmp / f"coupler_{core_widths_str}_{gaps_str}_{core_thickness}_{slab_thickness}"
     )
 
     mode_solver = mpb.ModeSolver(
         geometry_lattice=geometry_lattice,
         geometry=geometry,
         k_points=k_points,
         resolution=resolution,
         num_bands=nmodes,
         filename_prefix=str(filename_prefix),
         default_material=material_clad,
     )
     mode_solver.nmodes = nmodes
     mode_solver.info = dict(
-        wg_widths=wg_widths,
+        core_widths=core_widths,
         gaps=gaps,
-        wg_thickness=wg_thickness,
+        core_thickness=core_thickness,
         slab_thickness=slab_thickness,
-        ncore=ncore,
-        nclad=nclad,
+        core_material=core_material,
+        clad_material=clad_material,
         sy=sy,
         sz=sz,
         resolution=resolution,
         nmodes=nmodes,
     )
     return mode_solver
 
@@ -181,15 +181,15 @@
 if __name__ == "__main__":
     import matplotlib.pyplot as plt
 
     m = get_mode_solver_coupler(
         slab_thickness=90e-3,
         nslab=2,
         gap=0.5,
-        wg_width=1,
+        core_width=1,
         resolution=64,
         sidewall_angles=(10.0, 20.0),
     )
     m.init_params(p=mp.NO_PARITY, reset_fields=False)
     eps = m.get_epsilon()
     # cmap = 'viridis'
     # cmap = "RdBu"
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/get_mode_solver_cross_section.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/get_mode_solver_rib.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/get_mode_solver_rib.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,93 +13,93 @@
 
 tmp = pathlib.Path(tempfile.TemporaryDirectory().name).parent / "meep"
 tmp.mkdir(exist_ok=True)
 
 
 @pydantic.validate_arguments
 def get_mode_solver_rib(
-    wg_width: float = 0.45,
-    wg_thickness: float = 0.22,
+    core_width: float = 0.45,
+    core_thickness: float = 0.22,
     slab_thickness: float = 0.0,
-    ncore: float = 3.47,
-    nclad: float = 1.44,
+    core_material: float = 3.47,
+    clad_material: float = 1.44,
     nslab: Optional[float] = None,
     sy: float = 2.0,
     sz: float = 2.0,
     resolution: int = 32,
     nmodes: int = 4,
     sidewall_angle: Optional[float] = None,
 ) -> mpb.ModeSolver:
     """Returns a mode_solver simulation.
 
     Args:
-        wg_width: wg_width (um).
-        wg_thickness: wg thickness (um).
+        core_width: core_width (um).
+        core_thickness: wg thickness (um).
         slab_thickness: thickness for the waveguide slab.
-        ncore: core material refractive index.
-        nclad: clad material refractive index.
-        nslab: Optional slab material refractive index. Defaults to ncore.
+        core_material: core material refractive index.
+        clad_material: clad material refractive index.
+        nslab: Optional slab material refractive index. Defaults to core_material.
         sy: simulation region width (um).
         sz: simulation region height (um).
         resolution: resolution (pixels/um).
         nmodes: number of modes.
         sidewall_angle: waveguide sidewall angle (degrees),
-            tapers from wg_width at top of slab, upwards, to top of waveguide
+            tapers from core_width at top of slab, upwards, to top of waveguide
             with respect to the normal.
             a sidewall_angle = 10, will have 80 degrees with respect to the substrate.
 
     ::
 
           __________________________
           |
           |
           |         width
           |     <---------->
           |      ___________   _ _ _
           |     |           |       |
-        sz|_____|  ncore    |_______|
-          |                         | wg_thickness
+        sz|_____|  core_material    |_______|
+          |                         | core_thickness
           |slab_thickness    nslab  |
           |_________________________|
           |
-          |        nclad
+          |        clad_material
           |__________________________
           <------------------------>
                         sy
 
     """
-    material_core = mp.Medium(index=ncore)
-    material_clad = mp.Medium(index=nclad)
-    material_slab = mp.Medium(index=nslab or ncore)
+    material_core = mp.Medium(index=core_material)
+    material_clad = mp.Medium(index=clad_material)
+    material_slab = mp.Medium(index=nslab or core_material)
 
     # Define the computational cell.  We'll make x the propagation direction.
     # the other cell sizes should be big enough so that the boundaries are
     # far away from the mode field.
     geometry_lattice = mp.Lattice(size=mp.Vector3(0, sy, sz))
 
     geometry = []
     if sidewall_angle:
         geometry.append(
             mp.Prism(
                 vertices=[
-                    mp.Vector3(y=-wg_width / 2, z=0),
-                    mp.Vector3(y=wg_width / 2, z=0),
-                    mp.Vector3(x=1, y=wg_width / 2, z=0),
-                    mp.Vector3(x=1, y=-wg_width / 2, z=0),
+                    mp.Vector3(y=-core_width / 2, z=0),
+                    mp.Vector3(y=core_width / 2, z=0),
+                    mp.Vector3(x=1, y=core_width / 2, z=0),
+                    mp.Vector3(x=1, y=-core_width / 2, z=0),
                 ],
-                height=wg_thickness - slab_thickness,
+                height=core_thickness - slab_thickness,
                 center=mp.Vector3(z=0),
                 sidewall_angle=np.deg2rad(sidewall_angle),
                 material=material_core,
             )
         )
     else:
         geometry.append(
             mp.Block(
-                size=mp.Vector3(mp.inf, wg_width, wg_thickness),
+                size=mp.Vector3(mp.inf, core_width, core_thickness),
                 material=material_core,
                 center=mp.Vector3(z=0),
             )
         )
 
     geometry += [
         mp.Block(
@@ -117,47 +117,47 @@
     k_points = mp.interpolate(num_k, [mp.Vector3(k_min), mp.Vector3(k_max)])
 
     # Increase this to see more modes.  (The guided ones are the ones below the
     # light line, i.e. those with frequencies < kmag / 1.45, where kmag
     # is the corresponding column in the output if you grep for "freqs:".)
     # use this prefix for output files
 
-    filename_prefix = tmp / f"rib_{wg_width}_{wg_thickness}_{slab_thickness}"
+    filename_prefix = tmp / f"rib_{core_width}_{core_thickness}_{slab_thickness}"
 
     mode_solver = mpb.ModeSolver(
         geometry_lattice=geometry_lattice,
         geometry=geometry,
         k_points=k_points,
         resolution=resolution,
         num_bands=nmodes,
         default_material=material_clad,
         filename_prefix=str(filename_prefix),
     )
     mode_solver.nmodes = nmodes
     mode_solver.info = dict(
-        wg_width=wg_width,
-        wg_thickness=wg_thickness,
+        core_width=core_width,
+        core_thickness=core_thickness,
         slab_thickness=slab_thickness,
-        ncore=ncore,
-        nclad=nclad,
+        core_material=core_material,
+        clad_material=clad_material,
         sy=sy,
         sz=sz,
         resolution=resolution,
         nmodes=nmodes,
     )
     return mode_solver
 
 
 if __name__ == "__main__":
     import matplotlib.pyplot as plt
 
     m = get_mode_solver_rib(
         slab_thickness=0.25,
         # slab_thickness=0.,
-        wg_thickness=0.5,
+        core_thickness=0.5,
         resolution=64,
         nslab=2,
     )
     m.init_params(p=mp.NO_PARITY, reset_fields=False)
     eps = m.get_epsilon()
     # cmap = 'viridis'
     # cmap = "RdBu"
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/neff_convergence_test.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/neff_convergence_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,19 @@
         parity: mp.ODD_Y mp.EVEN_X for TE, mp.EVEN_Y for TM.
         rel_conv_tol: relative tolerance on hyperparameters
             (# decimal places; cannot be too demanding, since solver is iterative).
         rel_conv_step: relative increase in hyperparameters from initial values
         stdout: convergence test output.
 
     Keyword Args:
-        wg_width: wg_width (um).
-        wg_thickness: wg height (um).
+        core_width: core_width (um).
+        core_thickness: wg height (um).
         slab_thickness: thickness for the waveguide slab.
-        ncore: core material refractive index.
-        nclad: clad material refractive index.
+        core_material: core material refractive index.
+        clad_material: clad material refractive index.
         sy: INITIAL simulation region width (um).
         sz: INITIAL simulation region height (um).
         resolution: INITIAL resolution (pixels/um).
         nmodes: number of modes.
         tol: tolerance when finding modes.
         wavelength: wavelength.
         mode_number: mode order of the first mode.
@@ -140,19 +140,19 @@
         parity: mp.ODD_Y mp.EVEN_X for TE, mp.EVEN_Y for TM.
         rel_conv_tol: relative tolerance on hyperparameters (# decimal places;
             cannot be too demanding, since solver is iterative)
         rel_conv_step: relative increase in hyperparameters from initial values
         stdout: convergence test output
 
     Keyword Args:
-        wg_width: wg_width (um)
-        wg_thickness: wg height (um)
+        core_width: core_width (um)
+        core_thickness: wg height (um)
         slab_thickness: thickness for the waveguide slab
-        ncore: core material refractive index
-        nclad: clad material refractive index
+        core_material: core material refractive index
+        clad_material: clad material refractive index
         sy: INITIAL simulation region width (um)
         sz: INITIAL simulation region height (um)
         resolution: INITIAL resolution (pixels/um)
         nmodes: number of modes
         tol: tolerance when finding modes,
         wavelength: wavelength,
         mode_number: mode order of the first mode,
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/overlap.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_find_modes.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_find_modes.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 
 import numpy as np
 
 from gdsfactory.simulation.modes.find_modes import find_modes_waveguide
 
 
 def test_find_modes_waveguide() -> None:
-    modes = find_modes_waveguide(wg_width=0.45, resolution=20, cache=None)
+    modes = find_modes_waveguide(core_width=0.45, resolution=20, cache=None)
     m1 = modes[1]
     m2 = modes[2]
 
     # neff1 = 2.3815558509779744
     # neff2 = 1.7749644180250004
 
     neff1 = 2.3494603726390664
     neff2 = 1.7030929743774146
 
     assert np.isclose(m1.neff, neff1), m1.neff
     assert np.isclose(m2.neff, neff2), m2.neff
 
     # Using cache
-    modes = find_modes_waveguide(wg_width=0.45, resolution=20)
+    modes = find_modes_waveguide(core_width=0.45, resolution=20)
     m1 = modes[1]
     m2 = modes[2]
 
     assert np.isclose(m1.neff, neff1), m1.neff
     assert np.isclose(m2.neff, neff2), m2.neff
 
 
 if __name__ == "__main__":
     test_find_modes_waveguide()
-    # ms = get_mode_solver_rib(wg_width=0.45)
+    # ms = get_mode_solver_rib(core_width=0.45)
     # modes = find_neff(mode_solver=ms)
     # m1 = modes[1]
     # m2 = modes[2]
     # print(m1.neff)
     # print(m2.neff)
     # neff1 = 2.342628111145838
     # neff2 = 1.7286034634949181
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 
 from gdsfactory.simulation.modes.find_mode_dispersion import find_mode_dispersion
 
 
 def test_find_modes_waveguide_dispersion() -> None:
-    modes = find_mode_dispersion(wg_width=0.45, resolution=20, cache=None)
+    modes = find_mode_dispersion(core_width=0.45, resolution=20, cache=None)
     m1 = modes
 
     # print(f"neff1 = {m1.neff}")
     # print(f"ng1 = {m1.ng}")
 
     # neff1 = 2.3948
     # ng1 = 4.23194
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/types.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,32 +429,32 @@
         plt.show()
 
 
 class Waveguide(BaseModel):
     """Waveguide Model.
 
     Args:
-        wg_width: um
-        wg_thickness: um
+        core_width: um
+        core_thickness: um
         slab_thickness: um
-        ncore: core refractive index.
-        nclad: cladding refractive index.
+        core_material: core refractive index.
+        clad_material: cladding refractive index.
         sy: float
         sz: float
         resolution: int
         nmodes: int
         modes: Dict[Mode]
 
     """
 
-    wg_width: float = 0.45
-    wg_thickness: float = 0.22
+    core_width: float = 0.45
+    core_thickness: float = 0.22
     slab_thickness: float = 0
-    ncore: float = 3.47
-    nclad: float = 1.44
+    core_material: float = 3.47
+    clad_material: float = 1.44
     sy: float = 2.0
     sz: float = 2.0
     resolution: int = 32
     nmodes: int = 4
     modes: Optional[Dict[int, Mode]] = None
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/modes/waveguide.py` & `gdsfactory-6.93.0/gdsfactory/simulation/modes/waveguide.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 
 import gdsfactory as gf
 from gdsfactory.simulation.modes.find_neff_vs_width import find_neff_vs_width
 
 PATH = pathlib.Path(__file__).parent.absolute() / "modes"
 
 nm = 1e-3
-wg_thickness_silicon = 220 * nm
-wg_thickness_nitride = 400 * nm
+core_thickness_silicon = 220 * nm
+core_thickness_nitride = 400 * nm
 
 
 find_neff_vs_width_strip = gf.partial(
     find_neff_vs_width,
-    wg_thickness=wg_thickness_silicon,
+    core_thickness=core_thickness_silicon,
     slab_thickness=0,
     filepath=PATH / "neff_vs_width_strip.csv",
 )
 find_neff_vs_width_rib90 = gf.partial(
     find_neff_vs_width,
-    wg_thickness=wg_thickness_silicon,
+    core_thickness=core_thickness_silicon,
     slab_thickness=90 * nm,
     filepath=PATH / "neff_vs_width_rib.csv",
 )
 
 find_neff_vs_width_nitride = gf.partial(
     find_neff_vs_width,
-    wg_thickness=wg_thickness_nitride,
+    core_thickness=core_thickness_nitride,
     slab_thickness=0.0,
-    ncore=2.0,
+    core_material=2.0,
     width1=200 * nm,
     width2=1500 * nm,
     filepath=PATH / "neff_vs_width_nitride.csv",
 )
 
 
 if __name__ == "__main__":
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/coupler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/mzi.py` & `gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/mzi.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     import gdsfactory.simulation.gtidy3d as gt
     import matplotlib.pyplot as plt
 
     nm = 1e-3
     strip = gt.modes.Waveguide(
         wavelength=1.55,
         wg_width=500 * nm,
-        wg_thickness=220 * nm,
+        core_thickness=220 * nm,
         slab_thickness=0.0,
-        ncore=gt.modes.si,
-        nclad=gt.modes.sio2,
+        core_material=gt.modes.si,
+        clad_material=gt.modes.sio2,
     )
 
     neff = 2.46  # Effective index of the waveguides
     wl0 = 1.55  # [μm] the wavelength at which neff and ng are defined
     wl = np.linspace(1.5, 1.6, 1000)  # [μm] Wavelengths to sweep over
     ngs = [4.182551, 4.169563, 4.172917]
     thicknesses = [210, 220, 230]
```

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/photonic_circuit_models/ring.py` & `gdsfactory-6.93.0/gdsfactory/simulation/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/plot.py` & `gdsfactory-6.93.0/gdsfactory/simulation/plot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/plot_csv.py` & `gdsfactory-6.93.0/gdsfactory/simulation/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/port_symmetries.py` & `gdsfactory-6.93.0/gdsfactory/simulation/port_symmetries.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/process/diffusion.py` & `gdsfactory-6.93.0/gdsfactory/simulation/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/process/implant_tables.py` & `gdsfactory-6.93.0/gdsfactory/simulation/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/process/pysrim.py` & `gdsfactory-6.93.0/gdsfactory/simulation/process/pysrim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/process/silicon.py` & `gdsfactory-6.93.0/gdsfactory/simulation/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/process/skew/antimony_si_skew.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/process/skew/arsenic_si_skew.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/process/skew/boron_si_skew.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv` & `gdsfactory-6.93.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/build_model.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/femwell_waveguide_model.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/femwell_waveguide_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/interpolators.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/meep_FDTD_model.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/meep_FDTD_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/meow_eme_model.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/meow_eme_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/mlp.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/models.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/parameter.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/plot_model.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/read.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/tests/test_mzi.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/tests/test_mzi_lattice.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sax/tests/test_parameters.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/add_gc.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/add_gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/circuit.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/__init__.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/bend_circular.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/bend_euler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler_fdtd.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler_ring.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/gc.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/mmi1x2.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/mmi2x2.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/mzi.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/mzi_siepic.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/mzi_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/ring_double.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/ring_double_siepic.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/ring_single.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/ring_single_siepic.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/components/straight.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/get_transmission.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/get_transmission.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/model_from_gdsfactory.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/model_from_sparameters.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/model_from_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/plot_circuit.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/plot_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/plot_model.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_circuit.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/simphony/tests/test_components.py` & `gdsfactory-6.93.0/gdsfactory/simulation/simphony/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sipann/bend_circular.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sipann/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sipann/bend_euler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sipann/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sipann/coupler.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sipann/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sipann/coupler_ring.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sipann/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/sipann/straight.py` & `gdsfactory-6.93.0/gdsfactory/simulation/sipann/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/simulation/thermal/heater.py` & `gdsfactory-6.93.0/gdsfactory/simulation/thermal/heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/snap.py` & `gdsfactory-6.93.0/gdsfactory/snap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/symbols.py` & `gdsfactory-6.93.0/gdsfactory/symbols.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/technology/__init__.py` & `gdsfactory-6.93.0/gdsfactory/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/technology/klayout_tech.py` & `gdsfactory-6.93.0/gdsfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/technology/layer_map.py` & `gdsfactory-6.93.0/gdsfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/technology/layer_stack.py` & `gdsfactory-6.93.0/gdsfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/technology/layer_views.py` & `gdsfactory-6.93.0/gdsfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/technology/simulation_settings.py` & `gdsfactory-6.93.0/gdsfactory/technology/simulation_settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/types.py` & `gdsfactory-6.93.0/gdsfactory/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/typings.py` & `gdsfactory-6.93.0/gdsfactory/typings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/utils/async_utils.py` & `gdsfactory-6.93.0/gdsfactory/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/utils/file_utils.py` & `gdsfactory-6.93.0/gdsfactory/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/utils/xml_utils.py` & `gdsfactory-6.93.0/gdsfactory/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/utils/yaml_utils.py` & `gdsfactory-6.93.0/gdsfactory/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/watch.py` & `gdsfactory-6.93.0/gdsfactory/watch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/widgets/layout_viewer.py` & `gdsfactory-6.93.0/gdsfactory/widgets/layout_viewer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/gdsfactory/write_cells.py` & `gdsfactory-6.93.0/gdsfactory/write_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.92.2/pyproject.toml` & `gdsfactory-6.93.0/pyproject.toml`

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
-version = "6.92.2"
+version = "6.93.0"
 authors = [
 {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 keywords = ["eda", "photonics", "python"]
 license = {file = "LICENSE"}
 dependencies = [
   "click",
@@ -90,15 +90,15 @@
       "mapbox_earcut",
       "meshio",
       "pygmsh",
       "pyvista",
       "trimesh",
       "shapely",
     ]
-    tidy3d = ["tidy3d==2.0.3"]
+    tidy3d = ["tidy3d==2.1.1"]
     devsim = [
       "devsim",
       "mkl",
       "pyvista",
       "tidy3d",
     ]
     meow = ["meow-sim"]
```

### Comparing `gdsfactory-6.92.2/PKG-INFO` & `gdsfactory-6.93.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsfactory
-Version: 6.92.2
+Version: 6.93.0
 Summary: python library to generate GDS layouts
 Keywords: eda,photonics,python
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -97,28 +97,28 @@
 Requires-Dist: shapely ; extra == "gmsh"
 Requires-Dist: meow-sim ; extra == "meow"
 Requires-Dist: ray[tune,air] ; extra == "ray"
 Requires-Dist: hyperopt ; extra == "ray"
 Requires-Dist: sax>=0.8.6 ; extra == "sax"
 Requires-Dist: jaxlib ; extra == "sax"
 Requires-Dist: jax ; extra == "sax"
-Requires-Dist: tidy3d==2.0.3 ; extra == "tidy3d"
+Requires-Dist: tidy3d==2.1.1 ; extra == "tidy3d"
 Provides-Extra: database
 Provides-Extra: dev
 Provides-Extra: devsim
 Provides-Extra: docs
 Provides-Extra: femwell
 Provides-Extra: full
 Provides-Extra: gmsh
 Provides-Extra: meow
 Provides-Extra: ray
 Provides-Extra: sax
 Provides-Extra: tidy3d
 
-# gdsfactory 6.92.2
+# gdsfactory 6.93.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
```

