# Comparing `tmp/straxen-2.0.6.tar.gz` & `tmp/straxen-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "straxen-2.0.6.tar", last modified: Wed Mar  8 16:09:33 2023, max compression
+gzip compressed data, was "straxen-2.0.7.tar", last modified: Tue Apr 25 03:21:47 2023, max compression
```

## Comparing `straxen-2.0.6.tar` & `straxen-2.0.7.tar`

### file list

```diff
@@ -1,236 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.149204 straxen-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    36488 2023-03-08 16:09:28.000000 straxen-2.0.6/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-08 16:09:28.000000 straxen-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-08 16:09:28.000000 straxen-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    48794 2023-03-08 16:09:33.149204 straxen-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-08 16:09:28.000000 straxen-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.133204 straxen-2.0.6/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-03-08 16:09:28.000000 straxen-2.0.6/bin/ajax
--rwxr-xr-x   0 runner    (1001) docker     (123)    66633 2023-03-08 16:09:28.000000 straxen-2.0.6/bin/bootstrax
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-03-08 16:09:28.000000 straxen-2.0.6/bin/fake_daq
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-03-08 16:09:28.000000 straxen-2.0.6/bin/microstrax
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-03-08 16:09:28.000000 straxen-2.0.6/bin/refresh_raw_records
--rw-r--r--   0 runner    (1001) docker     (123)    35964 2023-03-08 16:09:28.000000 straxen-2.0.6/bin/restrax
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-08 16:09:28.000000 straxen-2.0.6/bin/straxen-print_versions
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-03-08 16:09:28.000000 straxen-2.0.6/bin/straxer
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.133204 straxen-2.0.6/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-08 16:09:28.000000 straxen-2.0.6/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-08 16:09:28.000000 straxen-2.0.6/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-08 16:09:28.000000 straxen-2.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-08 16:09:33.149204 straxen-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-03-08 16:09:28.000000 straxen-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.133204 straxen-2.0.6/straxen/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.137204 straxen-2.0.6/straxen/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38954 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/bokeh_waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/daq_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/event_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/holoviews_waveform_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/posrec_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/pulse_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/quick_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/records_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/analyses/waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/bokeh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20732 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/corrections_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/daq_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/get_corrections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.137204 straxen-2.0.6/straxen/holoviews/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/holoviews/holoviews_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/holoviews/holoviews_peak_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/holoviews/holoviews_pmt_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/holoviews/holoviews_tpc_event_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/itp_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.137204 straxen-2.0.6/straxen/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/legacy/contexts_1t.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/legacy/hitfinder_thresholds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.137204 straxen-2.0.6/straxen/legacy/plugins_1t/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/legacy/plugins_1t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/legacy/plugins_1t/event_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/legacy/plugins_1t/pax_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/legacy/plugins_1t/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/legacy/plugins_1t/x1t_cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/legacy/xenon1t_url_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/matplotlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/mini_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/numbafied_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.137204 straxen-2.0.6/straxen/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.137204 straxen-2.0.6/straxen/plugins/afterpulses/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/afterpulses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/afterpulses/afterpulse_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.137204 straxen-2.0.6/straxen/plugins/aqmon_hits/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/aqmon_hits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/aqmon_hits/aqmon_hits.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.137204 straxen-2.0.6/straxen/plugins/detector_time_offsets/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/detector_time_offsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/detector_time_offsets/detector_time_offsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/_event_s2_position_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/corrected_areas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/distinct_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/energy_estimates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_ambience.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_area_per_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_info_double.py
--rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_pattern_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_s2_position_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_s2_position_gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_s2_position_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/event_w_bayes_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/local_minimum_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/multi_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/s2_recon_pos_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events/veto_proximity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/events_mv/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events_mv/events_mv.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events_mv/events_sync_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/events_nv/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events_nv/event_positions_nv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events_nv/events_nv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/events_nv/events_sync_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/hitlets_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/hitlets_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/hitlets_mv/hitlets_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/hitlets_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/hitlets_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/hitlets_nv/hitlets_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/individual_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/individual_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/led_cal/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/led_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/led_cal/led_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/merged_s2s/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/merged_s2s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/merged_s2s/merged_s2s.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/merged_s2s_he/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/merged_s2s_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/merged_s2s_he/merged_s2s_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/online_monitor_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/online_monitor_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/online_monitor_mv/online_monitor_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/online_monitor_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/online_monitor_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/online_monitor_nv/online_monitor_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/online_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/online_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/online_peak_monitor/online_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/peaklets/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaklets/peaklet_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaklets/peaklets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.141204 straxen-2.0.6/straxen/plugins/peaklets_he/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaklets_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaklets_he/peaklet_classification_he.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaklets_he/peaklets_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/plugins/peaks/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/_peak_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_ambience.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_classification_bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_proximity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peak_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peaks_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks/peaks_per_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/plugins/peaks_he/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks_he/peak_basics_he.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/peaks_he/peaks_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/plugins/raw_records/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/raw_records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/raw_records/daqreader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/plugins/raw_records_coin_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/raw_records_coin_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19659 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/plugins/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/records/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/plugins/records_he/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/records_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/records_he/records_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/plugins/records_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/records_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/records_mv/records_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/plugins/records_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/records_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/records_nv/records_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/plugins/veto_intervals/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/veto_intervals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/plugins/veto_intervals/veto_intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/scada.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.145204 straxen-2.0.6/straxen/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/storage/mongo_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/storage/online_monitor_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/storage/rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/storage/rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/storage/rundb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-03-08 16:09:28.000000 straxen-2.0.6/straxen/url_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.133204 straxen-2.0.6/straxen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48794 2023-03-08 16:09:32.000000 straxen-2.0.6/straxen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-08 16:09:33.000000 straxen-2.0.6/straxen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:09:32.000000 straxen-2.0.6/straxen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:09:32.000000 straxen-2.0.6/straxen.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-08 16:09:32.000000 straxen-2.0.6/straxen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-08 16:09:32.000000 straxen-2.0.6/straxen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.149204 straxen-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:33.149204 straxen-2.0.6/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/storage/test_database_frontends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/storage/test_mongo_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/storage/test_mongo_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/storage/test_rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/storage/test_rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_1T_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_aqmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_channel_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_cmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_count_pulses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_daq_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_itp_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_led_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_mini_analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_nveto_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_nveto_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_patternfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_peaklet_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_scada.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_testing_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_url_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-08 16:09:28.000000 straxen-2.0.6/tests/test_veto_hitlets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    37812 2023-04-25 03:21:42.000000 straxen-2.0.7/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-25 03:21:42.000000 straxen-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 03:21:42.000000 straxen-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50278 2023-04-25 03:21:47.662989 straxen-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-25 03:21:42.000000 straxen-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.646988 straxen-2.0.7/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/ajax
+-rwxr-xr-x   0 runner    (1001) docker     (123)    67099 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/bootstrax
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/fake_daq
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/microstrax
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/refresh_raw_records
+-rw-r--r--   0 runner    (1001) docker     (123)    35964 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/restrax
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/straxen-print_versions
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/straxer
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.646988 straxen-2.0.7/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-25 03:21:42.000000 straxen-2.0.7/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-25 03:21:42.000000 straxen-2.0.7/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-25 03:21:43.000000 straxen-2.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-25 03:21:47.666989 straxen-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-25 03:21:43.000000 straxen-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.646988 straxen-2.0.7/straxen/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38954 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/bokeh_waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/daq_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/event_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/holoviews_waveform_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/posrec_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/pulse_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/quick_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/records_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/bokeh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/corrections_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/daq_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/get_corrections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/holoviews_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/holoviews_peak_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/holoviews_pmt_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/holoviews_tpc_event_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/itp_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/contexts_1t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/hitfinder_thresholds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/legacy/plugins_1t/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/pax_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/x1t_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/xenon1t_url_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/matplotlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/mini_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/numbafied_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/plugins/afterpulses/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/afterpulses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/afterpulses/afterpulse_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/plugins/aqmon_hits/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/aqmon_hits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/aqmon_hits/aqmon_hits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/plugins/detector_time_offsets/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/detector_time_offsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/detector_time_offsets/detector_time_offsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/_event_s1_position_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/_event_s2_position_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/corrected_areas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/distinct_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/energy_estimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_area_per_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_info_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_pattern_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_s1_position_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_s2_position_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_s2_position_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_s2_position_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_w_bayes_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/local_minimum_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/multi_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/s2_recon_pos_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/veto_proximity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/events_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_mv/events_mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_mv/events_sync_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/events_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_nv/event_positions_nv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_nv/events_nv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_nv/events_sync_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/hitlets_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/hitlets_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/hitlets_mv/hitlets_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/hitlets_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/hitlets_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/hitlets_nv/hitlets_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/individual_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/individual_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/led_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/led_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/led_cal/led_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/merged_s2s/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/merged_s2s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/merged_s2s/merged_s2s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/merged_s2s_he/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/merged_s2s_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/merged_s2s_he/merged_s2s_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/online_monitor_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_monitor_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_monitor_mv/online_monitor_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/online_monitor_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_monitor_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_monitor_nv/online_monitor_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.658989 straxen-2.0.7/straxen/plugins/online_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_peak_monitor/online_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.658989 straxen-2.0.7/straxen/plugins/peaklets/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets/peaklet_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets/peaklets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/peaklets_he/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets_he/peaklet_classification_he.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets_he/peaklets_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/peaks/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/_peak_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/_peak_s1_position_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_classification_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_s1_position_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peaks_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peaks_per_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/peaks_he/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks_he/peak_basics_he.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks_he/peaks_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/raw_records/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/raw_records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/raw_records/daqreader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/raw_records_coin_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/raw_records_coin_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19659 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/records/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/records_he/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_he/records_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/records_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_mv/records_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/records_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_nv/records_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/veto_intervals/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/veto_intervals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/veto_intervals/veto_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/scada.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/online_monitor_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/url_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50278 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_database_frontends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_mongo_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_mongo_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_1T_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_aqmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_channel_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_cmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_count_pulses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_daq_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_itp_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_led_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_mini_analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_nveto_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_nveto_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_patternfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_peaklet_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_scada.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_testing_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_url_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_veto_hitlets.py
```

### Comparing `straxen-2.0.6/HISTORY.md` & `straxen-2.0.7/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+v2.0.7 / 2023-04-25
+-------------------
+## What's Changed
+* Bootstrax target removal after failures by @cfuselli in https://github.com/XENONnT/straxen/pull/1145
+* reforming _raw_path and _processed_path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1149
+* Adding correction of Z position due to non-uniform drift velocity by @terliuk in https://github.com/XENONnT/straxen/pull/1148
+* Bump the versions of peaklets and quality check runs-on by @dachengx in https://github.com/XENONnT/straxen/pull/1153
+* S1-Based 3D Position Reconstruction by @matteoguida in https://github.com/XENONnT/straxen/pull/1146
+* Bump xedocs from 0.2.14 to 0.2.16 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1158
+* Use zstd as compressor of peaks by @dachengx in https://github.com/XENONnT/straxen/pull/1154
+* Bump sphinx from 5.3.0 to 6.2.0 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1161
+
+## New Contributors
+* @cfuselli made their first contribution in https://github.com/XENONnT/straxen/pull/1145
+* @matteoguida made their first contribution in https://github.com/XENONnT/straxen/pull/1146
+* @hmdyt made their first contribution in https://github.com/XENONnT/straxen/pull/1159
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.6...v2.0.7
+
+
 v2.0.6 / 2023-03-08
 -------------------
 ## What's Changed
 * Bump supercharge/mongodb-github-action from 1.8.0 to 1.9.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1140
 * Small patches to restrax module by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1143, d04a3428c52c159577b61af2a28ddd0af5652027, 602b807291211f083c8f54df6768b8198fbf6b55
 * Ms events by @michaweiss89 and @HenningSE in https://github.com/XENONnT/straxen/pull/1080
```

### Comparing `straxen-2.0.6/LICENSE` & `straxen-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/PKG-INFO` & `straxen-2.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.0.6
+Version: 2.0.7
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Description: # straxen
         Streaming analysis for XENON(nT)
         
@@ -25,14 +25,34 @@
         [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
         [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
         
         [![Update context collection](https://github.com/XENONnT/straxen/workflows/Update%20context%20collection/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/contexts.yml)
         [![Python style](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml)
         
         
+        v2.0.7 / 2023-04-25
+        -------------------
+        ## What's Changed
+        * Bootstrax target removal after failures by @cfuselli in https://github.com/XENONnT/straxen/pull/1145
+        * reforming _raw_path and _processed_path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1149
+        * Adding correction of Z position due to non-uniform drift velocity by @terliuk in https://github.com/XENONnT/straxen/pull/1148
+        * Bump the versions of peaklets and quality check runs-on by @dachengx in https://github.com/XENONnT/straxen/pull/1153
+        * S1-Based 3D Position Reconstruction by @matteoguida in https://github.com/XENONnT/straxen/pull/1146
+        * Bump xedocs from 0.2.14 to 0.2.16 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1158
+        * Use zstd as compressor of peaks by @dachengx in https://github.com/XENONnT/straxen/pull/1154
+        * Bump sphinx from 5.3.0 to 6.2.0 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1161
+        
+        ## New Contributors
+        * @cfuselli made their first contribution in https://github.com/XENONnT/straxen/pull/1145
+        * @matteoguida made their first contribution in https://github.com/XENONnT/straxen/pull/1146
+        * @hmdyt made their first contribution in https://github.com/XENONnT/straxen/pull/1159
+        
+        **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.6...v2.0.7
+        
+        
         v2.0.6 / 2023-03-08
         -------------------
         ## What's Changed
         * Bump supercharge/mongodb-github-action from 1.8.0 to 1.9.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1140
         * Small patches to restrax module by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1143, d04a3428c52c159577b61af2a28ddd0af5652027, 602b807291211f083c8f54df6768b8198fbf6b55
         * Ms events by @michaweiss89 and @HenningSE in https://github.com/XENONnT/straxen/pull/1080
```

### Comparing `straxen-2.0.6/README.md` & `straxen-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/bin/ajax` & `straxen-2.0.7/bin/ajax`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/bin/bootstrax` & `straxen-2.0.7/bin/bootstrax`

 * *Files 2% similar despite different names*

```diff
@@ -210,25 +210,41 @@
 # an eventbuilder should not process new data.
 max_queue_new_runs = 3
 
 # Remove any targets or post processing targets after the run failed
 # this many times. If high level data is hitting some edge case, we
 # might want to be able to keep the intermediate level data.
 # NB: fnmatch so event* applies e.g. to event_basics, peak* to e.g. peaklets
+# See https://xe1t-wiki.lngs.infn.it/doku.php?id=cfuselli:bootstrax_fail_targets
 remove_target_after_fails = {
-    'event*': 2,
-    'hitlets*': 2,
+    'event*':            2,
+    'corrected_areas':   2,
+    'energy_estimates':  2,
+    'distinct_channels': 2,
+    
+    '*pos*':             3,
+    'individual_peak*':  3,
     'online_monitor_*v': 3,
-    'online_peak': 5,
-    'peaks*': 4,
-    'peak_basics': 5,
-    'peaklets': 6,
-    'veto_*': 4,
-    '*': 7,
-}
+    
+    'peak_*':            4,
+    'online_peak*':      4,
+    '*hit*':             4,
+    'veto_*':            4,
+    '*pulse*':           4,
+    'led_*':             4,
+    'ext_timings_nv':    4,
+    
+    'merged_s2s*':       5,
+    
+    'peak*':             6,
+    'lone_*':            6,
+    'detector_time_*':   6,
+    
+    '*':                 7,
+} 
 
 ##
 # Initialize globals (e.g. rundb connection)
 ##
 hostname = socket.getfqdn()
 
 versions = straxen.print_versions(
```

### Comparing `straxen-2.0.6/bin/fake_daq` & `straxen-2.0.7/bin/fake_daq`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/bin/microstrax` & `straxen-2.0.7/bin/microstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/bin/refresh_raw_records` & `straxen-2.0.7/bin/refresh_raw_records`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/bin/restrax` & `straxen-2.0.7/bin/restrax`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/bin/straxen-print_versions` & `straxen-2.0.7/bin/straxen-print_versions`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/bin/straxer` & `straxen-2.0.7/bin/straxer`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/setup.cfg` & `straxen-2.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/setup.py` & `straxen-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md') as file:
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(name='straxen',
-                 version='2.0.6',
+                 version='2.0.7',
                  description='Streaming analysis for XENON',
                  author='Straxen contributors, the XENON collaboration',
                  url='https://github.com/XENONnT/straxen',
                  long_description=readme + '\n\n' + history,
                  long_description_content_type="text/markdown",
                  setup_requires=['pytest-runner'],
                  install_requires=requires,
```

### Comparing `straxen-2.0.6/straxen/__init__.py` & `straxen-2.0.7/straxen/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 from utilix import uconfig
 from .common import *
 # contexts.py below
 from .corrections_services import *
 from .get_corrections import *
```

### Comparing `straxen-2.0.6/straxen/analyses/bokeh_waveform_plot.py` & `straxen-2.0.7/straxen/analyses/bokeh_waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/analyses/daq_waveforms.py` & `straxen-2.0.7/straxen/analyses/daq_waveforms.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/analyses/event_display.py` & `straxen-2.0.7/straxen/analyses/event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/analyses/holoviews_waveform_display.py` & `straxen-2.0.7/straxen/analyses/holoviews_waveform_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/analyses/posrec_comparison.py` & `straxen-2.0.7/straxen/analyses/posrec_comparison.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/analyses/pulse_plots.py` & `straxen-2.0.7/straxen/analyses/pulse_plots.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/analyses/quick_checks.py` & `straxen-2.0.7/straxen/analyses/quick_checks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/analyses/records_matrix.py` & `straxen-2.0.7/straxen/analyses/records_matrix.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/analyses/waveform_plot.py` & `straxen-2.0.7/straxen/analyses/waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/bokeh_utils.py` & `straxen-2.0.7/straxen/bokeh_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/common.py` & `straxen-2.0.7/straxen/common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/contexts.py` & `straxen-2.0.7/straxen/contexts.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,19 @@
             'cmt://'
             'format://fdc_map_{alg}'
             '?alg=plugin.default_reconstruction_algorithm'
             '&version=ONLINE'
             '&run_id=plugin.run_id'
             '&fmt=binary'
             '&scale_coordinates=plugin.coordinate_scales',
+    z_bias_map='itp_map://'
+               'resource://'
+               'XnT_z_bias_map_chargeup_20230329.json.gz?'
+               'fmt=json.gz'
+               '&method=RegularGridInterpolator',
 )
 # these are placeholders to avoid calling cmt with non integer run_ids. Better solution pending.
 # s1,s2 and fd corrections are still problematic
 xnt_simulation_config = deepcopy(xnt_common_config)
 xnt_simulation_config.update(gain_model="legacy-to-pe://to_pe_placeholder",
                              gain_model_nv="legacy-to-pe://adc_nv",
                              gain_model_mv="legacy-to-pe://adc_mv",
@@ -118,16 +123,18 @@
                    include_online_monitor: bool = False,
                    include_rucio_local: bool = False,
 
                    # Frontend options
                    download_heavy: bool = False,
                    _rucio_path: str = '/dali/lgrandi/rucio/',
                    _rucio_local_path: ty.Optional[str] = None,
-                   _raw_path: ty.Optional[str] = '/dali/lgrandi/xenonnt/raw',
-                   _processed_path: ty.Optional[str] = '/dali/lgrandi/xenonnt/processed',
+                   _raw_paths: ty.Optional[str] = ['/dali/lgrandi/xenonnt/raw'],
+                   _processed_paths: ty.Optional[ty.List[str]] = ['/dali/lgrandi/xenonnt/processed',
+                                                                  '/project2/lgrandi/xenonnt/processed',
+                                                                  '/project/lgrandi/xenonnt/processed'],
 
                    # Testing options
                    _context_config_overwrite: ty.Optional[dict] = None,
                    _database_init: bool = True,
                    _forbid_creation_of: ty.Optional[dict] = None,
                    **kwargs):
     """
@@ -148,16 +155,16 @@
         data the runs database is out of sync with rucio
     :param download_heavy: bool, whether or not to allow downloads of
         heavy data (raw_records*, less the aqmon)
 
     :param _rucio_path: str, path of rucio
     :param _rucio_local_path: str, path of local RSE of rucio. Only use
         for testing!
-    :param _raw_path: str, common path of the raw-data
-    :param _processed_path: str. common path of output data
+    :param _raw_paths: list[str], common path of the raw-data
+    :param _processed_paths: list[str]. common paths of output data
     :param _context_config_overwrite: dict, overwrite config
     :param _database_init: bool, start the database (for testing)
     :param _forbid_creation_of: str/tuple, of datatypes to prevent form
         being written (raw_records* is always forbidden).
     :param kwargs: dict, context options
     :return: strax.Context
     """
@@ -178,23 +185,25 @@
             minimum_run_number=minimum_run_number,
             maximum_run_number=maximum_run_number,
             runid_field='number',
             new_data_path=output_folder,
             rucio_path=_rucio_path,
         )] if _database_init else []
     if not we_are_the_daq:
-        st.storage += [
-            strax.DataDirectory(
-                _raw_path,
-                readonly=True,
-                take_only=straxen.DAQReader.provides),
-            strax.DataDirectory(
+        for _raw_path in _raw_paths:
+            st.storage += [
+                strax.DataDirectory(
+                    _raw_path,
+                    readonly=True,
+                    take_only=straxen.DAQReader.provides)]
+        for _processed_path in _processed_paths:
+            st.storage += [strax.DataDirectory(
                 _processed_path,
-                readonly=True,
-            )]
+                readonly=True)]
+            
         if output_folder:
             st.storage += [strax.DataDirectory(output_folder,
                                                provide_run_metadata=True,
                                                )]
         st.context_config['forbid_creation_of'] = straxen.daqreader.DAQReader.provides
         if _forbid_creation_of is not None:
             st.context_config['forbid_creation_of'] += strax.to_str_tuple(_forbid_creation_of)
```

### Comparing `straxen-2.0.6/straxen/corrections_services.py` & `straxen-2.0.7/straxen/corrections_services.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/daq_core.py` & `straxen-2.0.7/straxen/daq_core.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/entry_points.py` & `straxen-2.0.7/straxen/entry_points.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/get_corrections.py` & `straxen-2.0.7/straxen/get_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/holoviews/holoviews_inspector.py` & `straxen-2.0.7/straxen/holoviews/holoviews_inspector.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/holoviews/holoviews_peak_data.py` & `straxen-2.0.7/straxen/holoviews/holoviews_peak_data.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/holoviews/holoviews_pmt_array.py` & `straxen-2.0.7/straxen/holoviews/holoviews_pmt_array.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/holoviews/holoviews_tpc_event_display.py` & `straxen-2.0.7/straxen/holoviews/holoviews_tpc_event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/holoviews_utils.py` & `straxen-2.0.7/straxen/holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/itp_map.py` & `straxen-2.0.7/straxen/itp_map.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/legacy/contexts_1t.py` & `straxen-2.0.7/straxen/legacy/contexts_1t.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/legacy/hitfinder_thresholds.py` & `straxen-2.0.7/straxen/legacy/hitfinder_thresholds.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/legacy/plugins_1t/event_info.py` & `straxen-2.0.7/straxen/legacy/plugins_1t/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/legacy/plugins_1t/pax_interface.py` & `straxen-2.0.7/straxen/legacy/plugins_1t/pax_interface.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/legacy/plugins_1t/peak_positions.py` & `straxen-2.0.7/straxen/legacy/plugins_1t/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/legacy/plugins_1t/x1t_cuts.py` & `straxen-2.0.7/straxen/legacy/plugins_1t/x1t_cuts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/legacy/xenon1t_url_configs.py` & `straxen-2.0.7/straxen/legacy/xenon1t_url_configs.py`

 * *Files 15% similar despite different names*

```diff
@@ -82,7 +82,16 @@
     else:
         raise ValueError(f'No legacy fdc for run {run_id}')
 
     if url is None:
         raise ValueError(f'No legacy fdc for run {run_id}')
 
     return InterpolatingMap(get_resource(url, fmt='binary'))
+
+
+@URLConfig.register('legacy-z_bias')
+def get_z_bias(offset: str):
+    """Return a lambda function return offset as placeholder"""
+    def fake_z_bias(rz, **kwargs):
+        return np.zeros(len(rz)) * int(offset)
+
+    return fake_z_bias
```

### Comparing `straxen-2.0.6/straxen/matplotlib_utils.py` & `straxen-2.0.7/straxen/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/mini_analysis.py` & `straxen-2.0.7/straxen/mini_analysis.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/misc.py` & `straxen-2.0.7/straxen/misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/numbafied_scipy.py` & `straxen-2.0.7/straxen/numbafied_scipy.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/__init__.py` & `straxen-2.0.7/straxen/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/afterpulses/afterpulse_processing.py` & `straxen-2.0.7/straxen/plugins/afterpulses/afterpulse_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/aqmon_hits/aqmon_hits.py` & `straxen-2.0.7/straxen/plugins/aqmon_hits/aqmon_hits.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/defaults.py` & `straxen-2.0.7/straxen/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/detector_time_offsets/detector_time_offsets.py` & `straxen-2.0.7/straxen/plugins/detector_time_offsets/detector_time_offsets.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/__init__.py` & `straxen-2.0.7/straxen/plugins/events/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,12 +51,15 @@
 
 from . import event_s2_position_cnn
 from .event_s2_position_cnn import *
 
 from . import event_s2_position_gcn
 from .event_s2_position_gcn import *
 
+from . import event_s1_position_cnn
+from .event_s1_position_cnn import *
+
 from . import local_minimum_info
 from .local_minimum_info import *
 
 from . import multi_scatter
 from .multi_scatter import *
```

### Comparing `straxen-2.0.6/straxen/plugins/events/_event_s2_position_base.py` & `straxen-2.0.7/straxen/plugins/events/_event_s2_position_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/corrected_areas.py` & `straxen-2.0.7/straxen/plugins/events/corrected_areas.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/distinct_channels.py` & `straxen-2.0.7/straxen/plugins/events/distinct_channels.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/energy_estimates.py` & `straxen-2.0.7/straxen/plugins/events/energy_estimates.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_ambience.py` & `straxen-2.0.7/straxen/plugins/events/event_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_area_per_channel.py` & `straxen-2.0.7/straxen/plugins/events/event_area_per_channel.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_basics.py` & `straxen-2.0.7/straxen/plugins/events/event_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_info.py` & `straxen-2.0.7/straxen/plugins/events/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_info_double.py` & `straxen-2.0.7/straxen/plugins/events/event_info_double.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_pattern_fit.py` & `straxen-2.0.7/straxen/plugins/events/event_pattern_fit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_positions.py` & `straxen-2.0.7/straxen/plugins/events/event_positions.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     positions of the default_reconstruction_algorithm. In case the fdc_map
     is given as a file (not through CMT), then the coordinate system
     should be given as (x, y, z), not (x, y, drift_time).
     """
 
     depends_on = ('event_basics',)
 
-    __version__ = '0.1.5'
+    __version__ = '0.2.0'
 
     default_reconstruction_algorithm = straxen.URLConfig(
         default=DEFAULT_POSREC_ALGO,
         help="default reconstruction algorithm that provides (x,y)"
     )
 
     electron_drift_velocity = straxen.URLConfig(
@@ -42,31 +42,43 @@
         cache=True)
 
     fdc_map = straxen.URLConfig(
         infer_type=False,
         help='3D field distortion correction map path',
         default='legacy-fdc://xenon1t_sr0_sr1?run_id=plugin.run_id')
 
+    z_bias_map = straxen.URLConfig(
+        infer_type=False,
+        help='Map of Z bias due to non uniform drift velocity/field',
+        default='legacy-z_bias://0')
+
     def infer_dtype(self):
         dtype = []
         for j in 'x y r'.split():
             comment = f'Main interaction {j}-position, field-distortion corrected (cm)'
             dtype += [(j, np.float32, comment)]
             for s_i in [1, 2]:
                 comment = f'Alternative S{s_i} interaction (rel. main S{int(2 * (1.5 - s_i) + s_i)}) {j}-position, field-distortion corrected (cm)'
                 field = f'alt_s{s_i}_{j}_fdc'
                 dtype += [(field, np.float32, comment)]
 
         for j in ['z']:
             comment = 'Interaction z-position, using mean drift velocity only (cm)'
             dtype += [(j, np.float32, comment)]
+            comment = 'Interaction z-position corrected to non-uniform drift velocity [ cm ]'
+            dtype += [(j + "_dv_corr", np.float32, comment)]
             for s_i in [1, 2]:
                 comment = f'Alternative S{s_i} z-position (rel. main S{int(2 * (1.5 - s_i) + s_i)}), using mean drift velocity only (cm)'
                 field = f'alt_s{s_i}_z'
                 dtype += [(field, np.float32, comment)]
+                # values for corrected Z position
+                comment = f'Alternative S{s_i} z-position (rel. main S{[1 if s_i==2 else 2]}), corrected for non-uniform field (cm)'
+                field = f'alt_s{s_i}_z_dv_corr'
+                dtype += [(field, np.float32, comment)]
+
 
         naive_pos = []
         fdc_pos = []
         for j in 'r z'.split():
             naive_pos += [(f'{j}_naive',
                            np.float32,
                            f'Main interaction {j}-position with observed position (cm)')]
@@ -125,24 +137,26 @@
             with np.errstate(invalid='ignore'):
                 z_cor = -(z_obs ** 2 - delta_r ** 2) ** 0.5
                 invalid = np.abs(z_obs) < np.abs(delta_r)
                 # do not apply z correction above gate
                 invalid |= z_obs >= 0
             z_cor[invalid] = z_obs[invalid]
             delta_z = z_cor - z_obs
+            # correction of z bias due to non-uniform field
+            z_dv_delta = self.z_bias_map(np.array([r_obs, z_obs]).T, map_name='z_bias_map')
 
             pre_field = '' if s_i == 0 else f'alt_s{s_i}_'
             post_field = '' if s_i == 0 else '_fdc'
             result.update({f'{pre_field}x{post_field}': orig_pos[:, 0] * scale,
                            f'{pre_field}y{post_field}': orig_pos[:, 1] * scale,
                            f'{pre_field}r{post_field}': r_cor,
                            f'{pre_field}r_naive': r_obs,
                            f'{pre_field}r_field_distortion_correction': delta_r,
                            f'{pre_field}theta': np.arctan2(orig_pos[:, 1], orig_pos[:, 0]),
                            f'{pre_field}z_naive': z_obs,
                            # using z_obs in agreement with the dtype description
                            # the FDC for z (z_cor) is found to be not reliable (see #527)
                            f'{pre_field}z': z_obs,
-                           f'{pre_field}z_field_distortion_correction': delta_z
+                           f'{pre_field}z_field_distortion_correction': delta_z,
+                           f'{pre_field}z_dv_corr': z_obs - z_dv_delta,
                            })
-
         return result
```

### Comparing `straxen-2.0.6/straxen/plugins/events/event_s2_position_cnn.py` & `straxen-2.0.7/straxen/plugins/events/event_s2_position_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_s2_position_gcn.py` & `straxen-2.0.7/straxen/plugins/events/event_s2_position_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_s2_position_mlp.py` & `straxen-2.0.7/straxen/plugins/events/event_s2_position_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_shadow.py` & `straxen-2.0.7/straxen/plugins/events/event_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_top_bottom_params.py` & `straxen-2.0.7/straxen/plugins/events/event_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/event_w_bayes_class.py` & `straxen-2.0.7/straxen/plugins/events/event_w_bayes_class.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/events.py` & `straxen-2.0.7/straxen/plugins/events/events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/local_minimum_info.py` & `straxen-2.0.7/straxen/plugins/events/local_minimum_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/multi_scatter.py` & `straxen-2.0.7/straxen/plugins/events/multi_scatter.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/s2_recon_pos_diff.py` & `straxen-2.0.7/straxen/plugins/events/s2_recon_pos_diff.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events/veto_proximity.py` & `straxen-2.0.7/straxen/plugins/events/veto_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events_mv/events_mv.py` & `straxen-2.0.7/straxen/plugins/events_mv/events_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events_mv/events_sync_mv.py` & `straxen-2.0.7/straxen/plugins/events_mv/events_sync_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events_nv/event_positions_nv.py` & `straxen-2.0.7/straxen/plugins/events_nv/event_positions_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events_nv/events_nv.py` & `straxen-2.0.7/straxen/plugins/events_nv/events_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/events_nv/events_sync_nv.py` & `straxen-2.0.7/straxen/plugins/events_nv/events_sync_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/hitlets_mv/hitlets_mv.py` & `straxen-2.0.7/straxen/plugins/hitlets_mv/hitlets_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/hitlets_nv/hitlets_nv.py` & `straxen-2.0.7/straxen/plugins/hitlets_nv/hitlets_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py` & `straxen-2.0.7/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/led_cal/led_calibration.py` & `straxen-2.0.7/straxen/plugins/led_cal/led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/merged_s2s/merged_s2s.py` & `straxen-2.0.7/straxen/plugins/merged_s2s/merged_s2s.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/merged_s2s_he/merged_s2s_he.py` & `straxen-2.0.7/straxen/plugins/merged_s2s_he/merged_s2s_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/online_monitor_mv/online_monitor_mv.py` & `straxen-2.0.7/straxen/plugins/online_monitor_mv/online_monitor_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/online_monitor_nv/online_monitor_nv.py` & `straxen-2.0.7/straxen/plugins/online_monitor_nv/online_monitor_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/online_peak_monitor/online_peak_monitor.py` & `straxen-2.0.7/straxen/plugins/online_peak_monitor/online_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaklets/peaklet_classification.py` & `straxen-2.0.7/straxen/plugins/peaklets/peaklet_classification.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaklets/peaklets.py` & `straxen-2.0.7/straxen/plugins/peaklets/peaklets.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     depends_on = ('records',)
     provides = ('peaklets', 'lone_hits')
     data_kind = dict(peaklets='peaklets',
                      lone_hits='lone_hits')
     parallel = 'process'
     compressor = 'zstd'
 
-    __version__ = '1.0.0'
+    __version__ = '1.0.1'
 
     peaklet_gap_threshold = straxen.URLConfig(
         default=700, infer_type=False,
         help="No hits for this many ns triggers a new peak")
 
     peak_left_extension = straxen.URLConfig(
         default=30, infer_type=False,
```

### Comparing `straxen-2.0.6/straxen/plugins/peaklets_he/peaklet_classification_he.py` & `straxen-2.0.7/straxen/plugins/peaklets_he/peaklet_classification_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaklets_he/peaklets_he.py` & `straxen-2.0.7/straxen/plugins/peaklets_he/peaklets_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/__init__.py` & `straxen-2.0.7/straxen/plugins/peaks/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 from . import peak_basics
 from .peak_basics import *
 
 from . import peak_classification_bayes
 from .peak_classification_bayes import *
 
+from . import peak_s1_position_cnn
+from .peak_s1_position_cnn import *
+
 from . import peak_positions
 from .peak_positions import *
 
 from . import peak_positions_cnn
 from .peak_positions_cnn import *
 
 from . import peak_positions_gcn
```

### Comparing `straxen-2.0.6/straxen/plugins/peaks/_peak_positions_base.py` & `straxen-2.0.7/straxen/plugins/peaks/_peak_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_ambience.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_basics.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_classification_bayes.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_classification_bayes.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_positions.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_positions_cnn.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_positions_gcn.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_positions_mlp.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_positions_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_proximity.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_shadow.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peak_top_bottom_params.py` & `straxen-2.0.7/straxen/plugins/peaks/peak_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peaks.py` & `straxen-2.0.7/straxen/plugins/peaks/peaks.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     """
     __version__ = '0.1.2'
 
     depends_on = ('peaklets', 'peaklet_classification', 'merged_s2s')
     data_kind = 'peaks'
     provides = 'peaks'
     parallel = True
+    compressor = 'zstd'
     save_when = strax.SaveWhen.EXPLICIT
 
     diagnose_sorting = straxen.URLConfig(
         track=False, default=False, infer_type=False,
         help="Enable runtime checks for sorting and disjointness")
 
     merge_without_s1 = straxen.URLConfig(
```

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peaks_corrections.py` & `straxen-2.0.7/straxen/plugins/peaks/peaks_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks/peaks_per_event.py` & `straxen-2.0.7/straxen/plugins/peaks/peaks_per_event.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/peaks_he/peaks_he.py` & `straxen-2.0.7/straxen/plugins/peaks_he/peaks_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/raw_records/daqreader.py` & `straxen-2.0.7/straxen/plugins/raw_records/daqreader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/raw_records_coin_nv/nveto_recorder.py` & `straxen-2.0.7/straxen/plugins/raw_records_coin_nv/nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/records/records.py` & `straxen-2.0.7/straxen/plugins/records/records.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/records_he/records_he.py` & `straxen-2.0.7/straxen/plugins/records_he/records_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/records_mv/records_mv.py` & `straxen-2.0.7/straxen/plugins/records_mv/records_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/records_nv/records_nv.py` & `straxen-2.0.7/straxen/plugins/records_nv/records_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/plugins/veto_intervals/veto_intervals.py` & `straxen-2.0.7/straxen/plugins/veto_intervals/veto_intervals.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/scada.py` & `straxen-2.0.7/straxen/scada.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 @export
 class SCADAInterface:
 
     def __init__(self, context=None, use_progress_bar=True):
         """
-        Interface to excess the XENONnT slow control data via python.
+        Interface to access the XENONnT slow control data via python.
 
         :param context: Context you are using e.g. st. This is needed
             if you would like to query data via run_ids.
         :param use_progress_bar: Use a progress bar in the Scada interface
         """
         self.we_are_straxen = False
         self._token_expire_time = None
```

### Comparing `straxen-2.0.6/straxen/storage/mongo_storage.py` & `straxen-2.0.7/straxen/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/storage/online_monitor_frontend.py` & `straxen-2.0.7/straxen/storage/online_monitor_frontend.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/storage/rucio_local.py` & `straxen-2.0.7/straxen/storage/rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/storage/rucio_remote.py` & `straxen-2.0.7/straxen/storage/rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/storage/rundb.py` & `straxen-2.0.7/straxen/storage/rundb.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/test_utils.py` & `straxen-2.0.7/straxen/test_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/units.py` & `straxen-2.0.7/straxen/units.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen/url_config.py` & `straxen-2.0.7/straxen/url_config.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/straxen.egg-info/PKG-INFO` & `straxen-2.0.7/straxen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.0.6
+Version: 2.0.7
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Description: # straxen
         Streaming analysis for XENON(nT)
         
@@ -25,14 +25,34 @@
         [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
         [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
         
         [![Update context collection](https://github.com/XENONnT/straxen/workflows/Update%20context%20collection/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/contexts.yml)
         [![Python style](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml)
         
         
+        v2.0.7 / 2023-04-25
+        -------------------
+        ## What's Changed
+        * Bootstrax target removal after failures by @cfuselli in https://github.com/XENONnT/straxen/pull/1145
+        * reforming _raw_path and _processed_path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1149
+        * Adding correction of Z position due to non-uniform drift velocity by @terliuk in https://github.com/XENONnT/straxen/pull/1148
+        * Bump the versions of peaklets and quality check runs-on by @dachengx in https://github.com/XENONnT/straxen/pull/1153
+        * S1-Based 3D Position Reconstruction by @matteoguida in https://github.com/XENONnT/straxen/pull/1146
+        * Bump xedocs from 0.2.14 to 0.2.16 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1158
+        * Use zstd as compressor of peaks by @dachengx in https://github.com/XENONnT/straxen/pull/1154
+        * Bump sphinx from 5.3.0 to 6.2.0 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1161
+        
+        ## New Contributors
+        * @cfuselli made their first contribution in https://github.com/XENONnT/straxen/pull/1145
+        * @matteoguida made their first contribution in https://github.com/XENONnT/straxen/pull/1146
+        * @hmdyt made their first contribution in https://github.com/XENONnT/straxen/pull/1159
+        
+        **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.6...v2.0.7
+        
+        
         v2.0.6 / 2023-03-08
         -------------------
         ## What's Changed
         * Bump supercharge/mongodb-github-action from 1.8.0 to 1.9.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1140
         * Small patches to restrax module by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1143, d04a3428c52c159577b61af2a28ddd0af5652027, 602b807291211f083c8f54df6768b8198fbf6b55
         * Ms events by @michaweiss89 and @HenningSE in https://github.com/XENONnT/straxen/pull/1080
```

### Comparing `straxen-2.0.6/straxen.egg-info/SOURCES.txt` & `straxen-2.0.7/straxen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,25 +68,27 @@
 straxen/plugins/afterpulses/__init__.py
 straxen/plugins/afterpulses/afterpulse_processing.py
 straxen/plugins/aqmon_hits/__init__.py
 straxen/plugins/aqmon_hits/aqmon_hits.py
 straxen/plugins/detector_time_offsets/__init__.py
 straxen/plugins/detector_time_offsets/detector_time_offsets.py
 straxen/plugins/events/__init__.py
+straxen/plugins/events/_event_s1_position_base.py
 straxen/plugins/events/_event_s2_position_base.py
 straxen/plugins/events/corrected_areas.py
 straxen/plugins/events/distinct_channels.py
 straxen/plugins/events/energy_estimates.py
 straxen/plugins/events/event_ambience.py
 straxen/plugins/events/event_area_per_channel.py
 straxen/plugins/events/event_basics.py
 straxen/plugins/events/event_info.py
 straxen/plugins/events/event_info_double.py
 straxen/plugins/events/event_pattern_fit.py
 straxen/plugins/events/event_positions.py
+straxen/plugins/events/event_s1_position_cnn.py
 straxen/plugins/events/event_s2_position_cnn.py
 straxen/plugins/events/event_s2_position_gcn.py
 straxen/plugins/events/event_s2_position_mlp.py
 straxen/plugins/events/event_shadow.py
 straxen/plugins/events/event_top_bottom_params.py
 straxen/plugins/events/event_w_bayes_class.py
 straxen/plugins/events/events.py
@@ -123,22 +125,24 @@
 straxen/plugins/peaklets/peaklet_classification.py
 straxen/plugins/peaklets/peaklets.py
 straxen/plugins/peaklets_he/__init__.py
 straxen/plugins/peaklets_he/peaklet_classification_he.py
 straxen/plugins/peaklets_he/peaklets_he.py
 straxen/plugins/peaks/__init__.py
 straxen/plugins/peaks/_peak_positions_base.py
+straxen/plugins/peaks/_peak_s1_position_base.py
 straxen/plugins/peaks/peak_ambience.py
 straxen/plugins/peaks/peak_basics.py
 straxen/plugins/peaks/peak_classification_bayes.py
 straxen/plugins/peaks/peak_positions.py
 straxen/plugins/peaks/peak_positions_cnn.py
 straxen/plugins/peaks/peak_positions_gcn.py
 straxen/plugins/peaks/peak_positions_mlp.py
 straxen/plugins/peaks/peak_proximity.py
+straxen/plugins/peaks/peak_s1_position_cnn.py
 straxen/plugins/peaks/peak_shadow.py
 straxen/plugins/peaks/peak_top_bottom_params.py
 straxen/plugins/peaks/peaks.py
 straxen/plugins/peaks/peaks_corrections.py
 straxen/plugins/peaks/peaks_per_event.py
 straxen/plugins/peaks_he/__init__.py
 straxen/plugins/peaks_he/peak_basics_he.py
```

### Comparing `straxen-2.0.6/tests/storage/test_database_frontends.py` & `straxen-2.0.7/tests/storage/test_database_frontends.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/storage/test_mongo_downloader.py` & `straxen-2.0.7/tests/storage/test_mongo_downloader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/storage/test_mongo_interactions.py` & `straxen-2.0.7/tests/storage/test_mongo_interactions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/storage/test_rucio_local.py` & `straxen-2.0.7/tests/storage/test_rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/storage/test_rucio_remote.py` & `straxen-2.0.7/tests/storage/test_rucio_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     def get_context(self, download_heavy: bool) -> strax.Context:
         os.makedirs(self.staging_dir, exist_ok=True)
         context = straxen.contexts.xenonnt_online(
             output_folder=os.path.join(self.staging_dir, 'output'),
             include_rucio_remote=True,
             download_heavy=download_heavy,
             _rucio_path=self.staging_dir,
-            _raw_path=os.path.join(self.staging_dir, 'raw'),
+            _raw_paths=[os.path.join(self.staging_dir, 'raw')],
             _database_init=False,
-            _processed_path=os.path.join(self.staging_dir, 'processed'),
+            _processed_paths=[os.path.join(self.staging_dir, 'processed')],
         )
         return context
 
     def tearDown(self):
         if os.path.exists(self.staging_dir):
             shutil.rmtree(self.staging_dir)
```

### Comparing `straxen-2.0.6/tests/test_1T_plugins.py` & `straxen-2.0.7/tests/test_1T_plugins.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_aqmon.py` & `straxen-2.0.7/tests/test_aqmon.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_basics.py` & `straxen-2.0.7/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_channel_split.py` & `straxen-2.0.7/tests/test_channel_split.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_cmt.py` & `straxen-2.0.7/tests/test_cmt.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_common.py` & `straxen-2.0.7/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_contexts.py` & `straxen-2.0.7/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_count_pulses.py` & `straxen-2.0.7/tests/test_count_pulses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_daq_reader.py` & `straxen-2.0.7/tests/test_daq_reader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_holoviews_utils.py` & `straxen-2.0.7/tests/test_holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_itp_map.py` & `straxen-2.0.7/tests/test_itp_map.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_led_calibration.py` & `straxen-2.0.7/tests/test_led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_mini_analyses.py` & `straxen-2.0.7/tests/test_mini_analyses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_misc.py` & `straxen-2.0.7/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_nveto_events.py` & `straxen-2.0.7/tests/test_nveto_events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_nveto_recorder.py` & `straxen-2.0.7/tests/test_nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_patternfit.py` & `straxen-2.0.7/tests/test_patternfit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_peaklet_processing.py` & `straxen-2.0.7/tests/test_peaklet_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_peaks.py` & `straxen-2.0.7/tests/test_peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_scada.py` & `straxen-2.0.7/tests/test_scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_url_config.py` & `straxen-2.0.7/tests/test_url_config.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.6/tests/test_veto_hitlets.py` & `straxen-2.0.7/tests/test_veto_hitlets.py`

 * *Files identical despite different names*

