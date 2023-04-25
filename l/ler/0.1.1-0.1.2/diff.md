# Comparing `tmp/ler-0.1.1.tar.gz` & `tmp/ler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ler-0.1.1.tar", last modified: Wed Apr 12 05:31:39 2023, max compression
+gzip compressed data, was "ler-0.1.2.tar", last modified: Tue Apr 25 09:33:40 2023, max compression
```

## Comparing `ler-0.1.1.tar` & `ler-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-12 05:31:39.248831 ler-0.1.1/
--rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-04-12 05:31:39.248533 ler-0.1.1/PKG-INFO
--rw-r--r--   0 hemantaph   (501) staff       (20)       50 2023-04-12 04:14:44.000000 ler-0.1.1/README.md
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-12 05:31:39.246292 ler-0.1.1/ler/
--rw-r--r--   0 hemantaph   (501) staff       (20)      248 2023-04-09 00:20:02.000000 ler-0.1.1/ler/__init__.py
--rw-r--r--   0 hemantaph   (501) staff       (20)     7651 2023-04-09 00:20:55.000000 ler-0.1.1/ler/helperroutines.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    28242 2023-04-09 00:20:55.000000 ler-0.1.1/ler/lens_galaxy_population.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    17424 2023-04-09 00:20:55.000000 ler-0.1.1/ler/ler.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    53400 2023-04-09 00:20:02.000000 ler-0.1.1/ler/ler_old1.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    18973 2023-04-09 00:20:02.000000 ler-0.1.1/ler/ler_old2.py
--rw-r--r--   0 hemantaph   (501) staff       (20)     5759 2023-04-09 00:20:55.000000 ler-0.1.1/ler/solve_lens_equation.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    11812 2023-04-09 00:20:55.000000 ler-0.1.1/ler/source_population.py
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-12 05:31:39.248149 ler-0.1.1/ler.egg-info/
--rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/PKG-INFO
--rw-r--r--   0 hemantaph   (501) staff       (20)      315 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/SOURCES.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)        1 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/dependency_links.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)      131 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/requires.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)        4 2023-04-12 05:31:39.000000 ler-0.1.1/ler.egg-info/top_level.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)       38 2023-04-12 05:31:39.248930 ler-0.1.1/setup.cfg
--rw-r--r--   0 hemantaph   (501) staff       (20)      592 2023-04-12 05:31:26.000000 ler-0.1.1/setup.py
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-25 09:33:40.090283 ler-0.1.2/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-04-25 09:33:40.089932 ler-0.1.2/PKG-INFO
+-rw-r--r--   0 hemantaph   (501) staff       (20)       50 2023-04-12 04:14:44.000000 ler-0.1.2/README.md
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-25 09:33:40.085946 ler-0.1.2/ler/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      314 2023-04-18 09:53:24.000000 ler-0.1.2/ler/__init__.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)     7651 2023-04-25 09:26:09.000000 ler-0.1.2/ler/helperroutines.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    29191 2023-04-25 09:25:05.000000 ler-0.1.2/ler/lens_galaxy_population.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    36372 2023-04-25 09:24:51.000000 ler-0.1.2/ler/ler.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    12758 2023-04-25 09:25:14.000000 ler-0.1.2/ler/multiprocessing_routine.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    11811 2023-04-25 09:25:23.000000 ler-0.1.2/ler/source_population.py
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-25 09:33:40.089429 ler-0.1.2/ler.egg-info/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-04-25 09:33:39.000000 ler-0.1.2/ler.egg-info/PKG-INFO
+-rw-r--r--   0 hemantaph   (501) staff       (20)      287 2023-04-25 09:33:40.000000 ler-0.1.2/ler.egg-info/SOURCES.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)        1 2023-04-25 09:33:39.000000 ler-0.1.2/ler.egg-info/dependency_links.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)      131 2023-04-25 09:33:39.000000 ler-0.1.2/ler.egg-info/requires.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)        4 2023-04-25 09:33:39.000000 ler-0.1.2/ler.egg-info/top_level.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)       38 2023-04-25 09:33:40.090405 ler-0.1.2/setup.cfg
+-rw-r--r--   0 hemantaph   (501) staff       (20)      592 2023-04-25 09:32:09.000000 ler-0.1.2/setup.py
```

### Comparing `ler-0.1.1/ler/helperroutines.py` & `ler-0.1.2/ler/helperroutines.py`

 * *Files identical despite different names*

### Comparing `ler-0.1.1/ler/lens_galaxy_population.py` & `ler-0.1.2/ler/lens_galaxy_population.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 from source_population import CompactBinaryPopulation
 from helperroutines import add_dictionaries_together, trim_dictionary
 # for multiprocessing 
 from multiprocessing import Pool
 from tqdm import tqdm
 
 # multiprocessing routines
-import solve_lens_equation
-
-min_images = 2
-max_images = 5 
+import multiprocessing_routine as mp
 
 class LensGalaxyPopulation():
     def __init__(self, CompactBinaryPopulation_=False):
         '''
         class for lens galaxy population sampling
         Also includes functions to calculate lensed event rate
         Input parameters:
@@ -32,15 +29,15 @@
         Output parameters:
             None
         '''
         
         if CompactBinaryPopulation_==False:
             # initialization of clasess
             # CompactBinaryPopulation already inherits from Source_Galaxy_Population_Model class form source_population.py
-            self.CompactBinaryPopulation = CompactBinaryPopulation(z_min=0.0001, z_max=10., m_min=4.59, m_max=86.22, event_type = "StellarBBH")
+            self.CompactBinaryPopulation = CompactBinaryPopulation(z_min=0., z_max=10., m_min=4.59, m_max=86.22, event_type = "StellarBBH")
         else:
             # if the classes are already initialized, then just use them
             self.CompactBinaryPopulation = CompactBinaryPopulation_
 
         self.z_min = self.CompactBinaryPopulation.z_min
         self.z_max = self.CompactBinaryPopulation.z_max
         self.m_min = self.CompactBinaryPopulation.m_min
@@ -97,51 +94,74 @@
         r = np.linspace(0, 1, num = 100)
         u = 10*r**3 - 15*r**4 + 6*r**5 # See the integral of Eq. A7 of https://arxiv.org/pdf/1807.07062.pdf (cdf)
         self.lens_redshift_sampler_helper_function = interp1d(u, r, kind = 'cubic') # Computes r(u)
         
         # Create a lookup table for the differential comoving volume
         self.differential_comoving_volume = self.CompactBinaryPopulation.differential_comoving_volume
         return None
-
+    
     def sample_lens_parameters(self, size=1000, lens_parameters_input={}):
         '''
         Function to sample galaxy lens parameters
         Input parameters:
             size : number of lens parameters to sample
             lens_parameters_input : dictionary of lens parameters to sample
         Output parameters:
             lens_parameters : dictionary of lens parameters and source parameters (lens conditions applied)
                             e.g. dictionary keys: 
                             lensing related=>['zl':redshift of lens, 'zs': redshift of source, 'sigma':velocity dispersion, 'q':axis ratios, 'e1':ellipticity, 'e2':ellipticity, 'gamma1':external-shear, 'gamma2':external-shear, 'Dl':angular diameter distance of lens, 'Ds':angular diameter distance of source, 'Dls':angular diameter distance between lens and source, 'theta_E': einstein radius in radian, 'gamma':spectral index of mass density distribution]
                             source related=>['mass_1': mass in detector frame (mass1>mass2), 'mass_2': mass in detector frame, 'mass_1_source':mass in source frame, 'mass_2_source':mass source frame, 'luminosity_distance': luminosity distance, 'iota': inclination angle, 'psi': polarization angle, 'phase': coalesence phase, 'geocent_time': coalensence GPS time at geocenter, 'ra': right ascension, 'dec': declination,]
                                     
         '''
+        print('sampling PEMD lens galaxy (with external shear) parameters...')
+        return self.sample_lens_parameters_routine(size=size, lens_parameters_input=lens_parameters_input)
+        
+    def sample_lens_parameters_routine(self, size=1000, lens_parameters_input={}):
+        '''
+        Function to sample galaxy lens parameters
+        Input parameters:
+            size : number of lens parameters to sample
+            lens_parameters_input : dictionary of lens parameters to sample
+        Output parameters:
+            lens_parameters : dictionary of lens parameters and source parameters (lens conditions applied)
+                            e.g. dictionary keys: 
+                            lensing related=>['zl':redshift of lens, 'zs': redshift of source, 'sigma':velocity dispersion, 'q':axis ratios, 'e1':ellipticity, 'e2':ellipticity, 'gamma1':external-shear, 'gamma2':external-shear, 'Dl':angular diameter distance of lens, 'Ds':angular diameter distance of source, 'Dls':angular diameter distance between lens and source, 'theta_E': einstein radius in radian, 'gamma':spectral index of mass density distribution]
+                            source related=>['mass_1': mass in detector frame (mass1>mass2), 'mass_2': mass in detector frame, 'mass_1_source':mass in source frame, 'mass_2_source':mass source frame, 'luminosity_distance': luminosity distance, 'iota': inclination angle, 'psi': polarization angle, 'phase': coalesence phase, 'geocent_time': coalensence GPS time at geocenter, 'ra': right ascension, 'dec': declination,]
+                                    
+        '''
+        
         # Sample source redshifts from the source population
         # rejection sampled with optical depth
+        #print('sampling source parameters...')
         source_params_strongly_lensed = self.sample_strongly_lensed_source_parameters(size=size)
         zs = source_params_strongly_lensed['zs']
 
         # Sample lens redshifts
+        #print("sampling lens's redshifts...")
         zl = self.sample_lens_redshifts(zs)
         # Sample velocity dispersions and axis ratios (note: these should be sampled together because the lensing probability depends on the combination of these two parameters)
         sigma, q = self.sample_velocity_dispersion_axis_ratio(zs)
 
         # Compute the Einstein radii
+        # print("sampling einstein radius...")
         theta_E = self.compute_einstein_radii(sigma, zl, zs)
 
         # Sample the axis ratio angle
+        # print("sampling axis ratio and angle...")
         axis_ratio_angle_phi = self.sample_axis_ratio_angle_phi(size=size)
 
         # Transform the axis ratio and the angle, to ellipticities e1, e2, using lenstronomy
         e1, e2 = phi_q2_ellipticity(axis_ratio_angle_phi, q)
 
         # Sample shears
+        # print("sampling external shears...")
         gamma1, gamma2 = self.sample_galaxy_shear(size=size)
 
         # Sample the spectral index of the mass density distribution
+        # print("sampling spectral index...")
         gamma = self.sample_gamma(size=size)
 
         # Compute the angular diameter distances
         Dl = self.angular_diameter_distance(zl) # for the lens
         Ds = self.angular_diameter_distance(zs) # for the source
         # Compute Dls also
         Dls = self.angular_diameter_distance_z1z2(zl, zs) # for the lens-source pair
@@ -164,15 +184,16 @@
         # Check if the lens are larger than requested size
         if len(lens_parameters['zl']) >= size:
             # Trim dicitionary to right size
             lens_parameters = trim_dictionary(lens_parameters, size)
             return lens_parameters
         else:
             # Run iteratively until we have the right number of lensing parmaeters
-            return self.sample_lens_parameters(size=size, lens_parameters_input=lens_parameters)
+            #print("current sampled size", len(lens_parameters['zl']))
+            return self.sample_lens_parameters_routine(size=size, lens_parameters_input=lens_parameters)
         
     
     def sample_strongly_lensed_source_parameters(self, size=1000):
         '''
         Function to sample source redshifts and other parameters, conditioned on the source being strongly lensed
         PDF of source redshifts : R0(zs)/(1+zs) * dVc/dz * tau(zs)
         where R0(zs) is the source redshift distribution, dVc/dz is the comoving volume element, and tau(zs) is the strong lensing optical depth
@@ -315,15 +336,15 @@
         Input parameters:
             size : number of samples
         Output parameters:
             gamma : spectral index of the density profile
         '''
         self.gamma_mean = 2
         self.gamma_std = 0.2
-        return np.random.normal(loc = self.gamma_mean, scale = self.gamma_std, size = size) 
+        return np.random.normal(loc = self.gamma_mean, scale = self.gamma_std, size = size)
     
     def rejection_sample_lensing_probability(self, theta_E):
         '''
         Function to conduct rejection sampling wrt einstein radius
         Input parameters:
             theta_E : einstein radius
         Output parameters:
@@ -343,69 +364,45 @@
             zs : source redshifts
         Output parameters:
             tau : strong lensing optical depth
         '''
         # z to luminosity_distance (luminosity_distance) conversion
         Dc = self.z_to_Dc(zs)*1e-3  # 1e-3 converts Mpc to Gpc
         return( (Dc/62.2)**3 )
-
-    def get_caustics(self, theta_E, gamma, gamma1, gamma2, e1, e2):
-        '''
-        function to get the caustics of the lens
-        Input parameters:
-            theta_E : Einstein radius
-            gamma : spectral index of the density profile
-            gamma1 : shear component in the x-direction
-            gamma2 : shear component in the y-direction
-            e1 : ellipticity component in the x-direction
-            e2 : ellipticity component in the y-direction
-        Output parameters:
-            caustic_double : double caustic
-            caustic_diamond : diamond caustic
-        '''
-        # set up the lens model
-        kwargs_lens = [{'theta_E': theta_E, 'e1': e1, 'e2': e2, 'gamma': gamma, 'center_x': 0.0, 'center_y': 0.0}, 
-                       {'gamma1': gamma1, 'gamma2': gamma2, 'ra_0': 0, 'dec_0':0}]
-        # Get the lensing diamond and double caustics
-        caustic_double_points = caustics_epl_shear(kwargs_lens, return_which='double', maginf=-100)
-        caustic_diamond_points = caustics_epl_shear(kwargs_lens, return_which='caustic', maginf=-100)
-        caustic_double = Polygon(caustic_double_points.T)
-        caustic_diamond = Polygon(caustic_diamond_points.T)
-        return caustic_diamond, caustic_double
     
-    def get_image_properties(self, lens_parameters, lensModelList=['EPL_NUMBA', 'SHEAR'], npool=4):
+    def get_image_properties(self, lens_parameters, n_min_images=int(2), n_max_images=int(4), lensModelList=['EPL_NUMBA', 'SHEAR'], npool=4):
         '''
         Function to get the image properties
         Input parameters:
             lens_parameters : dictionary of lens parameters
                             e.g. lens_parameters.keys() = ['zs', 'zl', 'gamma1', 'gamma2', 'e1', 'e2', 'gamma', 'theta_E']
             lensModelList   : list of lens models
                             e.g. lensModelList = ['EPL_NUMBA', 'SHEAR']
             npool           : number of processes to use
                             to check the number of cores available, use os.cpu_count()
         Output parameters:
             lens_parameters : dictionary of lens parameters and image properties
                             e.g. lens_parameters.keys() = ['zs', 'zl', 'gamma1', 'gamma2', 'e1', 'e2', 'gamma', 'theta_E', 'x_image', 'y_image', 'theta_E_image', 'gamma_image', 'e1_image', 'e2_image', 'phi_image', 'caustic_diamond', 'caustic_double']
         '''
-        n_max_images     = max_images
         zs               = lens_parameters['zs']
         size             = len(zs)
         zl               = lens_parameters['zl']
         # external shear params to the 'PEMD' galaxy lens
         gamma1, gamma2   = lens_parameters['gamma1'], lens_parameters['gamma2']
         # ellipticity of the galaxy lens
         e1, e2           = lens_parameters['e1'], lens_parameters['e2']
         gamma            = lens_parameters['gamma']
         einstein_radius  = lens_parameters['theta_E']
         # Create the lens model list (note: can be a different lens model for different samples)
         lensModelList    = np.array(lensModelList)*np.ones((size,len(lensModelList)),dtype=object) 
-        
+        min_img_arr     = n_min_images*np.ones((size), dtype=int)
+
         # get image properties (with Multiprocessing)
         iterations = np.arange(size)
-        input_arguments = np.array([e1,e2,gamma,gamma1,gamma2,zl,zs,einstein_radius,iterations], dtype=object).T
+        input_arguments = np.array([min_img_arr,e1,e2,gamma,gamma1,gamma2,zl,zs,einstein_radius,iterations], dtype=object).T
         input_arguments = np.concatenate((input_arguments,lensModelList),axis=1)
         # Initialize the image positions and lens argument list here.
         x0_image_positions = np.ones((size, n_max_images))*np.nan
         x1_image_positions = np.ones((size, n_max_images))*np.nan
         magnifications = np.ones((size, n_max_images))*np.nan
         time_delays   = np.ones((size, n_max_images))*np.nan
         determinants  = np.ones((size, n_max_images))*np.nan
@@ -413,19 +410,25 @@
         n_images = np.ones(size, dtype=int)
         x_source, y_source = np.ones(size)*np.nan, np.ones(size)*np.nan
         eta = np.ones(size)*np.nan
         phi = np.ones(size)*np.nan
         weights = np.ones(size)*np.nan
         
         # Solve the lens equation
-        print('solving lens equations, started...')
+        print('solving lens equations...')
+        if n_min_images==2:
+            solve_lens_equation = mp.solve_lens_equation1
+        elif n_min_images>2:
+            solve_lens_equation = mp.solve_lens_equation2
+        else:
+            raise ValueError('n_min_images should be greater than 1')
         with Pool(processes=npool) as pool:
             # call the same function with different data in parallel
             # imap->retain order in the list, while map->doesn't
-            for result in tqdm(pool.imap(solve_lens_equation.solve_lens_equation,input_arguments), total=len(input_arguments), ncols= 100, disable=False): 
+            for result in tqdm(pool.imap(solve_lens_equation,input_arguments), total=len(input_arguments), ncols= 100, disable=False): 
                 #print(result)
                 '''
                 for i in tqdm(range(size)):
                     result = self.solve_lens_equation(input_arguments[i])
                 '''
                 x_source_i, y_source_i, eta_i, phi_i, x0_image_position_i, x1_image_position_i, magnifications_i,time_delays_i, \
                 n_image_i, determinant_i, trace_i, iter_i, weights_i = result
@@ -452,15 +455,14 @@
                 determinants[iter_i]             = determinant
                 traces[iter_i]                   = trace
                 x_source[iter_i]                 = x_source_i
                 y_source[iter_i]                 = y_source_i
                 eta[iter_i]                     = eta_i
                 phi[iter_i]                     = phi_i
                 weights[iter_i]                  = weights_i
-        print('solving lens equations, ended...')   
         
         # time-delays: convert to positive values
         # time-delays will be relative to the first arrived signal of an lensed event
         time_delays = time_delays - np.array([np.sort(time_delays,axis=1)[:,0]]).T
         
         # select only strongly lensed events are selected
         assert np.all(n_images>=2), "There are events with no images!"
@@ -469,20 +471,20 @@
         number_of_lensed_events = size
         image_type                   = np.zeros((number_of_lensed_events,n_max_images))
         image_type[traces < 0]       = 3
         image_type[traces > 0]       = 1
         image_type[determinants < 0] = 2
         
         # Return a dictionary with all of the lens information but also the BBH parameters from gw_param
-        image_parameters = {'n_images':n_images, 'x0_image_positions':x0_image_positions, 'x1_image_positions':x1_image_positions, 'magnifications':magnifications, 'time_delays':time_delays, 'traces':traces, 'determinants':determinants, 'image_type':image_type}
+        image_parameters = {'n_images':n_images, 'x0_image_positions':x0_image_positions, 'x1_image_positions':x1_image_positions, 'magnifications':magnifications, 'time_delays':time_delays, 'traces':traces, 'determinants':determinants, 'image_type':image_type, 'weights': weights}
         lens_parameters.update(image_parameters)
         
         return lens_parameters
 
-    def get_lensed_snrs(self, snr_calculator, lensed_param):
+    def get_lensed_snrs(self, snr_calculator, lensed_param, n_max_images=4):
         ''' 
         Function to calculate the signal to noise ratio for each image in each event.
         Input parameters:
             snr_calculator : snr_calculator class
                             this is an already initialized class that contains a 
                             function (snr_calculator.snr) that actually calculates snr with the given gw_params.
                             snr_calculator.list_of_detectors is a list of detectors that are used in the calculation.
@@ -498,15 +500,14 @@
             snrs = get_lensed_snrs(, lensed_param)
                             
         '''
         # needed to calculate effective luminosity distance and effective time delay
         magnifications = lensed_param['magnifications']
         time_delays    = lensed_param['time_delays']
 
-        n_max_images   = max_images
         # Get the binary parameters
         number_of_lensed_events = len(magnifications)
         mass_1, mass_2, luminosity_distance, iota, psi, ra, dec, geocent_time, phase = \
         lensed_param['mass_1'], lensed_param['mass_2'], lensed_param['luminosity_distance'], lensed_param['iota'], \
         lensed_param['psi'], lensed_param['ra'], lensed_param['dec'], lensed_param['geocent_time'], lensed_param['phase']
         
         # setting up snr dictionary
```

### Comparing `ler-0.1.1/ler/source_population.py` & `ler-0.1.2/ler/source_population.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # for generating mass distribution
 from gwcosmo import priors as p
 # for multiprocessing 
 # Import helper routines
 from helperroutines import rejection_sample
 
 class SourceGalaxyPopulationModel():
-    def __init__(self, z_min=0.0001, z_max=10):
+    def __init__(self, z_min=0., z_max=10.):
         '''
         Functions to create lookup tables for redshifts and distances
         1. Redshift to co-moving distance
         2. Co-moving distance to redshift
         3. Redshift to luminosity distance
         Input parameters:
             z_min (float): minimum redshift of the source population
@@ -56,15 +56,15 @@
         self.z_to_luminosity_distance    = interp1d( z, luminosity_distance, kind = 'cubic')
 
         # Create a lookup table for the differential comoving volume
         dVcdz = Planck18.differential_comoving_volume(z).value*4*np.pi
         self.differential_comoving_volume = interp1d(z, dVcdz, kind='linear', fill_value='extrapolate')
         return None
 
-    def sample_source_redshifts(self, size=1000, z_min=0, z_max=12):
+    def sample_source_redshifts(self, size=1000, z_min=0., z_max=12.):
         '''
         Function to sample source redshifts from the source galaxy population model
         Input parameters:
             size (int): number of source redshifts to sample
             z_min (float): minimum redshift of the source population
             z_max (float): maximum redshift of the source population
         Output parameters:
```

### Comparing `ler-0.1.1/setup.py` & `ler-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 setup(name='ler',
-      version='0.1.1',
+      version='0.1.2',
       description='Lensing Rates',
       author='Hemantakumar',
       license="MIT",
       author_email='hemantaphurailatpam@gmail.com',
       url='https://github.com/hemantaph/ler',
       packages=find_packages(),
       install_requires=[
```

