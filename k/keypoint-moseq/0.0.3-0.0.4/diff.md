# Comparing `tmp/keypoint-moseq-0.0.3.tar.gz` & `tmp/keypoint-moseq-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.0.3.tar", last modified: Thu Apr 13 22:33:32 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.0.4.tar", last modified: Tue Apr 25 13:08:41 2023, max compression
```

## Comparing `keypoint-moseq-0.0.3.tar` & `keypoint-moseq-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-13 22:33:32.435466 keypoint-moseq-0.0.3/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.3/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.3/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-13 22:33:32.435588 keypoint-moseq-0.0.3/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4694 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.3/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-13 22:33:32.432396 keypoint-moseq-0.0.3/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      659 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17686 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    16272 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    32764 2023-04-13 16:54:16.000000 keypoint-moseq-0.0.3/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    30075 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    60436 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.3/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-13 22:33:32.435139 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      414 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      124 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-04-13 22:33:32.436096 keypoint-moseq-0.0.3/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      807 2023-04-13 22:32:55.000000 keypoint-moseq-0.0.3/setup.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-25 13:08:41.336174 keypoint-moseq-0.0.4/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.4/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.4/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-25 13:08:41.336442 keypoint-moseq-0.0.4/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1394 2023-04-23 11:46:01.000000 keypoint-moseq-0.0.4/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-25 13:08:41.333438 keypoint-moseq-0.0.4/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      784 2023-04-25 13:04:51.000000 keypoint-moseq-0.0.4/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-04-21 10:40:06.000000 keypoint-moseq-0.0.4/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17686 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.4/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17163 2023-04-25 13:04:51.000000 keypoint-moseq-0.0.4/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    32788 2023-04-23 11:46:01.000000 keypoint-moseq-0.0.4/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    26851 2023-04-23 11:46:01.000000 keypoint-moseq-0.0.4/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    66369 2023-04-25 13:04:51.000000 keypoint-moseq-0.0.4/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-25 13:08:41.335715 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      414 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      136 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-04-25 13:08:41.337339 keypoint-moseq-0.0.4/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      830 2023-04-25 13:07:50.000000 keypoint-moseq-0.0.4/setup.py
```

### Comparing `keypoint-moseq-0.0.3/LICENSE.md` & `keypoint-moseq-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.3/NOTICE.md` & `keypoint-moseq-0.0.4/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.3/keypoint_moseq/analysis.py` & `keypoint-moseq-0.0.4/keypoint_moseq/analysis.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.3/keypoint_moseq/calibration.py` & `keypoint-moseq-0.0.4/keypoint_moseq/calibration.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.3/keypoint_moseq/fitting.py` & `keypoint-moseq-0.0.4/keypoint_moseq/fitting.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,30 +6,51 @@
 import warnings
 warnings.formatwarning = lambda msg, *a: str(msg)
 from textwrap import fill
 from datetime import datetime
 
 from keypoint_moseq.viz import plot_progress
 from keypoint_moseq.io import save_checkpoint, format_data, save_hdf5
-from keypoint_moseq.util import get_durations, batch, unbatch, get_frequencies, pad_along_axis, reindex_by_frequency
+from keypoint_moseq.util import get_durations, get_frequencies, pad_along_axis, reindex_by_frequency
 from jax_moseq.models.keypoint_slds import estimate_coordinates, resample_model, init_model
+from jax_moseq.utils import check_for_nans, batch, unbatch
+
+class StopResampling(Exception):
+    pass
 
 def _update_history(history, iteration, model, include_states=True): 
     
     model_snapshot = {
         'params': jax.device_get(model['params']),
         'seed': jax.device_get(model['seed'])}
     
     if include_states: 
         model_snapshot['states'] = jax.device_get(model['states'])
         
     history[iteration] = model_snapshot
     return history
 
 
+def _wrapped_resample(data, model, **resample_options):
+    try: 
+        resample_model(data, **model, **resample_options)
+    except KeyboardInterrupt: 
+        print('Early termination of fitting: user interruption')
+        raise StopResampling()
+
+    any_nans, nan_info, messages = check_for_nans(model)
+    
+    if any_nans:
+        print('Early termination of fitting: NaNs encountered')
+        for msg in messages: print('  - {}'.format(msg))
+        print('\nFor additional information, see https://keypoint-moseq.readthedocs.io/en/latest/troubleshooting.html#nans-during-fitting')
+        raise StopResampling()
+    
+    return model
+
 
 def fit_model(model,
               data,
               labels,
               start_iter=0,
               history=None,
               verbose=True,
@@ -146,15 +167,14 @@
             '``save_progress_figs=False``')
         if name is None: 
             name = str(datetime.now().strftime('%Y_%m_%d-%H_%M_%S'))
         savedir = os.path.join(project_dir,name)
         if not os.path.exists(savedir): os.makedirs(savedir)
         print(fill(f'Outputs will be saved to {savedir}'))
 
-    
     if history is None: history = {}
 
     for iteration in tqdm.trange(start_iter, num_iters+1):
         if history_every_n_iters>0 and (iteration%history_every_n_iters)==0:
             history = _update_history(history, iteration, model, 
                                      include_states=states_in_history)
             
@@ -163,17 +183,19 @@
                           savefig=save_progress_figs, project_dir=project_dir)
 
         if save_every_n_iters>0 and (iteration%save_every_n_iters)==0:
             save_checkpoint(model, data, history, labels, iteration, name=name,
                             project_dir=project_dir,save_history=save_history, 
                             save_states=save_states, save_data=save_data)
             
-        try: model = resample_model(data, **model, ar_only=ar_only, verbose=verbose)
-        except KeyboardInterrupt: break
-    
+        try: model = _wrapped_resample(
+            data, model, ar_only=ar_only, verbose=verbose)
+        except StopResampling: break
+
+
     return model, history, name
     
     
 def resume_fitting(*, params, hypparams, labels, iteration, mask,
                    Y, conf, seed, noise_prior=None, states=None, **kwargs):
     """Resume fitting a model from a checkpoint."""
     
@@ -197,15 +219,16 @@
             to allow parallelization during fitting. In this case,
             set ``use_saved_states=True`` and provide ``states``.
         - The model is being applied to new data. In this case,
             set ``use_saved_states=False``.
 
     Model outputs are saved to disk as a .h5 file, either at ``results_path``
     if it is specified, or at ``{project_dir}/{name}/results.h5`` if it is not.
-    The results have the following structure::
+    If a .h5 file with the given path already exists, the outputs will be added
+    to it. The results have the following structure::
 
         results.h5
         ├──session_name1
         │  ├──syllables             # model state sequence (z), shape=(T,)
         │  ├──syllables_reindexed   # states reindexed by frequency, shape=(T,)
         │  ├──estimated_coordinates # model predicted coordinates, shape=(T,n_keypoints,dim)
         │  ├──latent_state          # model latent state (x), shape=(T,latent_dim)
@@ -311,15 +334,18 @@
         states = None
         noise_prior = None
     
     model = init_model(data, states, params, noise_prior=noise_prior, verbose=verbose, **kwargs)
     
     if num_iters>0:
         for iteration in tqdm.trange(num_iters, desc='Applying model'):
-            model = resample_model(data, **model, ar_only=ar_only, states_only=True, verbose=verbose)
+            try: model = _wrapped_resample(
+                    data, model, ar_only=ar_only, states_only=True, verbose=verbose)
+            except StopResampling: break
+
 
     nlags = model['hypparams']['ar_hypparams']['nlags']
     states = jax.device_get(model['states'])                     
     estimated_coords = jax.device_get(estimate_coordinates(
         **model['states'], **model['params'], **data))
     z_reindexed = reindex_by_frequency(states['z'], np.array(data['mask']))
```

### Comparing `keypoint-moseq-0.0.3/keypoint_moseq/io.py` & `keypoint-moseq-0.0.4/keypoint_moseq/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 import re
 import pandas as pd
 from datetime import datetime
 from textwrap import fill
 from vidio.read import OpenCVReader
 warnings.formatwarning = lambda msg, *a: str(msg)
 
+from jax_moseq.utils import batch
 from keypoint_moseq.util import (
-    batch, 
     reindex_by_bodyparts, 
     list_files_with_exts, 
     interpolate_keypoints,
 )
 
 
+
+
 def _build_yaml(sections, comments):
     text_blocks = []
     for title,data in sections:
         centered_title = f' {title} '.center(50, '=')
         text_blocks.append(f"\n\n{'#'}{centered_title}{'#'}")
         for key,value in data.items():
             text = yaml.dump({key:value}).strip('\n')
```

### Comparing `keypoint-moseq-0.0.3/keypoint_moseq/util.py` & `keypoint-moseq-0.0.4/keypoint_moseq/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -325,119 +325,24 @@
 
     """
     pad_widths_full = [(0,0)]*len(arr.shape)
     pad_widths_full[axis] = pad_widths
     padded_arr = np.pad(arr, pad_widths_full, constant_values=value)
     return padded_arr
 
-
-def unbatch(data, labels): 
-    """
-    Invert :py:func:`keypoint_moseq.util.batch`
- 
-    Parameters
-    -------
-    data: ndarray, shape (num_segs, seg_length, ...)
-        Stack of segmented time-series
-
-    labels: tuples (str,int,int)
-        Labels for the rows of ``data`` as tuples with the form
-        (name,start,end)
-
-    Returns
-    -------
-    data_dict: dict
-        Dictionary mapping names to reconstructed time-series
-    """     
-    data_dict = {}
-    keys = sorted(set([key for key,start,end in labels]))    
-    for key in keys:
-        length = np.max([e for k,s,e in labels if k==key])
-        seq = np.zeros((int(length),*data.shape[2:]), dtype=data.dtype)
-        for (k,s,e),d in zip(labels,data):
-            if k==key: seq[s:e] = d[:e-s]
-        data_dict[key] = seq
-    return data_dict
-
-
-def batch(data_dict, keys=None, seg_length=None, seg_overlap=30):
-    """
-    Stack time-series data of different lengths into a single array for
-    batch processing, optionally breaking up the data into fixed length 
-    segments. Data is 0-padded so that the stacked array isn't ragged.
-
-    Parameters
-    -------
-    data_dict: dict {str : ndarray}
-        Dictionary mapping names to ndarrays, where the first dim
-        represents time. All data arrays must have the same shape except
-        for the first dim. 
-
-    keys: list of str, default=None
-        Optional list of names specifying which datasets to include in 
-        the output and what order to put them in. Each name must be a 
-        key in ``data_dict``. If ``keys=None``, names will be sorted 
-        alphabetically.
-
-    seg_length: int, default=None
-        Break each time-series into segments of this length. If 
-        ``seg_length=None``, the final stacked array will be as long
-        as the longest time-series. 
-
-    seg_overlap: int, default=30
-        Amount of overlap between segments. For example, setting
-        ``seg_length=N`` and ``seg_overlap=M`` will result in segments
-        with start/end times (0, N+M), (N, 2*N+M), (2*N, 3*N+M),...
-
-    Returns
-    -------
-    data: ndarray, shape (N, seg_length, ...)
-        Stacked data array
-
-    mask: ndarray, shape (N, seg_length)
-        Binary indicator specifying which elements of ``data`` are not
-        padding (``mask==0`` in padded locations)
-
-    keys: list of tuples (str,int), length N
-        Row labels for ``data`` consisting (name, segment_num) pairs
-
-    """
-    if keys is None: keys = sorted(data_dict.keys())
-    Ns = [len(data_dict[key]) for key in keys]
-    if seg_length is None: seg_length = np.max(Ns)
-        
-    stack,mask,labels = [],[],[]
-    for key,N in zip(keys,Ns):
-        for start in range(0,N,seg_length):
-            arr = data_dict[key]
-            end = min(start+seg_length+seg_overlap, N)
-            pad_length = seg_length+seg_overlap-(end-start)
-            padding = np.zeros((pad_length,*arr.shape[1:]), dtype=arr.dtype)
-            mask.append(np.hstack([np.ones(end-start),np.zeros(pad_length)]))
-            stack.append(np.concatenate([arr[start:end],padding],axis=0))
-            labels.append((key,start,end))
-
-    stack = np.stack(stack)
-    mask = np.stack(mask)
-    return stack,mask,labels
-
-
-    
 def filter_angle(angles, size=9, axis=0):
     """
     Perform median filtering on time-series of angles by transforming to
     a (cos,sin) representation, filtering in R^2, and then transforming 
     back into angle space. 
-
     Parameters
     -------
     angles: ndarray, Array of angles (in radians)
     size: int, default=9, Size of the filtering kernel
     axis: int, default=0, Axis along which to filter
-
     Returns
     -------
     filtered_angles: ndarray
     """
     kernel = np.where(np.arange(len(angles.shape))==axis, size, 1)
     return np.arctan2(median_filter(np.sin(angles), kernel),
                       median_filter(np.cos(angles), kernel))
```

### Comparing `keypoint-moseq-0.0.3/keypoint_moseq/viz.py` & `keypoint-moseq-0.0.4/keypoint_moseq/viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,20 +198,160 @@
         
         if savefig:
             assert project_dir is not None, fill(
                 'The ``savefig`` option requires a ``project_dir``')
             plt.savefig(os.path.join(project_dir,f'pcs-{name}.pdf'))
         plt.show()
         
+
+def plot_syllable_frequencies(results=None, path=None, project_dir=None, 
+                              name=None, use_reindexed=True, minlength=10,
+                              min_frequency=0.005):
+    """
+    Plot a histogram showing the frequency of each syllable.
+    
+    Caller must provide a results dictionary, a path to a results .h5,
+    or a project directory and model name, in which case the results are
+    loaded from ``{project_dir}/{name}/results.h5``.
+
+    Parameters
+    ----------
+    results : dict, default=None
+        Dictionary containing modeling results for a dataset (see
+        :py:func:`keypoint_moseq.fitting.apply_model`)
+
+    name: str, default=None
+        Name of the model. Required to load results if ``results`` is 
+        None and ``path`` is None. 
+        
+    project_dir: str, default=None
+        Project directory. Required to load results if ``results`` is 
+        None and ``path`` is None. 
+
+    path: str, default=None
+        Path to a results file. If None, results will be loaded from
+        ``{project_dir}/{name}/results.h5``.
+
+    use_reindexed: bool, default=True
+        Whether to use label syllables by their frequency rank (True) or
+        or their original label (False). When reindexing, "0"  represents
+        the most frequent syllable).
+
+    minlength: int, default=10
+        Minimum x-axis length of the histogram.
+
+    min_frequency: float, default=0.005
+        Minimum frequency of syllables to include in the histogram.
+
+    Returns
+    -------
+    fig : matplotlib.figure.Figure
+        Figure containing the histogram.
+    
+    ax : matplotlib.axes.Axes
+        Axes containing the histogram.
+    """
+    if results is None:
+        results = load_results(path=path, name=name, project_dir=project_dir)
+
+    syllable_key = 'syllables' if not use_reindexed else 'syllables_reindexed'
+    syllables = {k:res[syllable_key] for k,res in results.items()}
+    frequencies = get_frequencies(syllables)
+    frequencies = frequencies[frequencies>min_frequency]
+    xmax = max(minlength, len(frequencies))
+
+    fig, ax = plt.subplots()
+    ax.bar(range(len(frequencies)),frequencies,width=1)
+    ax.set_ylabel('probability')
+    ax.set_xlabel('syllable rank')
+    ax.set_xlim(-1,xmax+1)
+    ax.set_title('Frequency distribution')
+    ax.set_yticks([])
+    return fig, ax
+
+
+def plot_duration_distribution(results=None, path=None, project_dir=None, 
+                               name=None, use_reindexed=True, lim=None,
+                               num_bins=30, fps=None):
+    """
+    Plot a histogram showing the frequency of each syllable.
+    
+    Caller must provide a results dictionary, a path to a results .h5,
+    or a project directory and model name, in which case the results are
+    loaded from ``{project_dir}/{name}/results.h5``.
+
+    Parameters
+    ----------
+    results : dict, default=None
+        Dictionary containing modeling results for a dataset (see
+        :py:func:`keypoint_moseq.fitting.apply_model`)
+
+    name: str, default=None
+        Name of the model. Required to load results if ``results`` is 
+        None and ``path`` is None. 
+        
+    project_dir: str, default=None
+        Project directory. Required to load results if ``results`` is 
+        None and ``path`` is None. 
+
+    path: str, default=None
+        Path to a results file. If None, results will be loaded from
+        ``{project_dir}/{name}/results.h5``.
+
+    lim: tuple, default=None
+        x-axis limits as a pair of ints (in units of frames). If None,
+        the limits are set to (0, 95th-percentile).
+
+    num_bins: int, default=30
+        Number of bins in the histogram.
+
+    fps: int, default=None
+        Frames per second. Used to convert x-axis from frames to seconds.
+
+    Returns
+    -------
+    fig : matplotlib.figure.Figure
+        Figure containing the histogram.
+    
+    ax : matplotlib.axes.Axes
+        Axes containing the histogram.
+    """
+    if results is None:
+        results = load_results(path=path, name=name, project_dir=project_dir)
+
+    syllable_key = 'syllables' if not use_reindexed else 'syllables_reindexed'
+    syllables = {k:res[syllable_key] for k,res in results.items()}
+    durations = get_durations(syllables)
+    
+    if lim is None:
+        lim = int(np.percentile(durations, 95))
+    binsize = max(int(np.floor(lim/num_bins)),1)
+
+    if fps is not None:
+        durations = durations/fps
+        binsize = binsize/fps
+        lim = lim/fps
+        xlabel = 'syllable duration (s)'
+    else:
+        xlabel = 'syllable duration (frames)'
+
+    fig, ax = plt.subplots()
+    ax.hist(durations, range=(0,lim), bins=(int(lim/binsize)), density=True)
+    ax.set_xlim([0,lim])
+    ax.set_xlabel(xlabel)
+    ax.set_ylabel('probability')
+    ax.set_title('Duration distribution')
+    ax.set_yticks([])
+    return fig, ax
         
 
 def plot_progress(model, data, history, iteration, path=None,
                   project_dir=None, name=None, savefig=True,
                   fig_size=None, seq_length=600, min_frequency=.001, 
-                  **kwargs):
+                  min_histogram_length=10, **kwargs):
     """
     Plot the progress of the model during fitting.
 
     The figure shows the following plots:
         - Duration distribution: 
             The distribution of state durations for the most recent
             iteration of the model.
@@ -249,17 +389,28 @@
     seq_length : int, default=600
         Length of the state sequence history plot.
 
     min_frequency : float, default=.001
         Minimum frequency for including a state in the frequency 
         distribution plot.
 
+    min_histogram_length : int, default=10
+        Minimum x-axis length of the frequency distribution plot.
+
     project_dir : str, default=None
     name : str, default=None
     path : str, default=None
+
+    Returns
+    -------
+    fig : matplotlib.figure.Figure
+        Figure containing the plots.
+
+    axs : list of matplotlib.axes.Axes
+        Axes containing the plots.
     """
     z = np.array(model['states']['z'])
     mask = np.array(data['mask'])
     durations = get_durations(z,mask)
     frequencies = get_frequencies(z,mask)
     
     history_iters = np.array(sorted(history.keys()))
@@ -271,23 +422,24 @@
         fig,axs = plt.subplots(1,4, gridspec_kw={'width_ratios':[1,1,1,3]})
         if fig_size is None: fig_size=(12,2.5)
     else: 
         fig,axs = plt.subplots(1,2)
         if fig_size is None: fig_size=(4,2.5)
 
     frequencies = np.sort(frequencies[frequencies>min_frequency])[::-1]
+    xmax = max(len(frequencies),min_histogram_length)
     axs[0].bar(range(len(frequencies)),frequencies,width=1)
     axs[0].set_ylabel('probability')
     axs[0].set_xlabel('syllable rank')
+    axs[0].set_xlim([-1,xmax+1])
     axs[0].set_title('Frequency distribution')
     axs[0].set_yticks([])
     
     lim = int(np.percentile(durations, 95))
     binsize = max(int(np.floor(lim/30)),1)
-    lim = lim-(lim%binsize)
     axs[1].hist(durations, range=(1,lim), bins=(int(lim/binsize)), density=True)
     axs[1].set_xlim([1,lim])
     axs[1].set_xlabel('syllable duration (frames)')
     axs[1].set_ylabel('probability')
     axs[1].set_title('Duration distribution')
     axs[1].set_yticks([])
     
@@ -324,14 +476,16 @@
             assert name is not None and project_dir is not None, fill(
                 'The ``savefig`` option requires either a ``path`` '
                 'or a ``name`` and ``project_dir``')
             path = os.path.join(project_dir,name,'fitting_progress.pdf')
         plt.savefig(path)  
     plt.show()
 
+    return fig,axs
+
     
 def write_video_clip(frames, path, fps=30, quality=7):
     """
     Write a video clip to a file.
 
     Parameters
     ----------
@@ -558,18 +712,17 @@
         Minimum frequency of a syllable to be included in the grid movies.
 
     min_duration: int, default=3
         Minimum duration of a syllable instance to be included in the 
         grid movie for that syllable. 
 
     use_reindexed: bool, default=True
-        Determines the naming of syllables (``results["syllables"]`` if 
-        False, or ``results["syllables_reindexed"]`` if True). The
-        reindexed naming corresponds to the rank order of syllable
-        frequency (e.g. "0" for the most frequent syllable).
+        Whether to use label syllables by their frequency rank (True) or
+        or their original label (False). When reindexing, "0"  represents
+        the most frequent syllable).
 
     sampling_options: dict, default={}
         Dictionary of options for sampling syllable instances (see
         :py:func:`keypoint_moseq.util.sample_instances`).
     
     coordinates: dict, default=None
         Dictionary mapping session names to keypoint coordinates as 
@@ -647,14 +800,21 @@
     syllables = {k:v[syllable_key] for k,v in results.items()}
     centroids = {k:v['centroid'] for k,v in results.items()}
     headings = {k:v['heading'] for k,v in results.items()}
 
     syllable_instances = get_syllable_instances(
         syllables, pre=pre, post=post, min_duration=min_duration,
         min_frequency=min_frequency, min_instances=rows*cols)
+    
+    if len(syllable_instances) == 0:
+        warnings.warn(fill(
+            'No syllables with sufficient instances to make a grid movie. '
+            'This usually occurs when all frames have the same syllable label '
+            '(use `plot_syllable_frequencies` to check if this is the case)'))
+        return
 
     sampled_instances = sample_instances(
         syllable_instances, rows*cols, coordinates=coordinates, 
         centroids=centroids, headings=headings, **sampling_options)
 
     centroids,headings = filter_centroids_headings(
         centroids, headings, filter_size=filter_size)
@@ -973,18 +1133,17 @@
         Minimum frequency of a syllable to plotted.
 
     min_duration: float, default=3
         Minimum duration of a syllable instance to be included in the
         trajectory average.
 
     use_reindexed: bool, default=True
-        Determines the naming of syllables (``results["syllables"]`` if 
-        False, or ``results["syllables_reindexed"]`` if True). The
-        reindexed naming corresponds to the rank order of syllable
-        frequency (e.g. "0" for the most frequent syllable).
+        Whether to use label syllables by their frequency rank (True) or
+        or their original label (False). When reindexing, "0"  represents
+        the most frequent syllable).
 
     bodyparts: list of str, default=None
         List of bodypart names in ``coordinates``. 
 
     use_bodyparts: list of str, default=None
         Ordered list of bodyparts to include in trajectory plot.
         If None, all bodyparts will be included.
@@ -1056,14 +1215,21 @@
     headings = {k:v['heading'] for k,v in results.items()}
     plot_options.update({'keypoint_colormap':keypoint_colormap})
             
     syllable_instances = get_syllable_instances(
         syllables, pre=pre, post=post, min_duration=min_duration,
         min_frequency=min_frequency, min_instances=num_samples)
     
+    if len(syllable_instances) == 0:
+        warnings.warn(fill(
+            'No syllables with sufficient instances to make a trajectory plot. '
+            'This usually occurs when all frames have the same syllable label '
+            '(use `plot_syllable_frequencies` to check if this is the case)'))
+        return
+    
     sampling_options['n_neighbors'] = num_samples
     sampled_instances = sample_instances(
         syllable_instances, num_samples, coordinates=coordinates, 
         centroids=centroids, headings=headings, **sampling_options)
 
     trajectories = {syllable: get_trajectories(
         instances, coordinates, pre=pre, post=post, 
@@ -1469,19 +1635,18 @@
         Minimum frequency of a syllable to be included in the crowd movies.
 
     min_duration: int, default=3
         Minimum duration of a syllable instance to be included in the 
         crowd movie for that syllable. 
 
     use_reindexed: bool, default=True
-        Determines the naming of syllables (``results["syllables"]`` if 
-        False, or ``results["syllables_reindexed"]`` if True). The
-        reindexed naming corresponds to the rank order of syllable
-        frequency (e.g. "0" for the most frequent syllable).
-    
+        Whether to use label syllables by their frequency rank (True) or
+        or their original label (False). When reindexing, "0"  represents
+        the most frequent syllable).
+
     bodyparts: list of str, default=None
         List of bodypart names in ``coordinates``. 
 
     use_bodyparts: list of str, default=None
         Ordered list of bodyparts to include in the crowd
         movies. If None, all bodyparts will be included.
         
@@ -1549,14 +1714,21 @@
                 '``use_bodyparts`` must be specified')
             edges = get_edges(use_bodyparts, skeleton)
         else: edges = skeleton
 
     syllable_instances = get_syllable_instances(
         syllables, pre=pre, post=post, min_duration=min_duration,
         min_frequency=min_frequency, min_instances=num_instances)
+    
+    if len(syllable_instances) == 0:
+        warnings.warn(fill(
+            'No syllables with sufficient instances to make a crowd movie. '
+            'This usually occurs when all frames have the same syllable label '
+            '(use `plot_syllable_frequencies` to check if this is the case)'))
+        return
 
     sampled_instances = sample_instances(
         syllable_instances, num_instances, coordinates=coordinates, 
         centroids=centroids, headings=headings, **sampling_options)
 
     for syllable,instances in tqdm.tqdm(
         sampled_instances.items(), desc='Generating crowd movies'):
```

### Comparing `keypoint-moseq-0.0.3/setup.py` & `keypoint-moseq-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='keypoint-moseq',
-    version='0.0.3',
+    version='0.0.4',
     author='Caleb Weinreb',
     author_email='calebsw@gmail.com',
     include_package_data=True,
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent'
@@ -18,14 +18,15 @@
     install_requires=[
         'seaborn',
         'cytoolz',
         'matplotlib',
         'tqdm',
         'ipykernel',
         'imageio[ffmpeg]',
+        'statsmodels',
         'pyyaml',
         'vidio',
         'holoviews[recommended]',
         'bokeh',
         'pandas',
         'tables',
         'jax-moseq',
```

