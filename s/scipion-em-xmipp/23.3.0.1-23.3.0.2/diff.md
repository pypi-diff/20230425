# Comparing `tmp/scipion-em-xmipp-23.3.0.1.tar.gz` & `tmp/scipion-em-xmipp-23.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-xmipp-23.3.0.1.tar", last modified: Tue Mar 28 12:44:00 2023, max compression
+gzip compressed data, was "scipion-em-xmipp-23.3.0.2.tar", last modified: Tue Apr 25 11:11:16 2023, max compression
```

## Comparing `scipion-em-xmipp-23.3.0.1.tar` & `scipion-em-xmipp-23.3.0.2.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:44:00.383733 scipion-em-xmipp-23.3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-28 12:44:00.383733 scipion-em-xmipp-23.3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:44:00.363733 scipion-em-xmipp-23.3.0.1/scipion_em_xmipp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-28 12:44:00.000000 scipion-em-xmipp-23.3.0.1/scipion_em_xmipp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-03-28 12:44:00.000000 scipion-em-xmipp-23.3.0.1/scipion_em_xmipp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:44:00.000000 scipion-em-xmipp-23.3.0.1/scipion_em_xmipp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-28 12:44:00.000000 scipion-em-xmipp-23.3.0.1/scipion_em_xmipp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-28 12:44:00.000000 scipion-em-xmipp-23.3.0.1/scipion_em_xmipp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 12:44:00.000000 scipion-em-xmipp-23.3.0.1/scipion_em_xmipp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:44:00.383733 scipion-em-xmipp-23.3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:44:00.363733 scipion-em-xmipp-23.3.0.1/xmipp3/
--rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26010 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:44:00.363733 scipion-em-xmipp-23.3.0.1/xmipp3/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62027 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/convert/io_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/programs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:44:00.375733 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18950 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_align_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_align_volume_and_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_analyze_local_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_angular_graph_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_apply_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_apply_deformation_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_apply_transformation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_apply_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_assignment_tilt_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_break_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_center_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    27226 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_cl2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_cl2d_align.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classes_2d_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classification_gpuCorr.py
--rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classification_gpuCorr_full.py
--rw-r--r--   0 runner    (1001) docker     (123)    18244 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classification_gpuCorr_semi.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classify_kmeans2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_compare_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_compare_reprojections.py
--rw-r--r--   0 runner    (1001) docker     (123)    31955 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_consensus_classes3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_consensus_local_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_convert_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_core_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_create_gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)    42641 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ctf_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ctf_correct_wiener2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ctf_defocus_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ctf_micrographs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21324 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_deep_denoising.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_deep_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)    21735 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_deep_micrograph_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_denoise_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_eliminate_empty_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    25080 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_enrich.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_extract_asymmetric_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_extract_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_extract_particles_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_extract_particles_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18475 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_flexalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_generate_reprojections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_helical_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_kerdensom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_kmeans_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_local_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_metaprotocol_create_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32782 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_metaprotocol_golden_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ml2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_movie_gain.py
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_movie_max_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    18030 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_movie_opticalflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_movie_split_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_multiple_fscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27778 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_multireference_alignability.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_normalize_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_boxsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick_automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick_remove_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_phantom_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_pick_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_postProcessing_deepPostProcessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:44:00.375733 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/geometrical_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_create_mask2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_create_mask3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_crop_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_image_operate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_movie_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    39852 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    24220 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess_micrographs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:44:00.375733 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/projmatch_form.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/projmatch_initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    34600 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/projmatch_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/protocol_projmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_random_conical_tilt.py
--rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ransac.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_reconstruct_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)   107816 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_reconstruct_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_reconstruct_significant.py
--rw-r--r--   0 runner    (1001) docker     (123)    30163 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_reconstruct_swarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_bfactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_deepres.py
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_fso.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_monogenic_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_rotate_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_rotational_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_rotational_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    88133 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_screen_deepConsensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_screen_deeplearning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_screen_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_shift_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_shift_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_simulate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    29287 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_solid_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_split_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_split_volume_hierarchical_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_structure_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_structure_map_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_subtract_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    28360 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_tilt_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_trigger_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23655 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_validate_fscq.py
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_validate_nontilt.py
--rw-r--r--   0 runner    (1001) docker     (123)    25116 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_validate_overfitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_adjust_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_deform_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_local_sharpening.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_write_testC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_write_testP.py
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:44:00.379733 scipion-em-xmipp-23.3.0.1/xmipp3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44475 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_convert_xmipp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_angular_graph_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_apply_transformation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_compare_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_consensus_classes3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_ctf_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_deep_denoising.py
--rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_extract_asymmetric_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_monodir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_multiple_fsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_multireference_alignability.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_reconstruct_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_screen_deepConsensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_simulate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_validate_fscq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_validate_overfitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_continuousflex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_deepVolPostprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_deepres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_fso.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_gpuCorr_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_gpuCorr_fullStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_gpuCorr_semiStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_local_defocus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_localdeblur.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_metaprotocol_golden_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_mixed_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_monores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_realignment_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_solid_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    76668 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)   161922 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    61131 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_mics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_movie_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:44:00.383733 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_analyze_local_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_cl2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_classes3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_consensus_classes3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_ctf_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_deepEMHancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_deep_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_deep_micrograph_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_eliminate_empty_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_extract_asymmetric_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_local_sharpening.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_metaprotocol_golden_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_ml2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_movie_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_normalize_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_pdb_deform_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_projmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_ransac.py
--rw-r--r--   0 runner    (1001) docker     (123)    13184 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_reconstruct_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_bfactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_deepres.py
--rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_fso.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_monogenic_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_solid_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_split_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    14398 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_structure_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_subtract_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_swarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18651 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_validate_fscq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_validate_nontilt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_validate_overfitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_volume_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_volume_deform_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_volume_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_volume_subtraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20151 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)    84496 2023-03-28 12:41:59.000000 scipion-em-xmipp-23.3.0.1/xmipp3/xmipp_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:11:16.722180 scipion-em-xmipp-23.3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-25 11:11:16.722180 scipion-em-xmipp-23.3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:11:16.702180 scipion-em-xmipp-23.3.0.2/scipion_em_xmipp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-25 11:11:16.000000 scipion-em-xmipp-23.3.0.2/scipion_em_xmipp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-04-25 11:11:16.000000 scipion-em-xmipp-23.3.0.2/scipion_em_xmipp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:11:16.000000 scipion-em-xmipp-23.3.0.2/scipion_em_xmipp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-25 11:11:16.000000 scipion-em-xmipp-23.3.0.2/scipion_em_xmipp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 11:11:16.000000 scipion-em-xmipp-23.3.0.2/scipion_em_xmipp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 11:11:16.000000 scipion-em-xmipp-23.3.0.2/scipion_em_xmipp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:11:16.726179 scipion-em-xmipp-23.3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:11:16.702180 scipion-em-xmipp-23.3.0.2/xmipp3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26010 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:11:16.702180 scipion-em-xmipp-23.3.0.2/xmipp3/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62027 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/convert/io_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/programs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:11:16.714180 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18950 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_align_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_align_volume_and_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_analyze_local_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_angular_graph_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_apply_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_apply_deformation_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_apply_transformation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_apply_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_assignment_tilt_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_break_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_center_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27226 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_cl2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_cl2d_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classes_2d_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classification_gpuCorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classification_gpuCorr_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18244 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classification_gpuCorr_semi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classify_kmeans2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_compare_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_compare_reprojections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31955 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_consensus_classes3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_consensus_local_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_convert_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_core_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_create_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42641 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ctf_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ctf_correct_wiener2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ctf_defocus_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ctf_micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21324 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_deep_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_deep_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21735 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_deep_micrograph_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_denoise_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_eliminate_empty_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25080 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_extract_asymmetric_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_extract_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_extract_particles_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_extract_particles_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18475 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_flexalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_generate_reprojections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_helical_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_kerdensom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_kmeans_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_local_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_metaprotocol_create_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32782 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_metaprotocol_golden_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ml2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_movie_gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_movie_max_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18030 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_movie_opticalflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_movie_split_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_multiple_fscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27778 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_multireference_alignability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_normalize_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_boxsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick_automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick_remove_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_phantom_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_pick_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_postProcessing_deepPostProcessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:11:16.714180 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/geometrical_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_create_mask2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_create_mask3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_crop_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_image_operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_movie_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39852 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24220 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess_micrographs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:11:16.718180 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/projmatch_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/projmatch_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34600 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/projmatch_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/protocol_projmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_random_conical_tilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_reconstruct_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107816 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_reconstruct_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_reconstruct_significant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30163 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_reconstruct_swarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_bfactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_deepres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_fso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_monogenic_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_rotate_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_rotational_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_rotational_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88133 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_screen_deepConsensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_screen_deeplearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_screen_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_shift_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_shift_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_simulate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29287 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_solid_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_split_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_split_volume_hierarchical_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_structure_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_structure_map_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_subtract_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28360 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_tilt_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_trigger_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23655 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_validate_fscq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_validate_nontilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25116 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_validate_overfitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_adjust_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_deform_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_local_sharpening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_write_testC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_write_testP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:11:16.718180 scipion-em-xmipp-23.3.0.2/xmipp3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44475 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_convert_xmipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_angular_graph_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_apply_transformation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_compare_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_consensus_classes3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_ctf_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_deep_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_extract_asymmetric_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_monodir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_multiple_fsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_multireference_alignability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_reconstruct_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_screen_deepConsensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_simulate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_validate_fscq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_validate_overfitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_continuousflex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_deepVolPostprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_deepres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_fso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_gpuCorr_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_gpuCorr_fullStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_gpuCorr_semiStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_local_defocus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_localdeblur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_metaprotocol_golden_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_mixed_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_monores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_realignment_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_solid_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76668 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161922 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61131 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_mics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_movie_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:11:16.722180 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_analyze_local_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_cl2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_classes3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_consensus_classes3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_ctf_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_deepEMHancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_deep_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_deep_micrograph_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_eliminate_empty_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_extract_asymmetric_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_local_sharpening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_metaprotocol_golden_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_ml2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_movie_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_normalize_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_pdb_deform_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_projmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13184 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_reconstruct_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_bfactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_deepres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_fso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_monogenic_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_solid_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_split_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14398 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_structure_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_subtract_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_swarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18651 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_validate_fscq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_validate_nontilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_validate_overfitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_volume_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_volume_deform_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_volume_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_volume_subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20151 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84496 2023-04-25 11:09:35.000000 scipion-em-xmipp-23.3.0.2/xmipp3/xmipp_logo.png
```

### Comparing `scipion-em-xmipp-23.3.0.1/CHANGES.txt` & `scipion-em-xmipp-23.3.0.2/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/LICENSE` & `scipion-em-xmipp-23.3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/PKG-INFO` & `scipion-em-xmipp-23.3.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipp
-Version: 23.3.0.1
+Version: 23.3.0.2
 Summary: Plugin to use Xmipp programs within the Scipion framework (see https://scipion-em.github.io/docs/).
 Home-page: https://github.com/i2pc/scipion-em-xmipp
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: [![Build](https://github.com/I2PC/scipion-em-xmipp/actions/workflows/build.yml/badge.svg)](https://github.com/I2PC/scipion-em-xmipp/actions/workflows/build.yml)
```

### Comparing `scipion-em-xmipp-23.3.0.1/README.md` & `scipion-em-xmipp-23.3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/scipion_em_xmipp.egg-info/PKG-INFO` & `scipion-em-xmipp-23.3.0.2/scipion_em_xmipp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipp
-Version: 23.3.0.1
+Version: 23.3.0.2
 Summary: Plugin to use Xmipp programs within the Scipion framework (see https://scipion-em.github.io/docs/).
 Home-page: https://github.com/i2pc/scipion-em-xmipp
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: [![Build](https://github.com/I2PC/scipion-em-xmipp/actions/workflows/build.yml/badge.svg)](https://github.com/I2PC/scipion-em-xmipp/actions/workflows/build.yml)
```

### Comparing `scipion-em-xmipp-23.3.0.1/scipion_em_xmipp.egg-info/SOURCES.txt` & `scipion-em-xmipp-23.3.0.2/scipion_em_xmipp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/setup.py` & `scipion-em-xmipp-23.3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/__init__.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from .base import *
 from .constants import XMIPP_HOME, XMIPP_URL, XMIPP_DLTK_NAME
 
 _logo = "xmipp_logo.png"
 _references = ['delaRosaTrevin2013', 'Sorzano2013']
 _currentBinVersion = '3.23.03.0'
 # This will allow scipion to detect the plugin version and print it in the log.
-__version__ = _currentBinVersion[2:] + ".1"  # Set this to ".0" on each xmipp binary release, otherwise increase it --> ".1", ".2", ...
+__version__ = _currentBinVersion[2:] + ".2"  # Set this to ".0" on each xmipp binary release, otherwise increase it --> ".1", ".2", ...
 
 
 class Plugin(pwem.Plugin):
     _homeVar = XMIPP_HOME
     _pathVars = [XMIPP_HOME]
     _supportedVersions = []
     _url = XMIPP_URL
```

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/base.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/bibtex.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/constants.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/convert/__init__.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/convert/convert.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/convert/dataimport.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/convert/io_coordinates.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/convert/io_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/programs.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/programs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/__init__.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_align_volume.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_align_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_align_volume_and_particles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_align_volume_and_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_analyze_local_ctf.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_analyze_local_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_angular_graph_consistency.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_angular_graph_consistency.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_apply_alignment.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_apply_alignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_apply_deformation_zernike3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_apply_deformation_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_apply_transformation_matrix.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_apply_transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_apply_zernike3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_apply_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_assignment_tilt_pair.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_assignment_tilt_pair.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_break_symmetry.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_break_symmetry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_center_particles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_center_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_cl2d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_cl2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_cl2d_align.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_cl2d_align.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classes_2d_mapping.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classes_2d_mapping.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classification_gpuCorr.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classification_gpuCorr.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classification_gpuCorr_full.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classification_gpuCorr_full.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classification_gpuCorr_semi.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classification_gpuCorr_semi.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_classify_kmeans2d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_classify_kmeans2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_compare_angles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_compare_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_compare_reprojections.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_compare_reprojections.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_consensus_classes3D.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_consensus_classes3D.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_consensus_local_ctf.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_consensus_local_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_convert_pdb.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_convert_pdb.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_core_analysis.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_core_analysis.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_create_gallery.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_create_gallery.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ctf_consensus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ctf_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ctf_correct_wiener2d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ctf_correct_wiener2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ctf_defocus_group.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ctf_defocus_group.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ctf_micrographs.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ctf_micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_deep_denoising.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_deep_denoising.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_deep_hand.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_deep_hand.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_deep_micrograph_screen.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_deep_micrograph_screen.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_denoise_particles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_denoise_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_eliminate_empty_images.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_eliminate_empty_images.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_enrich.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_enrich.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_extract_asymmetric_unit.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_extract_asymmetric_unit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_extract_particles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_extract_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_extract_particles_movies.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_extract_particles_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_extract_particles_pairs.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_extract_particles_pairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_flexalign.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_flexalign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_generate_reprojections.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_generate_reprojections.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_helical_parameters.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_helical_parameters.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_kerdensom.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_kerdensom.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_kmeans_clustering.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_kmeans_clustering.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_local_ctf.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_local_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_metaprotocol_create_subset.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_metaprotocol_create_subset.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_metaprotocol_golden_highres.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_metaprotocol_golden_highres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ml2d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ml2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_movie_gain.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_movie_gain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_movie_max_shift.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_movie_max_shift.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_movie_opticalflow.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_movie_opticalflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_movie_split_frames.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_movie_split_frames.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_multiple_fscs.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_multiple_fscs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_multireference_alignability.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_multireference_alignability.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_normalize_strain.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_normalize_strain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_boxsize.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_boxsize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick_automatic.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick_automatic.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick_consensus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick_pairs.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick_pairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_particle_pick_remove_duplicates.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_particle_pick_remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_phantom_create.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_phantom_create.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_pick_noise.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_pick_noise.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_postProcessing_deepPostProcessing.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_postProcessing_deepPostProcessing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/__init__.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/geometrical_mask.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/geometrical_mask.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_add_noise.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_add_noise.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_create_mask2d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_create_mask2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_create_mask3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_create_mask3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_crop_resize.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_crop_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_filter.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_filter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_image_operate.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_image_operate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_mask.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_mask.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_movie_resize.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_movie_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_preprocess.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_preprocess.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess/protocol_process.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess/protocol_process.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_preprocess_micrographs.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_preprocess_micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/__init__.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/projmatch_form.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/projmatch_form.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/projmatch_initialize.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/projmatch_initialize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/projmatch_steps.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/projmatch_steps.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_projmatch/protocol_projmatch.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_projmatch/protocol_projmatch.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_random_conical_tilt.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_random_conical_tilt.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_ransac.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_ransac.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_reconstruct_fourier.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_reconstruct_fourier.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_reconstruct_highres.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_reconstruct_highres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_reconstruct_significant.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_reconstruct_significant.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_reconstruct_swarm.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_reconstruct_swarm.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_bfactor.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_bfactor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_deepres.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_deepres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_directional.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_directional.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_fso.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_fso.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_resolution_monogenic_signal.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_resolution_monogenic_signal.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_rotate_volume.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_rotate_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_rotational_spectra.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_rotational_spectra.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_rotational_symmetry.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_rotational_symmetry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_screen_deepConsensus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_screen_deepConsensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_screen_deeplearning.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_screen_deeplearning.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_screen_particles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_screen_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_shift_particles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_shift_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_shift_volume.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_shift_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_simulate_ctf.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_simulate_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_solid_angles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_solid_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_split_volume.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_split_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_split_volume_hierarchical_cluster.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_split_volume_hierarchical_cluster.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_structure_map.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_structure_map.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_structure_map_zernike3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_structure_map_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_subtract_projection.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_subtract_projection.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_tilt_analysis.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_tilt_analysis.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_trigger_data.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_trigger_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_validate_fscq.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_validate_fscq.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_validate_nontilt.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_validate_nontilt.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_validate_overfitting.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_validate_overfitting.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_adjust_sub.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_adjust_sub.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_consensus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_deform_zernike3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_deform_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_local_sharpening.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_local_sharpening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_volume_strain.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_volume_strain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_write_testC.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_write_testC.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols/protocol_write_testP.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols/protocol_write_testP.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/protocols.conf` & `scipion-em-xmipp-23.3.0.2/xmipp3/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_convert_xmipp.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_convert_xmipp.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_angular_graph_consistency.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_angular_graph_consistency.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_apply_transformation_matrix.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_apply_transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_compare_angles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_compare_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_consensus_classes3D.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_consensus_classes3D.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_ctf_consensus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_ctf_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_deep_denoising.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_deep_denoising.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_extract_asymmetric_unit.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_extract_asymmetric_unit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_monodir.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_monodir.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_multiple_fsc.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_multiple_fsc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_multireference_alignability.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_multireference_alignability.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_reconstruct_fourier.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_reconstruct_fourier.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_screen_deepConsensus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_screen_deepConsensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_simulate_ctf.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_simulate_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_validate_fscq.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_validate_fscq.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocol_validate_overfitting.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocol_validate_overfitting.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_add_noise.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_add_noise.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_continuousflex.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_continuousflex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_deepVolPostprocessing.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_deepVolPostprocessing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_deepres.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_deepres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_fso.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_fso.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_gpuCorr_classifier.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_gpuCorr_classifier.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_gpuCorr_fullStreaming.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_gpuCorr_fullStreaming.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_gpuCorr_semiStreaming.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_gpuCorr_semiStreaming.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_highres.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_highres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_local_defocus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_local_defocus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_localdeblur.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_localdeblur.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_metaprotocol_golden_highres.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_metaprotocol_golden_highres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_mixed_movies.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_mixed_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_monores.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_monores.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_realignment_classes.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_realignment_classes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_solid_angles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_solid_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_2d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_mics.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_mics.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_movie_resize.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_movie_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_xmipp_movies.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_xmipp_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/tests/test_protocols_zernike3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/tests/test_protocols_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/utils.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/__init__.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/plotter.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/plotter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_analyze_local_ctf.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_analyze_local_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_cl2d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_cl2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_classes3D.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_classes3D.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_consensus_classes3D.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_consensus_classes3D.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_ctf_consensus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_ctf_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_deepEMHancer.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_deepEMHancer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_deep_consensus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_deep_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_deep_micrograph_cleaner.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_deep_micrograph_cleaner.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_eliminate_empty_images.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_eliminate_empty_images.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_extract_asymmetric_unit.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_extract_asymmetric_unit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_local_sharpening.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_local_sharpening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_metaprotocol_golden_highres.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_metaprotocol_golden_highres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_ml2d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_ml2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_movie_alignment.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_movie_alignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_normalize_strain.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_normalize_strain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_pdb_deform_zernike3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_pdb_deform_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_projmatch.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_projmatch.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_ransac.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_ransac.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_reconstruct_highres.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_reconstruct_highres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_bfactor.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_bfactor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_deepres.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_deepres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_directional.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_directional.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_fso.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_fso.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_resolution_monogenic_signal.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_resolution_monogenic_signal.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_solid_angles.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_solid_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_split_volume.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_split_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_structure_map.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_structure_map.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_subtract_projection.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_subtract_projection.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_swarm.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_swarm.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_validate_fscq.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_validate_fscq.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_validate_nontilt.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_validate_nontilt.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_validate_overfitting.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_validate_overfitting.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_volume_consensus.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_volume_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_volume_deform_zernike3d.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_volume_deform_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_volume_strain.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_volume_strain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/viewers/viewer_volume_subtraction.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/viewers/viewer_volume_subtraction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/wizards.py` & `scipion-em-xmipp-23.3.0.2/xmipp3/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.1/xmipp3/xmipp_logo.png` & `scipion-em-xmipp-23.3.0.2/xmipp3/xmipp_logo.png`

 * *Files identical despite different names*

