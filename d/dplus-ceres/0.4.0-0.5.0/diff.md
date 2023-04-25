# Comparing `tmp/dplus_ceres-0.4.0-cp39-cp39-win_amd64.whl.zip` & `tmp/dplus_ceres-0.5.0-cp310-cp310-manylinux_2_24_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,14 @@
-Zip file size: 824008 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat  1917440 b- defN 22-Jun-29 19:55 dplus_ceres.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      887 b- defN 22-Jun-29 19:22 dplus_ceres/call_cost_function.pyx
--rw-rw-rw-  2.0 fat    21040 b- defN 22-Jun-29 19:22 dplus_ceres/dplus_ceres.pyx
--rw-rw-rw-  2.0 fat      987 b- defN 22-Jun-29 19:22 dplus_ceres/iteration_callback_func.pyx
--rw-rw-rw-  2.0 fat     4080 b- defN 22-Jun-29 19:55 dplus_ceres-0.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5335 b- defN 22-Jun-29 19:55 dplus_ceres-0.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Jun-29 19:55 dplus_ceres-0.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 22-Jun-29 19:54 dplus_ceres-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      767 b- defN 22-Jun-29 19:55 dplus_ceres-0.4.0.dist-info/RECORD
-9 files, 1950648 bytes uncompressed, 822684 bytes compressed:  57.8%
+Zip file size: 2206598 bytes, number of entries: 12
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-25 05:20 dplus_ceres.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-25 05:20 dplus_ceres/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-25 05:20 dplus_ceres-0.5.0.dist-info/
+-rwxr-xr-x  2.0 unx  7743920 b- defN 23-Apr-25 05:20 dplus_ceres.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx    20602 b- defN 23-Apr-25 05:20 dplus_ceres/dplus_ceres.pyx
+-rw-r--r--  2.0 unx      862 b- defN 23-Apr-25 05:20 dplus_ceres/call_cost_function.pyx
+-rw-r--r--  2.0 unx      963 b- defN 23-Apr-25 05:20 dplus_ceres/iteration_callback_func.pyx
+-rw-r--r--  2.0 unx     4016 b- defN 23-Apr-25 05:20 dplus_ceres-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      114 b- defN 23-Apr-25 05:20 dplus_ceres-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-25 05:20 dplus_ceres-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      789 b- defN 23-Apr-25 05:20 dplus_ceres-0.5.0.dist-info/RECORD
+-rw-r--r--  2.0 unx     5303 b- defN 23-Apr-25 05:20 dplus_ceres-0.5.0.dist-info/METADATA
+12 files, 7776581 bytes uncompressed, 2204906 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -1,28 +1,37 @@
-Filename: dplus_ceres.cp39-win_amd64.pyd
+Filename: dplus_ceres.libs/
 Comment: 
 
-Filename: dplus_ceres/call_cost_function.pyx
+Filename: dplus_ceres/
+Comment: 
+
+Filename: dplus_ceres-0.5.0.dist-info/
+Comment: 
+
+Filename: dplus_ceres.cpython-310-x86_64-linux-gnu.so
 Comment: 
 
 Filename: dplus_ceres/dplus_ceres.pyx
 Comment: 
 
+Filename: dplus_ceres/call_cost_function.pyx
+Comment: 
+
 Filename: dplus_ceres/iteration_callback_func.pyx
 Comment: 
 
-Filename: dplus_ceres-0.4.0.dist-info/LICENSE
+Filename: dplus_ceres-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: dplus_ceres-0.4.0.dist-info/METADATA
+Filename: dplus_ceres-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: dplus_ceres-0.4.0.dist-info/WHEEL
+Filename: dplus_ceres-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dplus_ceres-0.4.0.dist-info/top_level.txt
+Filename: dplus_ceres-0.5.0.dist-info/RECORD
 Comment: 
 
-Filename: dplus_ceres-0.4.0.dist-info/RECORD
+Filename: dplus_ceres-0.5.0.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## dplus_ceres/call_cost_function.pyx

 * *Ordering differences only*

```diff
@@ -1,26 +1,26 @@
-from libc.stdio cimport printf #printf for debugging
-from libcpp cimport bool
-from libcpp.string cimport string
-
-#although we dont use these imports, without them this file doesnt compile
-import numpy as np
-cimport numpy as np
-
-cdef public bool call_cost_function(obj, const double* x,  double * p, double* residual, int numResiduals, int numParams) :
-    # for some unknown reason you can't use numpy here ( cdef double[:] view fail, np_x.data fail)
-    # however we must convert c types to python types. so we will create python lists that contain the values
-    cdef int i
-    PyX = []
-    for i in range(numResiduals):
-        PyX.append(x[i])
-
-    PyParams =[]
-    for i in range(numParams):
-        PyParams.append(p[i])
-
-    PyResiduals = obj(PyParams, numResiduals)
-
-    for i in range(numResiduals):
-        residual[i] = PyResiduals[i]
-
+from libc.stdio cimport printf #printf for debugging
+from libcpp cimport bool
+from libcpp.string cimport string
+
+#although we dont use these imports, without them this file doesnt compile
+import numpy as np
+cimport numpy as np
+
+cdef public bool call_cost_function(obj, const double* x,  double * p, double* residual, int numResiduals, int numParams) :
+    # for some unknown reason you can't use numpy here ( cdef double[:] view fail, np_x.data fail)
+    # however we must convert c types to python types. so we will create python lists that contain the values
+    cdef int i
+    PyX = []
+    for i in range(numResiduals):
+        PyX.append(x[i])
+
+    PyParams =[]
+    for i in range(numParams):
+        PyParams.append(p[i])
+
+    PyResiduals = obj(PyParams, numResiduals)
+
+    for i in range(numResiduals):
+        residual[i] = PyResiduals[i]
+
     return True
```

## dplus_ceres/dplus_ceres.pyx

 * *Ordering differences only*

```diff
@@ -1,439 +1,439 @@
-# distutils: language = c++
-import cython
-from libcpp.vector cimport vector
-from libc.stdlib cimport malloc, free
-from libc.stdint cimport uint8_t, uint16_t, int32_t, uint64_t
-cimport cython.operator.dereference as drf
-import numpy as np
-cimport numpy as np
-from enum import Enum
-cimport ceres_static
-# from cyres cimport *
-############################
-def enum(*sequential, **named):
-    enums = dict(zip(sequential, range(len(sequential))), **named)
-    reverse = dict((value, key) for key, value in enums.iteritems())
-    enums['reverse_mapping'] = reverse
-    return type('Enum', (), enums)
-
-Ownership = enum("DO_NOT_TAKE_OWNERSHIP", "TAKE_OWNERSHIP")
-
-MinimizerType = enum("LINE_SEARCH", "TRUST_REGION")
-
-LinearSolverType = enum("DENSE_NORMAL_CHOLESKY", "DENSE_QR",
-                        "SPARSE_NORMAL_CHOLESKY", "DENSE_SCHUR", "SPARSE_SCHUR",
-                        "ITERATIVE_SCHUR", "CGNR")
-PreconditionerType = enum("IDENTITY", "JACOBI", "SCHUR_JACOBI",
-                          "CLUSTER_JACOBI", "CLUSTER_TRIDIAGONAL")
-SparseLinearAlgebraLibraryType = enum("SUITE_SPARSE", "CX_SPARSE")
-LinearSolverTerminationType = enum("TOLERANCE", "MAX_ITERATIONS", "STAGNATION",
-                                   "FAILURE")
-LoggingType = enum("SILENT", "PER_MINIMIZER_ITERATION")
-LineSearchDirectionType = enum("STEEPEST_DESCENT",
-                               "NONLINEAR_CONJUGATE_GRADIENT",
-                               "LBFGS")
-NonlinearConjugateGradientType = enum("FLETCHER_REEVES", "POLAK_RIBIRERE",
-                                      "HESTENES_STIEFEL")
-LineSearchType = enum("ARMIJO")
-TrustRegionStrategyType = enum("LEVENBERG_MARQUARDT", "DOGLEG")
-DoglegType = enum("TRADITIONAL_DOGLEG", "SUBSPACE_DOGLEG")
-SolverTerminationType = enum("CONVERGENCE", "NO_CONVERGENCE", "FAILURE", "USER_SUCCESS", "USER_FAILURE")
-CallbackReturnType = enum("SOLVER_CONTINUE", "SOLVER_ABORT", "SOLVER_TERMINATE_SUCCESSFULLY")
-DumpFormatType = enum("CONSOLE", "PROTOBUF", "TEXTFILE")
-DimensionType = enum(DYNAMIC=-1)
-NumericDiffMethod = enum("CENTRAL", "FORWARD")
-
-# This class exist because you can't just send python function to c++
-# You will receive "bad argument to internal function" without it
-class RunCostFunc:
-    def __init__(self, func2run):
-        self.func = func2run
-    def in_func2run(self, params, num_residual):
-        return self.func(params, num_residual)
-cdef class PyResidual: # chana
-    cdef ceres_static.CostFunction* _residual_cost_function
-    def __init__(self, x , y, num_params, num_residual, func2run, step_size, eps, best_param, best_eval):
-        # const double *x, const double *y,
-		# int numParams, int numResiduals, PyCostFuncWrapper calcVector, double stepSize,
-		# double eps, vector[double] pBestParams, double *pBestEval
-        # np_y, num_params, num_residual, func2run, step_size, eps, best_param, best_eval
-        cdef double* _x_ptr = NULL
-        cdef np.ndarray[np.double_t, ndim=1] np_x
-        np_x = x
-        _x_ptr = <double*> np_x.data
-        cdef double* _y_ptr = NULL
-        cdef np.ndarray[np.double_t, ndim=1] np_y
-        np_y = y
-        _x_ptr = <double*> np_y.data
-        cdef np.ndarray[np.double_t, ndim=1] array
-        array = best_param
-        cdef long size = array.size
-        cdef vector[double] best_param_vec
-        cdef long i
-        for i in range(size):
-            best_param_vec.push_back(array[i])
-        in_class = RunCostFunc(func2run) # chana
-        cdef ceres_static.PyCostFuncWrapper func2run_wrapper = ceres_static.PyCostFuncWrapper(in_class.in_func2run) # chana
-        cdef double* _best_v_ptr = NULL
-        cdef np.ndarray[np.double_t, ndim=1] best_v
-        best_v = best_eval
-        _best_v_ptr = <double*> best_v.data
-        self._residual_cost_function = ceres_static.Residual.GetCeresCostFunction(_x_ptr, _y_ptr, num_params, num_residual,
-                                                                            func2run_wrapper, step_size, eps,
-                                                                             best_param_vec, _best_v_ptr)
-cdef class PyCostFunction:
-    cdef ceres_static.CostFunction* _cost_function
-    cpdef parameter_block_sizes(self):
-        block_sizes = []
-        cdef vector[int32_t] _parameter_block_sizes = self._cost_function.parameter_block_sizes()
-        for i in range(_parameter_block_sizes.size()):
-            block_sizes.append(_parameter_block_sizes[i])
-        return block_sizes
-    cpdef num_residuals(self):
-        return self._cost_function.num_residuals()
-    def evaluate(self, *param_blocks, **kwargs):
-        include_jacobians = kwargs.get("include_jacobians", False)
-        cdef double** _params_ptr = NULL
-        cdef double* _residuals_ptr = NULL
-        cdef double** _jacobians_ptr = NULL
-        block_sizes = self.parameter_block_sizes()
-        _params_ptr = <double**> malloc(sizeof(double*)*len(block_sizes))
-        cdef np.ndarray[np.double_t, ndim=1] _param_block
-        for i, param_block in enumerate(param_blocks):
-            if block_sizes[i] != len(param_block):
-                raise Exception("Expected param block of size %d, got %d" % (block_sizes[i], len(param_block)))
-            _param_block = param_block
-            _params_ptr[i] = <double*> _param_block.data
-        cdef np.ndarray[np.double_t, ndim=1] residuals
-        residuals = np.empty((self.num_residuals()), dtype=np.double)
-        _residuals_ptr = <double*> residuals.data
-        cdef np.ndarray[np.double_t, ndim=2] _jacobian
-        if include_jacobians:
-            # jacobians is an array of size CostFunction::parameter_block_sizes_
-            # containing pointers to storage for Jacobian matrices corresponding
-            # to each parameter block. The Jacobian matrices are in the same
-            # order as CostFunction::parameter_block_sizes_. jacobians[i] is an
-            # array that contains CostFunction::num_residuals_ x
-            # CostFunction::parameter_block_sizes_[i] elements. Each Jacobian
-            # matrix is stored in row-major order, i.e., jacobians[i][r *
-            # parameter_block_size_[i] + c]
-            jacobians = []
-            _jacobians_ptr = <double**> malloc(sizeof(double*)*len(block_sizes))
-            for i, block_size in enumerate(block_sizes):
-                jacobian = np.empty((self.num_residuals(), block_size), dtype=np.double)
-                jacobians.append(jacobian)
-                _jacobian = jacobian
-                _jacobians_ptr[i] = <double*> _jacobian.data
-        self._cost_function.Evaluate(_params_ptr, _residuals_ptr, _jacobians_ptr)
-        free(_params_ptr)
-        if include_jacobians:
-            free(_jacobians_ptr)
-            return residuals, jacobians
-        else:
-            return residuals
-cdef class PyLossFunction:
-    cdef ceres_static.LossFunction* _loss_function
-    def __cinit__(self):
-        pass
-cdef class PyTrivialLoss(PyLossFunction):
-    cdef ceres_static.TrivialLoss* _loss
-    def __init__(self):
-        self._loss_function =  self._loss
-cdef class PyHuberLoss(PyLossFunction):
-    cdef ceres_static.HuberLoss* _loss
-    def __init__(self, double _a):
-        self._loss_function =  self._loss
-cdef class PySoftLOneLoss(PyLossFunction):
-    def __init__(self, double _a):
-        self._loss_function =  new ceres_static.SoftLOneLoss(_a)
-cdef class PyCauchyLoss(PyLossFunction):
-    def __init__(self, double _a):
-        self._loss_function =  new ceres_static.CauchyLoss(_a)
-cdef class PyArctanLoss(PyLossFunction):
-    def __init__(self, double _a):
-        """
-        Loss that is capped beyond a certain level using the arc-tangent
-        function. The scaling parameter 'a' determines the level where falloff
-        occurs. For costs much smaller than 'a', the loss function is linear
-        and behaves like TrivialLoss, and for values much larger than 'a' the
-        value asymptotically approaches the constant value of a * PI / 2.
-          rho(s) = a atan(s / a).
-        At s = 0: rho = [0, 1, 0].
-        """
-        self._loss_function =  new ceres_static.ArctanLoss(_a)
-cdef class PyTolerantLoss(PyLossFunction):
-    """
-    Loss function that maps to approximately zero cost in a range around the
-    origin, and reverts to linear in error (quadratic in cost) beyond this
-    range. The tolerance parameter 'a' sets the nominal point at which the
-    transition occurs, and the transition size parameter 'b' sets the nominal
-    distance over which most of the transition occurs. Both a and b must be
-    greater than zero, and typically b will be set to a fraction of a. The
-    slope rho'[s] varies smoothly from about 0 at s <= a - b to about 1 at s >=
-    a + b.
-    The term is computed as:
-      rho(s) = b log(1 + exp((s - a) / b)) - c0.
-    where c0 is chosen so that rho(0) == 0
-      c0 = b log(1 + exp(-a / b)
-    This has the following useful properties:
-      rho(s) == 0               for s = 0
-      rho'(s) ~= 0              for s << a - b
-      rho'(s) ~= 1              for s >> a + b
-      rho''(s) > 0              for all s
-    In addition, all derivatives are continuous, and the curvature is
-    concentrated in the range a - b to a + b.
-    At s = 0: rho = [0, ~0, ~0].
-    """
-    def __init__(self, double _a, double _b):
-        self._loss_function =  new ceres_static.TolerantLoss(_a, _b)
-cdef class PyComposedLoss(PyLossFunction):
-    def __init__(self, PyLossFunction f, PyLossFunction g):
-        self._loss_function =  new ceres_static.ComposedLoss(f._loss_function,
-                                                     ceres_static.DO_NOT_TAKE_OWNERSHIP,
-                                                     g._loss_function,
-                                                     ceres_static.DO_NOT_TAKE_OWNERSHIP)
-cdef class PyScaledLoss(PyLossFunction):
-    def __cinit__(self, PyLossFunction loss_function, double _a):
-        self._loss_function =  new ceres_static.ScaledLoss(loss_function._loss_function,
-                                                   _a,
-                                                   ceres_static.DO_NOT_TAKE_OWNERSHIP)
-    def __dealloc__(self):
-        del self._loss_function
-cdef class PySolverSummary:
-    cdef ceres_static.SolverSummary _summary
-    def briefReport(self):
-        return self._summary.BriefReport()
-    def fullReport(self):
-        return self._summary.FullReport()
-    # def get_ter_type(self):
-    #     return self._summary.termination_type
-    property termination_type:
-        def __get__(self):
-            return self._summary.termination_type
-        def __set__(self, value):
-            self._summary.termination_type = value
-    property final_cost:
-        def __get__(self):
-            return self._summary.final_cost
-cdef class PyProblem:
-    cdef ceres_static.Problem _problem
-    def __cinit__(self):
-        pass
-    # loss_function=NULL yields squared loss
-    cpdef add_residual_block(self,
-                             PyResidual cost_function, # chana
-                             PyLossFunction loss_function,
-                             parameter_blocks=[]):
-        cdef np.ndarray _tmp_array
-        cdef vector[double*] _parameter_blocks
-        cdef double f
-        cdef ceres_static.ResidualBlockId _block_id
-        for parameter_block in parameter_blocks:
-            _tmp_array = np.ascontiguousarray(parameter_block, dtype=np.double)
-            _parameter_blocks.push_back(<double*> _tmp_array.data)
-        _block_id = self._problem.AddResidualBlock(cost_function._residual_cost_function,
-                                                   loss_function._loss_function,
-                                                   _parameter_blocks)
-        block_id = PyResidualBlockId()
-        block_id._block_id = _block_id
-        return block_id
-    cpdef evaluate(self, residual_blocks, apply_loss_function=True):
-        cdef double cost
-        options = PyEvaluateOptions()
-        options.apply_loss_function = apply_loss_function
-        options.residual_blocks = residual_blocks
-        self._problem.Evaluate(options._options, &cost, NULL, NULL, NULL)
-        return cost
-    cpdef set_parameter_block_constant(self, block):
-        cdef np.ndarray _tmp_array = np.ascontiguousarray(block, dtype=np.double)
-        cdef double* _values = <double*> _tmp_array.data
-        self._problem.SetParameterBlockConstant(_values)
-    cpdef set_parameter_block_variable(self, block):
-        cdef np.ndarray _tmp_array = np.ascontiguousarray(block, dtype=np.double)
-        cdef double* _values = <double*> _tmp_array.data
-        self._problem.SetParameterBlockVariable(_values)
-    cpdef set_parameter_lower_bound(self, values, index, lower_bound):
-        cdef np.ndarray _tmp_array = np.ascontiguousarray(values, dtype=np.double)
-        cdef double* _values = <double*> _tmp_array.data
-        self._problem.SetParameterLowerBound(_values, index, lower_bound)
-    cpdef set_parameter_upper_bound(self, values, index, upper_bound):
-        cdef np.ndarray _tmp_array = np.ascontiguousarray(values, dtype=np.double)
-        cdef double* _values = <double*> _tmp_array.data
-        self._problem.SetParameterUpperBound(_values, index, upper_bound)
-def solve(PySolverOptions options, PyProblem problem, PySolverSummary summary):
-    ceres_static.Solve(drf(options._options), &problem._problem, &summary._summary)
-cdef class PyResidualBlockId:
-    cdef ceres_static.ResidualBlockId _block_id
-cdef class PyEvaluateOptions:
-    cdef ceres_static.EvaluateOptions _options
-    def __cinit__(self):
-        pass
-    def __init__(self):
-        self._options = ceres_static.EvaluateOptions()
-    property residual_blocks:
-        def __get__(self):
-            blocks = []
-            cdef int i
-            for i in range(self._options.residual_blocks.size()):
-                block = PyResidualBlockId()
-                block._block_id = self._options.residual_blocks[i]
-                blocks.append(block)
-            return blocks
-        def __set__(self, blocks):
-            self._options.residual_blocks.clear()
-            cdef PyResidualBlockId block
-            for block in blocks:
-                self._options.residual_blocks.push_back(block._block_id)
-    property apply_loss_function:
-        def __get__(self):
-            return self._options.apply_loss_function
-        def __set__(self, value):
-            self._options.apply_loss_function = value
-
-class RunIterationCallbackFunc:
-    def __init__(self, func2run):
-        self.func = func2run
-    def in_func2run(self, iteration_summary=None):
-        return self.func(iteration_summary)
-
-
-cdef class PySolverOptions:
-    cdef ceres_static.SolverOptions* _options
-    cdef ceres_static.PyIterationCallbackWrapper wrapper
-
-    def __cinit__(self):
-        pass
-    def __init__(self):
-        self._options = new ceres_static.SolverOptions() 
-        cdef vector[ceres_static.IterationCallback*] callbacks
-        self._options.callbacks = callbacks
-        
-    def set_callbacks(self, func2run):
-        in_class = RunIterationCallbackFunc(func2run) # chana
-        self.wrapper = ceres_static.PyIterationCallbackWrapper(in_class.in_func2run)
-        cdef vector[ceres_static.IterationCallback*] callbacks
-        callbacks.push_back(<ceres_static.IterationCallback*>&self.wrapper)
-        self._options.callbacks = callbacks
-
-    property max_num_iterations:
-        def __get__(self):
-            return self._options.max_num_iterations
-        def __set__(self, value):
-            self._options.max_num_iterations = value
-    property minimizer_progress_to_stdout:
-        def __get__(self):
-            return self._options.minimizer_progress_to_stdout
-        def __set__(self, value):
-            self._options.minimizer_progress_to_stdout = value
-    property linear_solver_type:
-        def __get__(self):
-            return self._options.linear_solver_type
-        def __set__(self, value):
-            self._options.linear_solver_type = value
-    property trust_region_strategy_type:
-        def __get__(self):
-            return self._options.trust_region_strategy_type
-        def __set__(self, value):
-            new_val = str_to_enum_str(value)
-            int_val = 0
-            if new_val not in TrustRegionStrategyType.reverse_mapping.values():
-                raise Exception("no such trust region strategy type")
-            for key, str_val in TrustRegionStrategyType.reverse_mapping.items():
-                if str_val == new_val:
-                    int_val = key
-            self._options.trust_region_strategy_type = int_val
-    property dogleg_type:
-        def __get__(self):
-            return self._options.dogleg_type
-        def __set__(self, value):
-            self._options.dogleg_type = value
-    property preconditioner_type:
-        def __get__(self):
-            return self._options.preconditioner_type
-        def __set__(self, value):
-            self._options.preconditioner_type = value
-    property num_threads:
-        def __get__(self):
-            return self._options.num_threads
-        def __set__(self, value):
-            self._options.num_threads = value
-    property use_nonmonotonic_steps:
-        def __get__(self):
-            return self._options.use_nonmonotonic_steps
-        def __set__(self, value):
-            self._options.use_nonmonotonic_steps = value
-    property function_tolerance:
-        def __get__(self):
-            return self._options.function_tolerance
-        def __set__(self, value):
-            self._options.function_tolerance = value
-    property update_state_every_iteration:
-        def __get__(self):
-            return self._options.update_state_every_iteration
-        def __set__(self, value):
-            self._options.update_state_every_iteration = value
-    property gradient_tolerance:
-        def __get__(self):
-            return self._options.gradient_tolerance
-        def __set__(self, value):
-            self._options.gradient_tolerance = value
-    property use_inner_iterations:
-        def __get__(self):
-            return self._options.use_inner_iterations
-        def __set__(self, value):
-            self._options.use_inner_iterations = value
-    property minimizer_type:
-        def __get__(self):
-            return self._options.minimizer_type
-        def __set__(self, value):
-            new_val = str_to_enum_str(value)
-            int_val = 0
-            if new_val not in MinimizerType.reverse_mapping.values():
-                raise Exception("no such minimizer type")
-            for key, str_val in MinimizerType.reverse_mapping.items():
-                if str_val == new_val:
-                    int_val = key
-            self._options.minimizer_type = int_val
-    property line_search_direction_type:
-        def __get__(self):
-            return self._options.line_search_direction_type
-        def __set__(self, value):
-            new_val = str_to_enum_str(value)
-            int_val = 0
-            if new_val not in LineSearchDirectionType.reverse_mapping.values():
-                raise Exception("line search direction type")
-            for key, str_val in LineSearchDirectionType.reverse_mapping.items():
-                if str_val == new_val:
-                    int_val = key
-            self._options.line_search_direction_type = int_val
-    property nonlinear_conjugate_gradient_type:
-        def __get__(self):
-            return self._options.nonlinear_conjugate_gradient_type
-        def __set__(self, value):
-            new_val = str_to_enum_str(value)
-            int_val = 0
-            if new_val not in NonlinearConjugateGradientType.reverse_mapping.values():
-                raise Exception("no such nonlinear conjugate gradient type")
-            for key, str_val in NonlinearConjugateGradientType.reverse_mapping.items():
-                if str_val == new_val:
-                    int_val = key
-            self._options.nonlinear_conjugate_gradient_type = int_val
-    property line_search_type:
-        def __get__(self):
-            return self._options.line_search_type
-        def __set__(self, value):
-            new_val = str_to_enum_str(value)
-            int_val = 0
-            if new_val not in LineSearchType.reverse_mapping.values():
-                raise Exception("no such line search type")
-            for key, str_val in LineSearchType.reverse_mapping.items():
-                if str_val == new_val:
-                    int_val = key
-            self._options.line_search_type = int_val
-
-#
-def str_to_enum_str(value):
-    val_up = value.upper()
-    val_rep1 = val_up.replace("-", "_")
-    val_rep2 = val_rep1.replace(" ", "_")
+# distutils: language = c++
+import cython
+from libcpp.vector cimport vector
+from libc.stdlib cimport malloc, free
+from libc.stdint cimport uint8_t, uint16_t, int32_t, uint64_t
+cimport cython.operator.dereference as drf
+import numpy as np
+cimport numpy as np
+from enum import Enum
+cimport ceres_static
+# from cyres cimport *
+############################
+def enum(*sequential, **named):
+    enums = dict(zip(sequential, range(len(sequential))), **named)
+    reverse = dict((value, key) for key, value in enums.iteritems())
+    enums['reverse_mapping'] = reverse
+    return type('Enum', (), enums)
+
+Ownership = enum("DO_NOT_TAKE_OWNERSHIP", "TAKE_OWNERSHIP")
+
+MinimizerType = enum("LINE_SEARCH", "TRUST_REGION")
+
+LinearSolverType = enum("DENSE_NORMAL_CHOLESKY", "DENSE_QR",
+                        "SPARSE_NORMAL_CHOLESKY", "DENSE_SCHUR", "SPARSE_SCHUR",
+                        "ITERATIVE_SCHUR", "CGNR")
+PreconditionerType = enum("IDENTITY", "JACOBI", "SCHUR_JACOBI",
+                          "CLUSTER_JACOBI", "CLUSTER_TRIDIAGONAL")
+SparseLinearAlgebraLibraryType = enum("SUITE_SPARSE", "CX_SPARSE")
+LinearSolverTerminationType = enum("TOLERANCE", "MAX_ITERATIONS", "STAGNATION",
+                                   "FAILURE")
+LoggingType = enum("SILENT", "PER_MINIMIZER_ITERATION")
+LineSearchDirectionType = enum("STEEPEST_DESCENT",
+                               "NONLINEAR_CONJUGATE_GRADIENT",
+                               "LBFGS")
+NonlinearConjugateGradientType = enum("FLETCHER_REEVES", "POLAK_RIBIRERE",
+                                      "HESTENES_STIEFEL")
+LineSearchType = enum("ARMIJO")
+TrustRegionStrategyType = enum("LEVENBERG_MARQUARDT", "DOGLEG")
+DoglegType = enum("TRADITIONAL_DOGLEG", "SUBSPACE_DOGLEG")
+SolverTerminationType = enum("CONVERGENCE", "NO_CONVERGENCE", "FAILURE", "USER_SUCCESS", "USER_FAILURE")
+CallbackReturnType = enum("SOLVER_CONTINUE", "SOLVER_ABORT", "SOLVER_TERMINATE_SUCCESSFULLY")
+DumpFormatType = enum("CONSOLE", "PROTOBUF", "TEXTFILE")
+DimensionType = enum(DYNAMIC=-1)
+NumericDiffMethod = enum("CENTRAL", "FORWARD")
+
+# This class exist because you can't just send python function to c++
+# You will receive "bad argument to internal function" without it
+class RunCostFunc:
+    def __init__(self, func2run):
+        self.func = func2run
+    def in_func2run(self, params, num_residual):
+        return self.func(params, num_residual)
+cdef class PyResidual: # chana
+    cdef ceres_static.CostFunction* _residual_cost_function
+    def __init__(self, x , y, num_params, num_residual, func2run, step_size, eps, best_param, best_eval):
+        # const double *x, const double *y,
+		# int numParams, int numResiduals, PyCostFuncWrapper calcVector, double stepSize,
+		# double eps, vector[double] pBestParams, double *pBestEval
+        # np_y, num_params, num_residual, func2run, step_size, eps, best_param, best_eval
+        cdef double* _x_ptr = NULL
+        cdef np.ndarray[np.double_t, ndim=1] np_x
+        np_x = x
+        _x_ptr = <double*> np_x.data
+        cdef double* _y_ptr = NULL
+        cdef np.ndarray[np.double_t, ndim=1] np_y
+        np_y = y
+        _x_ptr = <double*> np_y.data
+        cdef np.ndarray[np.double_t, ndim=1] array
+        array = best_param
+        cdef long size = array.size
+        cdef vector[double] best_param_vec
+        cdef long i
+        for i in range(size):
+            best_param_vec.push_back(array[i])
+        in_class = RunCostFunc(func2run) # chana
+        cdef ceres_static.PyCostFuncWrapper func2run_wrapper = ceres_static.PyCostFuncWrapper(in_class.in_func2run) # chana
+        cdef double* _best_v_ptr = NULL
+        cdef np.ndarray[np.double_t, ndim=1] best_v
+        best_v = best_eval
+        _best_v_ptr = <double*> best_v.data
+        self._residual_cost_function = ceres_static.Residual.GetCeresCostFunction(_x_ptr, _y_ptr, num_params, num_residual,
+                                                                            func2run_wrapper, step_size, eps,
+                                                                             best_param_vec, _best_v_ptr)
+cdef class PyCostFunction:
+    cdef ceres_static.CostFunction* _cost_function
+    cpdef parameter_block_sizes(self):
+        block_sizes = []
+        cdef vector[int32_t] _parameter_block_sizes = self._cost_function.parameter_block_sizes()
+        for i in range(_parameter_block_sizes.size()):
+            block_sizes.append(_parameter_block_sizes[i])
+        return block_sizes
+    cpdef num_residuals(self):
+        return self._cost_function.num_residuals()
+    def evaluate(self, *param_blocks, **kwargs):
+        include_jacobians = kwargs.get("include_jacobians", False)
+        cdef double** _params_ptr = NULL
+        cdef double* _residuals_ptr = NULL
+        cdef double** _jacobians_ptr = NULL
+        block_sizes = self.parameter_block_sizes()
+        _params_ptr = <double**> malloc(sizeof(double*)*len(block_sizes))
+        cdef np.ndarray[np.double_t, ndim=1] _param_block
+        for i, param_block in enumerate(param_blocks):
+            if block_sizes[i] != len(param_block):
+                raise Exception("Expected param block of size %d, got %d" % (block_sizes[i], len(param_block)))
+            _param_block = param_block
+            _params_ptr[i] = <double*> _param_block.data
+        cdef np.ndarray[np.double_t, ndim=1] residuals
+        residuals = np.empty((self.num_residuals()), dtype=np.double)
+        _residuals_ptr = <double*> residuals.data
+        cdef np.ndarray[np.double_t, ndim=2] _jacobian
+        if include_jacobians:
+            # jacobians is an array of size CostFunction::parameter_block_sizes_
+            # containing pointers to storage for Jacobian matrices corresponding
+            # to each parameter block. The Jacobian matrices are in the same
+            # order as CostFunction::parameter_block_sizes_. jacobians[i] is an
+            # array that contains CostFunction::num_residuals_ x
+            # CostFunction::parameter_block_sizes_[i] elements. Each Jacobian
+            # matrix is stored in row-major order, i.e., jacobians[i][r *
+            # parameter_block_size_[i] + c]
+            jacobians = []
+            _jacobians_ptr = <double**> malloc(sizeof(double*)*len(block_sizes))
+            for i, block_size in enumerate(block_sizes):
+                jacobian = np.empty((self.num_residuals(), block_size), dtype=np.double)
+                jacobians.append(jacobian)
+                _jacobian = jacobian
+                _jacobians_ptr[i] = <double*> _jacobian.data
+        self._cost_function.Evaluate(_params_ptr, _residuals_ptr, _jacobians_ptr)
+        free(_params_ptr)
+        if include_jacobians:
+            free(_jacobians_ptr)
+            return residuals, jacobians
+        else:
+            return residuals
+cdef class PyLossFunction:
+    cdef ceres_static.LossFunction* _loss_function
+    def __cinit__(self):
+        pass
+cdef class PyTrivialLoss(PyLossFunction):
+    cdef ceres_static.TrivialLoss* _loss
+    def __init__(self):
+        self._loss_function =  self._loss
+cdef class PyHuberLoss(PyLossFunction):
+    cdef ceres_static.HuberLoss* _loss
+    def __init__(self, double _a):
+        self._loss_function =  self._loss
+cdef class PySoftLOneLoss(PyLossFunction):
+    def __init__(self, double _a):
+        self._loss_function =  new ceres_static.SoftLOneLoss(_a)
+cdef class PyCauchyLoss(PyLossFunction):
+    def __init__(self, double _a):
+        self._loss_function =  new ceres_static.CauchyLoss(_a)
+cdef class PyArctanLoss(PyLossFunction):
+    def __init__(self, double _a):
+        """
+        Loss that is capped beyond a certain level using the arc-tangent
+        function. The scaling parameter 'a' determines the level where falloff
+        occurs. For costs much smaller than 'a', the loss function is linear
+        and behaves like TrivialLoss, and for values much larger than 'a' the
+        value asymptotically approaches the constant value of a * PI / 2.
+          rho(s) = a atan(s / a).
+        At s = 0: rho = [0, 1, 0].
+        """
+        self._loss_function =  new ceres_static.ArctanLoss(_a)
+cdef class PyTolerantLoss(PyLossFunction):
+    """
+    Loss function that maps to approximately zero cost in a range around the
+    origin, and reverts to linear in error (quadratic in cost) beyond this
+    range. The tolerance parameter 'a' sets the nominal point at which the
+    transition occurs, and the transition size parameter 'b' sets the nominal
+    distance over which most of the transition occurs. Both a and b must be
+    greater than zero, and typically b will be set to a fraction of a. The
+    slope rho'[s] varies smoothly from about 0 at s <= a - b to about 1 at s >=
+    a + b.
+    The term is computed as:
+      rho(s) = b log(1 + exp((s - a) / b)) - c0.
+    where c0 is chosen so that rho(0) == 0
+      c0 = b log(1 + exp(-a / b)
+    This has the following useful properties:
+      rho(s) == 0               for s = 0
+      rho'(s) ~= 0              for s << a - b
+      rho'(s) ~= 1              for s >> a + b
+      rho''(s) > 0              for all s
+    In addition, all derivatives are continuous, and the curvature is
+    concentrated in the range a - b to a + b.
+    At s = 0: rho = [0, ~0, ~0].
+    """
+    def __init__(self, double _a, double _b):
+        self._loss_function =  new ceres_static.TolerantLoss(_a, _b)
+cdef class PyComposedLoss(PyLossFunction):
+    def __init__(self, PyLossFunction f, PyLossFunction g):
+        self._loss_function =  new ceres_static.ComposedLoss(f._loss_function,
+                                                     ceres_static.DO_NOT_TAKE_OWNERSHIP,
+                                                     g._loss_function,
+                                                     ceres_static.DO_NOT_TAKE_OWNERSHIP)
+cdef class PyScaledLoss(PyLossFunction):
+    def __cinit__(self, PyLossFunction loss_function, double _a):
+        self._loss_function =  new ceres_static.ScaledLoss(loss_function._loss_function,
+                                                   _a,
+                                                   ceres_static.DO_NOT_TAKE_OWNERSHIP)
+    def __dealloc__(self):
+        del self._loss_function
+cdef class PySolverSummary:
+    cdef ceres_static.SolverSummary _summary
+    def briefReport(self):
+        return self._summary.BriefReport()
+    def fullReport(self):
+        return self._summary.FullReport()
+    # def get_ter_type(self):
+    #     return self._summary.termination_type
+    property termination_type:
+        def __get__(self):
+            return self._summary.termination_type
+        def __set__(self, value):
+            self._summary.termination_type = value
+    property final_cost:
+        def __get__(self):
+            return self._summary.final_cost
+cdef class PyProblem:
+    cdef ceres_static.Problem _problem
+    def __cinit__(self):
+        pass
+    # loss_function=NULL yields squared loss
+    cpdef add_residual_block(self,
+                             PyResidual cost_function, # chana
+                             PyLossFunction loss_function,
+                             parameter_blocks=[]):
+        cdef np.ndarray _tmp_array
+        cdef vector[double*] _parameter_blocks
+        cdef double f
+        cdef ceres_static.ResidualBlockId _block_id
+        for parameter_block in parameter_blocks:
+            _tmp_array = np.ascontiguousarray(parameter_block, dtype=np.double)
+            _parameter_blocks.push_back(<double*> _tmp_array.data)
+        _block_id = self._problem.AddResidualBlock(cost_function._residual_cost_function,
+                                                   loss_function._loss_function,
+                                                   _parameter_blocks)
+        block_id = PyResidualBlockId()
+        block_id._block_id = _block_id
+        return block_id
+    cpdef evaluate(self, residual_blocks, apply_loss_function=True):
+        cdef double cost
+        options = PyEvaluateOptions()
+        options.apply_loss_function = apply_loss_function
+        options.residual_blocks = residual_blocks
+        self._problem.Evaluate(options._options, &cost, NULL, NULL, NULL)
+        return cost
+    cpdef set_parameter_block_constant(self, block):
+        cdef np.ndarray _tmp_array = np.ascontiguousarray(block, dtype=np.double)
+        cdef double* _values = <double*> _tmp_array.data
+        self._problem.SetParameterBlockConstant(_values)
+    cpdef set_parameter_block_variable(self, block):
+        cdef np.ndarray _tmp_array = np.ascontiguousarray(block, dtype=np.double)
+        cdef double* _values = <double*> _tmp_array.data
+        self._problem.SetParameterBlockVariable(_values)
+    cpdef set_parameter_lower_bound(self, values, index, lower_bound):
+        cdef np.ndarray _tmp_array = np.ascontiguousarray(values, dtype=np.double)
+        cdef double* _values = <double*> _tmp_array.data
+        self._problem.SetParameterLowerBound(_values, index, lower_bound)
+    cpdef set_parameter_upper_bound(self, values, index, upper_bound):
+        cdef np.ndarray _tmp_array = np.ascontiguousarray(values, dtype=np.double)
+        cdef double* _values = <double*> _tmp_array.data
+        self._problem.SetParameterUpperBound(_values, index, upper_bound)
+def solve(PySolverOptions options, PyProblem problem, PySolverSummary summary):
+    ceres_static.Solve(drf(options._options), &problem._problem, &summary._summary)
+cdef class PyResidualBlockId:
+    cdef ceres_static.ResidualBlockId _block_id
+cdef class PyEvaluateOptions:
+    cdef ceres_static.EvaluateOptions _options
+    def __cinit__(self):
+        pass
+    def __init__(self):
+        self._options = ceres_static.EvaluateOptions()
+    property residual_blocks:
+        def __get__(self):
+            blocks = []
+            cdef int i
+            for i in range(self._options.residual_blocks.size()):
+                block = PyResidualBlockId()
+                block._block_id = self._options.residual_blocks[i]
+                blocks.append(block)
+            return blocks
+        def __set__(self, blocks):
+            self._options.residual_blocks.clear()
+            cdef PyResidualBlockId block
+            for block in blocks:
+                self._options.residual_blocks.push_back(block._block_id)
+    property apply_loss_function:
+        def __get__(self):
+            return self._options.apply_loss_function
+        def __set__(self, value):
+            self._options.apply_loss_function = value
+
+class RunIterationCallbackFunc:
+    def __init__(self, func2run):
+        self.func = func2run
+    def in_func2run(self, iteration_summary=None):
+        return self.func(iteration_summary)
+
+
+cdef class PySolverOptions:
+    cdef ceres_static.SolverOptions* _options
+    cdef ceres_static.PyIterationCallbackWrapper wrapper
+
+    def __cinit__(self):
+        pass
+    def __init__(self):
+        self._options = new ceres_static.SolverOptions() 
+        cdef vector[ceres_static.IterationCallback*] callbacks
+        self._options.callbacks = callbacks
+        
+    def set_callbacks(self, func2run):
+        in_class = RunIterationCallbackFunc(func2run) # chana
+        self.wrapper = ceres_static.PyIterationCallbackWrapper(in_class.in_func2run)
+        cdef vector[ceres_static.IterationCallback*] callbacks
+        callbacks.push_back(<ceres_static.IterationCallback*>&self.wrapper)
+        self._options.callbacks = callbacks
+
+    property max_num_iterations:
+        def __get__(self):
+            return self._options.max_num_iterations
+        def __set__(self, value):
+            self._options.max_num_iterations = value
+    property minimizer_progress_to_stdout:
+        def __get__(self):
+            return self._options.minimizer_progress_to_stdout
+        def __set__(self, value):
+            self._options.minimizer_progress_to_stdout = value
+    property linear_solver_type:
+        def __get__(self):
+            return self._options.linear_solver_type
+        def __set__(self, value):
+            self._options.linear_solver_type = value
+    property trust_region_strategy_type:
+        def __get__(self):
+            return self._options.trust_region_strategy_type
+        def __set__(self, value):
+            new_val = str_to_enum_str(value)
+            int_val = 0
+            if new_val not in TrustRegionStrategyType.reverse_mapping.values():
+                raise Exception("no such trust region strategy type")
+            for key, str_val in TrustRegionStrategyType.reverse_mapping.items():
+                if str_val == new_val:
+                    int_val = key
+            self._options.trust_region_strategy_type = int_val
+    property dogleg_type:
+        def __get__(self):
+            return self._options.dogleg_type
+        def __set__(self, value):
+            self._options.dogleg_type = value
+    property preconditioner_type:
+        def __get__(self):
+            return self._options.preconditioner_type
+        def __set__(self, value):
+            self._options.preconditioner_type = value
+    property num_threads:
+        def __get__(self):
+            return self._options.num_threads
+        def __set__(self, value):
+            self._options.num_threads = value
+    property use_nonmonotonic_steps:
+        def __get__(self):
+            return self._options.use_nonmonotonic_steps
+        def __set__(self, value):
+            self._options.use_nonmonotonic_steps = value
+    property function_tolerance:
+        def __get__(self):
+            return self._options.function_tolerance
+        def __set__(self, value):
+            self._options.function_tolerance = value
+    property update_state_every_iteration:
+        def __get__(self):
+            return self._options.update_state_every_iteration
+        def __set__(self, value):
+            self._options.update_state_every_iteration = value
+    property gradient_tolerance:
+        def __get__(self):
+            return self._options.gradient_tolerance
+        def __set__(self, value):
+            self._options.gradient_tolerance = value
+    property use_inner_iterations:
+        def __get__(self):
+            return self._options.use_inner_iterations
+        def __set__(self, value):
+            self._options.use_inner_iterations = value
+    property minimizer_type:
+        def __get__(self):
+            return self._options.minimizer_type
+        def __set__(self, value):
+            new_val = str_to_enum_str(value)
+            int_val = 0
+            if new_val not in MinimizerType.reverse_mapping.values():
+                raise Exception("no such minimizer type")
+            for key, str_val in MinimizerType.reverse_mapping.items():
+                if str_val == new_val:
+                    int_val = key
+            self._options.minimizer_type = int_val
+    property line_search_direction_type:
+        def __get__(self):
+            return self._options.line_search_direction_type
+        def __set__(self, value):
+            new_val = str_to_enum_str(value)
+            int_val = 0
+            if new_val not in LineSearchDirectionType.reverse_mapping.values():
+                raise Exception("line search direction type")
+            for key, str_val in LineSearchDirectionType.reverse_mapping.items():
+                if str_val == new_val:
+                    int_val = key
+            self._options.line_search_direction_type = int_val
+    property nonlinear_conjugate_gradient_type:
+        def __get__(self):
+            return self._options.nonlinear_conjugate_gradient_type
+        def __set__(self, value):
+            new_val = str_to_enum_str(value)
+            int_val = 0
+            if new_val not in NonlinearConjugateGradientType.reverse_mapping.values():
+                raise Exception("no such nonlinear conjugate gradient type")
+            for key, str_val in NonlinearConjugateGradientType.reverse_mapping.items():
+                if str_val == new_val:
+                    int_val = key
+            self._options.nonlinear_conjugate_gradient_type = int_val
+    property line_search_type:
+        def __get__(self):
+            return self._options.line_search_type
+        def __set__(self, value):
+            new_val = str_to_enum_str(value)
+            int_val = 0
+            if new_val not in LineSearchType.reverse_mapping.values():
+                raise Exception("no such line search type")
+            for key, str_val in LineSearchType.reverse_mapping.items():
+                if str_val == new_val:
+                    int_val = key
+            self._options.line_search_type = int_val
+
+#
+def str_to_enum_str(value):
+    val_up = value.upper()
+    val_rep1 = val_up.replace("-", "_")
+    val_rep2 = val_rep1.replace(" ", "_")
     return val_rep2
```

## dplus_ceres/iteration_callback_func.pyx

 * *Ordering differences only*

```diff
@@ -1,25 +1,25 @@
-import cython
-from libc.stdio cimport printf #printf for debugging
-from libcpp cimport int
-from libcpp.string cimport string
-
-# although we dont use these imports, without them this file doesnt compile
-import numpy as np
-cimport numpy as np
-
-from enum import Enum
-def enum(*sequential, **named):
-    enums = dict(zip(sequential, range(len(sequential))), **named)
-    reverse = dict((value, key) for key, value in enums.iteritems())
-    enums['reverse_mapping'] = reverse
-    return type('Enum', (), enums)
-
-CallbackReturnType = enum("SOLVER_CONTINUE", "SOLVER_ABORT", "SOLVER_TERMINATE_SUCCESSFULLY")
-
-
-cdef public int call_iteration_function(obj) :
-    # for some unknown reason you can't use numpy here ( cdef double[:] view fail, np_x.data fail)
-    # however we must convert c types to python types. so we will create python lists that contain the values
-    cdef int CallbackReturnType_int
-    CallbackReturnType_int = obj()
+import cython
+from libc.stdio cimport printf #printf for debugging
+from libcpp cimport int
+from libcpp.string cimport string
+
+# although we dont use these imports, without them this file doesnt compile
+import numpy as np
+cimport numpy as np
+
+from enum import Enum
+def enum(*sequential, **named):
+    enums = dict(zip(sequential, range(len(sequential))), **named)
+    reverse = dict((value, key) for key, value in enums.iteritems())
+    enums['reverse_mapping'] = reverse
+    return type('Enum', (), enums)
+
+CallbackReturnType = enum("SOLVER_CONTINUE", "SOLVER_ABORT", "SOLVER_TERMINATE_SUCCESSFULLY")
+
+
+cdef public int call_iteration_function(obj) :
+    # for some unknown reason you can't use numpy here ( cdef double[:] view fail, np_x.data fail)
+    # however we must convert c types to python types. so we will create python lists that contain the values
+    cdef int CallbackReturnType_int
+    CallbackReturnType_int = obj()
     return CallbackReturnType_int
```

## Comparing `dplus_ceres-0.4.0.dist-info/LICENSE` & `dplus_ceres-0.5.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-pyceres:
-
-MIT License
-
-Copyright (c) 2021 research-software-company
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-cyres package code (https://github.com/rll/cyres) used, with license reproduced below:
-
-Copyright (c) 2013, Berkeley RLL
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
-
-  Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-  Redistributions in binary form must reproduce the above copyright notice, this
-  list of conditions and the following disclaimer in the documentation and/or
-  other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-ceres solver code:
-Ceres Solver is licensed under the New BSD license, whose terms are as follows.
-
-Copyright 2016 Google Inc. All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
-
-Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
-
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-
-Neither the name of Google Inc., nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
-
+pyceres:
+
+MIT License
+
+Copyright (c) 2021 research-software-company
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+cyres package code (https://github.com/rll/cyres) used, with license reproduced below:
+
+Copyright (c) 2013, Berkeley RLL
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+  Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+  Redistributions in binary form must reproduce the above copyright notice, this
+  list of conditions and the following disclaimer in the documentation and/or
+  other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+ceres solver code:
+Ceres Solver is licensed under the New BSD license, whose terms are as follows.
+
+Copyright 2016 Google Inc. All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+Neither the name of Google Inc., nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+
 This software is provided by the copyright holders and contributors “AS IS” and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. In no event shall Google Inc. be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
```

## Comparing `dplus_ceres-0.4.0.dist-info/METADATA` & `dplus_ceres-0.5.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dplus-ceres
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python wrapper of Ceres 2.0 - for DPlus
 Home-page: http://www.researchsoftware.co.il
 Author: Devora Witty
 Author-email: devora@researchsoftware.co.il
 License: pyceres:
         
         MIT License
@@ -66,24 +66,21 @@
         Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
         
         Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
         
         Neither the name of Google Inc., nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         
         This software is provided by the copyright holders and contributors “AS IS” and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. In no event shall Google Inc. be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: numpy (<1.24,>=1.23.0)
-
-UNKNOWN
+Requires-Dist: numpy (>=1.23.0)
```

