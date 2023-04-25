# Comparing `tmp/coldxrayPy-1.0.0.tar.gz` & `tmp/coldxrayPy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coldxrayPy-1.0.0.tar", last modified: Mon Apr 24 05:11:26 2023, max compression
+gzip compressed data, was "coldxrayPy-1.1.0.tar", last modified: Tue Apr 25 01:39:59 2023, max compression
```

## Comparing `coldxrayPy-1.0.0.tar` & `coldxrayPy-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 05:11:26.382307 coldxrayPy-1.0.0/
--rw-rw-rw-   0        0        0      103 2023-04-24 05:11:26.381285 coldxrayPy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1371 2023-04-18 19:23:19.000000 coldxrayPy-1.0.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 05:11:26.380270 coldxrayPy-1.0.0/coldxrayPy.egg-info/
--rw-rw-rw-   0        0        0      103 2023-04-24 05:11:26.000000 coldxrayPy-1.0.0/coldxrayPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-24 05:11:26.000000 coldxrayPy-1.0.0/coldxrayPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 05:11:26.000000 coldxrayPy-1.0.0/coldxrayPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 05:11:26.000000 coldxrayPy-1.0.0/coldxrayPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11026 2023-04-24 05:06:42.000000 coldxrayPy-1.0.0/coldxrayPy.py
--rw-rw-rw-   0        0        0      188 2023-04-24 05:11:02.000000 coldxrayPy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 05:11:26.382307 coldxrayPy-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 01:39:59.753425 coldxrayPy-1.1.0/
+-rw-rw-rw-   0        0        0      103 2023-04-25 01:39:59.752428 coldxrayPy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1371 2023-04-18 19:23:19.000000 coldxrayPy-1.1.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 01:39:59.751432 coldxrayPy-1.1.0/coldxrayPy.egg-info/
+-rw-rw-rw-   0        0        0      103 2023-04-25 01:39:59.000000 coldxrayPy-1.1.0/coldxrayPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-25 01:39:59.000000 coldxrayPy-1.1.0/coldxrayPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 01:39:59.000000 coldxrayPy-1.1.0/coldxrayPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 01:39:59.000000 coldxrayPy-1.1.0/coldxrayPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12635 2023-04-25 01:39:00.000000 coldxrayPy-1.1.0/coldxrayPy.py
+-rw-rw-rw-   0        0        0      188 2023-04-25 01:32:17.000000 coldxrayPy-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 01:39:59.753425 coldxrayPy-1.1.0/setup.cfg
```

### Comparing `coldxrayPy-1.0.0/README.txt` & `coldxrayPy-1.1.0/README.txt`

 * *Files identical despite different names*

### Comparing `coldxrayPy-1.0.0/coldxrayPy.py` & `coldxrayPy-1.1.0/coldxrayPy.py`

 * *Files 27% similar despite different names*

```diff
@@ -249,8 +249,50 @@
         for element in self.elements_list:
             if (element.temp > element.ablation_temp):
                 element.is_ablated = True
                 ablated_element_list.append(0)
             else:
                 element.is_ablated = False
                 ablated_element_list.append(1)
-        return ablated_element_list
+        return ablated_element_list
+    
+    
+     #Function to iterate through time for transient thermal analyses for the nomainal condition before cold x-ray exposure.
+
+    def transient_thermal_analysis(self, L, T0, Tinf, rho, c, k, dx, dt, t_max, emissivity, solar_flux):
+        
+        # Calculate the number of spatial and temporal steps
+        n_x = int(L/dx) + 1
+        n_t = int(t_max/dt) + 1
+
+        # Initialize the temperature array
+        T = np.zeros((n_t, n_x))
+
+        # Set the initial temperature
+        T[0,:] = T0
+
+        # Set the boundary conditions
+        T[:,0] = 303.15 #temp of space craft in kelvin
+        T[:,-1] = T[:,-2] + solar_flux*dx/k - emissivity*5.67e-8*(T[:,-2]**4 - Tinf**4)*dx/k
+
+        # Calculate the coefficients
+        alpha = k*dt/(rho*c*dx**2)
+        beta = 1 - 2*alpha
+
+        # Iterate over time
+        for i in range(1, n_t):
+            for j in range(1, n_x-1):
+                T[i,j] = alpha*(T[i-1,j+1] + T[i-1,j-1]) + beta*T[i-1,j]
+
+            # Update the boundary conditions
+            T[i,0] = 303.15 #temperature of space craft in kelvin
+            T[i,-1] = T[i,-2] + solar_flux*dx/k - emissivity*5.67e-8*(T[i,-2]**4 - Tinf**4)*dx/k
+
+        # Plot the temperature vs time at a specific point in the plate
+        t = np.linspace(0, t_max, n_t)
+        plt.plot(t, T[:,int(n_x/2)])
+        plt.xlabel('Time (s)')
+        plt.ylabel('Temperature (K)')
+        plt.title('Temperature vs Time at x = L/2')
+        plt.show()
+
+        #Function to iterate through time for transient thermal analyses for the plate post cold-xray
```

