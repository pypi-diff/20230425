# Comparing `tmp/sciqlopplots-0.2.6.tar.gz` & `tmp/sciqlopplots-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciqlopplots-0.2.6.tar", last modified: Tue Apr 18 15:47:29 2023, max compression
+gzip compressed data, was "sciqlopplots-0.3.3.tar", last modified: Tue Apr 25 08:27:59 2023, max compression
```

## Comparing `sciqlopplots-0.2.6.tar` & `sciqlopplots-0.3.3.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.clang-format
--rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.github/workflows/pythonpublish-linux.yml
--rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.github/workflows/pythonpublish-osx.yml
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.github/workflows/pythonpublish-win.yml
--rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.gitignore
--rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/COPYING
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/README.md
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/__init__.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/_QCustomPlot.hpp
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/bindings.h
--rw-r--r--   0        0        0    16781 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/bindings.xml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
--rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
--rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/src_list.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/snippets.cpp
--rw-r--r--   0        0        0     4717 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/meson.build
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopColorMap.hpp
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopGraph.hpp
--rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopPlot.hpp
--rw-r--r--   0        0        0     2362 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopPlotItem.hpp
--rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopVerticalSpan.hpp
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/constants.hpp
--rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/numpy_wrappers.hpp
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/meson.build
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/meson_options.txt
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/pyproject.toml
--rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/qcustomplot-source/GPL.txt
--rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/qcustomplot-source/changelog.txt
--rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/qcustomplot-source/qcustomplot.cpp
--rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/qcustomplot-source/qcustomplot.h
--rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/setup.cfg
--rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopColorMap.cpp
--rw-r--r--   0        0        0     5982 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopGraph.cpp
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopPlot.cpp
--rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopPlotItem.cpp
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopVerticalSpan.cpp
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/numpy_wrappers.cpp
--rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/subprojects/cpp_utils.wrap
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/subprojects/hedley.wrap
--rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/QCP_Examples/plots/main.py
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/SciQLopColorMap/main.py
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/SciQLopGraph/main.py
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/SciQLopVerticalSpan/main.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/StackedGraphs/main.py
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/meson.build
--rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/meson.build
--rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.clang-format
+-rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.github/workflows/pythonpublish-linux.yml
+-rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.github/workflows/pythonpublish-osx.yml
+-rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.github/workflows/pythonpublish-win.yml
+-rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/COPYING
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/README.md
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/__init__.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/_QCustomPlot.hpp
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/bindings.h
+-rw-r--r--   0        0        0    17049 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/bindings.xml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
+-rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
+-rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/src_list.py
+-rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/bindings/snippets.cpp
+-rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/SciQLopPlots/meson.build
+-rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopColorMap.hpp
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopColorMapResampler.hpp
+-rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopGraph.hpp
+-rw-r--r--   0        0        0     5992 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopGraphResampler.hpp
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopPlot.hpp
+-rw-r--r--   0        0        0     2362 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopPlotItem.hpp
+-rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopVerticalSpan.hpp
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/constants.hpp
+-rw-r--r--   0        0        0     6070 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/include/SciQLopPlots/numpy_wrappers.hpp
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/meson.build
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/meson_options.txt
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/pyproject.toml
+-rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/qcustomplot-source/GPL.txt
+-rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/qcustomplot-source/changelog.txt
+-rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/qcustomplot-source/qcustomplot.cpp
+-rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/qcustomplot-source/qcustomplot.h
+-rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/setup.cfg
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopColorMap.cpp
+-rw-r--r--   0        0        0     5102 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopGraph.cpp
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopPlot.cpp
+-rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopPlotItem.cpp
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/SciQLopVerticalSpan.cpp
+-rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/src/numpy_wrappers.cpp
+-rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/subprojects/cpp_utils.wrap
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/subprojects/hedley.wrap
+-rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/QCP_Examples/plots/main.py
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/SciQLopColorMap/main.py
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/SciQLopGraph/main.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/SciQLopVerticalSpan/main.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/StackedGraphs/main.py
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/manual-tests/meson.build
+-rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/tests/meson.build
+-rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.3.3/PKG-INFO
```

### Comparing `sciqlopplots-0.2.6/.clang-format` & `sciqlopplots-0.3.3/.clang-format`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/.github/workflows/pythonpublish-linux.yml` & `sciqlopplots-0.3.3/.github/workflows/pythonpublish-linux.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       - uses: actions/checkout@v3
         with:
           submodules: true
       - name: Build for Python ${{ matrix.python-version }}
         run: |
             dnf install -y /usr/lib64/libxkbcommon.so.0 /usr/lib64/libxslt.so.1 /usr/bin/llvm-config clang
             git config --global --add safe.directory '*'
-            python -m pip install --upgrade "pip" "meson" "ninja" "numpy" "meson-python" "build" "wheel" "twine" "auditwheel" "aqtinstall"
+            python -m pip install --upgrade "pip" "meson" "ninja" "numpy" "meson-python==0.12.1" "build" "wheel" "twine" "auditwheel" "aqtinstall"
             python -m pip install "PySide6==6.4.3"
             python -m pip install \
                 --index-url=http://download.qt.io/official_releases/QtForPython/ \
                 --trusted-host download.qt.io \
                 "shiboken6_generator==6.4.3"
             aqt install-qt -O /Qt linux desktop 6.4.3
             LD_LIBRARY_PATH=/Qt/6.4.3/gcc_64/lib python3 -m build --no-isolation  .
```

### Comparing `sciqlopplots-0.2.6/.github/workflows/pythonpublish-osx.yml` & `sciqlopplots-0.3.3/.github/workflows/pythonpublish-osx.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           python-version: ${{ matrix.python-version }}
           architecture: x64
       - name: add qt dir to path
         run: |
             echo "$GITHUB_WORKSPACE/Qt/6.4.3/macos/bin" >> $GITHUB_PATH
       - run: |
           brew install rename
-          pip install --upgrade "meson" "ninja" "numpy" "meson-python" "build" "wheel" "twine" "aqtinstall"
+          pip install --upgrade "meson" "ninja" "numpy" "meson-python==0.12.1" "build" "wheel" "twine" "aqtinstall"
           pip install "PySide6==6.4.3"
           pip install \
               --index-url=http://download.qt.io/official_releases/QtForPython/ \
               --trusted-host download.qt.io "shiboken6_generator==6.4.3"
           aqt install-qt -O $GITHUB_WORKSPACE/Qt mac desktop 6.4.3
           python3 -m build --no-isolation .
           #rename 's/macosx_10_15_[0-9]_x86_64/macosx_10_15_x86_64/g' dist/*.whl
```

### Comparing `sciqlopplots-0.2.6/.github/workflows/pythonpublish-win.yml` & `sciqlopplots-0.3.3/.github/workflows/pythonpublish-win.yml`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64 
       - name: Install deps and build package
         env:
           CLANG_INSTALL_DIR: C:\Program Files\LLVM\
         run: |
-          pip install --upgrade "meson" "ninja" "numpy" "meson-python" "build" "wheel" "twine" "auditwheel" "aqtinstall"
+          pip install --upgrade "meson" "ninja" "numpy" "meson-python==0.12.1" "build" "wheel" "twine" "auditwheel" "aqtinstall"
           pip install "PySide6==6.4.3"
           pip install --index-url=http://download.qt.io/official_releases/QtForPython/ --trusted-host download.qt.io "shiboken6_generator==6.4.3"
           aqt install-qt -O $env:GITHUB_WORKSPACE\Qt windows desktop 6.4.3 win64_mingw
           python3 -m build --no-isolation  .
 
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
```

### Comparing `sciqlopplots-0.2.6/COPYING` & `sciqlopplots-0.3.3/COPYING`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build` & `sciqlopplots-0.3.3/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/SciQLopPlots/bindings/_QCustomPlot.hpp` & `sciqlopplots-0.3.3/SciQLopPlots/bindings/_QCustomPlot.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/SciQLopPlots/bindings/bindings.xml` & `sciqlopplots-0.3.3/SciQLopPlots/bindings/bindings.xml`

 * *Files 1% similar despite different names*

#### Comparing `sciqlopplots-0.2.6/SciQLopPlots/bindings/bindings.xml` & `sciqlopplots-0.3.3/SciQLopPlots/bindings/bindings.xml`

```diff
@@ -69,14 +69,19 @@
       </modify-argument>
     </modify-function>
     <modify-function signature="addSciQLopGraph(QCPAxis*, QCPAxis*, QStringList, SciQLopGraph::DataOrder)">
       <modify-argument index="return">
         <define-ownership class="target" owner="target"/>
       </modify-argument>
     </modify-function>
+    <modify-function signature="addSciQLopGraph(QCPAxis*, QCPAxis*, SciQLopGraph::DataOrder)">
+      <modify-argument index="return">
+        <define-ownership class="target" owner="target"/>
+      </modify-argument>
+    </modify-function>
     <modify-function signature="addSciQLopColorMap(QCPAxis*, QCPAxis*, const QString&amp;, SciQLopGraph::DataOrder)">
       <modify-argument index="return">
         <define-ownership class="target" owner="target"/>
       </modify-argument>
     </modify-function>
   </object-type>
   <object-type name="QCPPainter" generate="yes"/>
```

### Comparing `sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/rpath-helper.py` & `sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/rpath-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py` & `sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py` & `sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/src_list.py` & `sciqlopplots-0.3.3/SciQLopPlots/bindings/helper_scripts/src_list.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/SciQLopPlots/bindings/snippets.cpp` & `sciqlopplots-0.3.3/SciQLopPlots/bindings/snippets.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 // @snippet QCPColorMapData-coordToCell
 
 // @snippet SciQLopGraph-setData
 %CPPSELF.setData(NpArray_view{pyArgs[0]}, NpArray_view{pyArgs[1]});
 // @snippet SciQLopGraph-setData
 
 // @snippet SciQLopColorMap-setData
+Py_BEGIN_ALLOW_THREADS
 %CPPSELF.setData(NpArray_view{pyArgs[0]}, NpArray_view{pyArgs[1]}, NpArray_view{pyArgs[2]});
+Py_END_ALLOW_THREADS
 // @snippet SciQLopColorMap-setData
 
 // @snippet QCPAxis-setTicker
 %CPPSELF.setTicker( QSharedPointer<QCPAxisTicker>(%1) );
 // @snippet QCPAxis-setTicker
 
 // @snippet QCPAxis-removeTicker
```

### Comparing `sciqlopplots-0.2.6/SciQLopPlots/meson.build` & `sciqlopplots-0.3.3/SciQLopPlots/meson.build`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 moc_headers = [
     'bindings/_QCustomPlot.hpp',
     project_source_root+'/include/SciQLopPlots/SciQLopGraph.hpp',
     project_source_root+'/include/SciQLopPlots/SciQLopColorMap.hpp',
     project_source_root+'/include/SciQLopPlots/SciQLopVerticalSpan.hpp',
     project_source_root+'/include/SciQLopPlots/SciQLopPlotItem.hpp',
     project_source_root+'/include/SciQLopPlots/SciQLopPlot.hpp',
+    project_source_root+'/include/SciQLopPlots/SciQLopGraphResampler.hpp',
+    project_source_root+'/include/SciQLopPlots/SciQLopColorMapResampler.hpp',
     project_source_root+'/qcustomplot-source/qcustomplot.h'
 ]
 
 moc_sources = []
 headers = moc_headers + \
          [project_source_root+'/include/SciQLopPlots/numpy_wrappers.hpp',
          project_source_root+'/include/SciQLopPlots/constants.hpp']
```

### Comparing `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopColorMap.hpp` & `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopColorMap.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -21,42 +21,44 @@
 ----------------------------------------------------------------------------*/
 #pragma once
 #include "numpy_wrappers.hpp"
 
 #include <QMutex>
 #include <qcustomplot.h>
 
+struct ColormapResampler;
+class QThread;
+
 class SciQLopColorMap : public QObject
 {
-    NpArray_view _x;
-    NpArray_view _y;
-    NpArray_view _z;
+    ColormapResampler* _resampler = nullptr;
+    QThread* _resampler_thread = nullptr;
+
     QCPRange _data_x_range;
     QCPAxis* _keyAxis;
     QCPAxis* _valueAxis;
     QCPColorMap* _cmap;
     QMutex _data_swap_mutex;
     Q_OBJECT
     inline QCustomPlot* _plot() const { return qobject_cast<QCustomPlot*>(this->parent()); }
 
 
     void _range_changed(const QCPRange& newRange, const QCPRange& oldRange);
     void _resample(const QCPRange& newRange);
-    void _setDataLinear();
-    void _setDataLog();
+    void _cmap_got_destroyed();
 
 public:
     enum class DataOrder
     {
         xFirst,
         yFirst
     };
     Q_ENUMS(FractionStyle)
-    explicit SciQLopColorMap(QCustomPlot* parent, QCPAxis* keyAxis, QCPAxis* valueAxis,const QString& name,
-        DataOrder dataOrder = DataOrder::xFirst);
+    explicit SciQLopColorMap(QCustomPlot* parent, QCPAxis* keyAxis, QCPAxis* valueAxis,
+        const QString& name, DataOrder dataOrder = DataOrder::xFirst);
     virtual ~SciQLopColorMap() override;
 
     void setData(NpArray_view&& x, NpArray_view&& y, NpArray_view&& z);
     inline QCPColorMap* colorMap() const { return _cmap; }
 
     Q_SIGNAL void range_changed(const QCPRange& newRange, bool missData);
```

### Comparing `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopGraph.hpp` & `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopGraph.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -18,59 +18,62 @@
 -------------------------------------------------------------------------------*/
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
 #pragma once
 
 #include "numpy_wrappers.hpp"
-#include <QMutex>
 #include <qcustomplot.h>
+struct GraphResampler;
+class QThread;
 
 class SciQLopGraph : public QObject
 {
-    NpArray_view _x;
-    NpArray_view _y;
-    QCPRange _data_x_range;
+    GraphResampler* _resampler = nullptr;
+    QThread* _resampler_thread = nullptr;
+
     QCPAxis* _keyAxis;
     QCPAxis* _valueAxis;
     QList<QCPGraph*> _graphs;
-    QMutex _data_swap_mutex;
+
     Q_OBJECT
-    inline QCustomPlot* _plot() const { return qobject_cast<QCustomPlot*>(this->parent()); }
 
-    inline void _create_graphs(QStringList labels)
-    {
-        for (const auto& label : labels)
-        {
-            _graphs.append(_plot()->addGraph(_keyAxis, _valueAxis));
-            _graphs.back()->setName(label);
-            _graphs.back()->setAdaptiveSampling(true);
-        }
-    }
+    inline QCustomPlot* _plot() const { return qobject_cast<QCustomPlot*>(this->parent()); }
 
 
     void _range_changed(const QCPRange& newRange, const QCPRange& oldRange);
-    void _resample(const QCPRange& newRange);
 
     void _setGraphData(std::size_t index, QVector<QCPGraphData> data);
 
     Q_SIGNAL void _setGraphDataSig(std::size_t index, QVector<QCPGraphData> data);
 
+    void clear_graphs(bool graph_already_removed = false);
+    void clear_resampler();
+    void create_resampler(const QStringList &labels);
+    void graph_got_removed_from_plot(QCPGraph* graph);
+
 public:
     enum class DataOrder
     {
         xFirst,
         yFirst
     };
     Q_ENUMS(FractionStyle)
     explicit SciQLopGraph(QCustomPlot* parent, QCPAxis* keyAxis, QCPAxis* valueAxis,
-        QStringList labels, DataOrder dataOrder = DataOrder::xFirst);
+        const QStringList& labels, DataOrder dataOrder = DataOrder::xFirst);
+
+    explicit SciQLopGraph(QCustomPlot* parent, QCPAxis* keyAxis, QCPAxis* valueAxis,
+        DataOrder dataOrder = DataOrder::xFirst);
+
     virtual ~SciQLopGraph() override;
 
     void setData(NpArray_view&& x, NpArray_view&& y, bool ignoreCurrentRange = false);
     inline QCPGraph* graphAt(std::size_t index) const { return _graphs[index]; }
+    void create_graphs(const QStringList& labels);
+
+    inline std::size_t line_count() { return std::size(this->_graphs); }
 
     Q_SIGNAL void range_changed(const QCPRange& newRange, bool missData);
 
 private:
     DataOrder _dataOrder = DataOrder::xFirst;
 };
```

### Comparing `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopPlot.hpp` & `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopPlot.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,22 @@
 
     inline SciQLopGraph* addSciQLopGraph(QCPAxis* x, QCPAxis* y, QStringList labels,
         SciQLopGraph::DataOrder dataOrder = SciQLopGraph::DataOrder::xFirst)
     {
         auto sg = new SciQLopGraph(this, x, y, labels, dataOrder);
         return sg;
     }
+
+    inline SciQLopGraph* addSciQLopGraph(
+        QCPAxis* x, QCPAxis* y, SciQLopGraph::DataOrder dataOrder = SciQLopGraph::DataOrder::xFirst)
+    {
+        auto sg = new SciQLopGraph(this, x, y, dataOrder);
+        return sg;
+    }
+
     inline SciQLopColorMap* addSciQLopColorMap(QCPAxis* x, QCPAxis* y, const QString& name,
         SciQLopColorMap::DataOrder dataOrder = SciQLopColorMap::DataOrder::xFirst)
     {
         auto sg = new SciQLopColorMap(this, x, y, name, dataOrder);
         return sg;
     }
```

### Comparing `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopPlotItem.hpp` & `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopPlotItem.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopVerticalSpan.hpp` & `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopVerticalSpan.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/include/SciQLopPlots/constants.hpp` & `sciqlopplots-0.3.3/include/SciQLopPlots/constants.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/include/SciQLopPlots/numpy_wrappers.hpp` & `sciqlopplots-0.3.3/include/SciQLopPlots/numpy_wrappers.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,25 @@
 
 
 template <typename dest_type = PyObject>
 struct PyObjectWrapper
 {
 private:
     PyObject* _py_obj = nullptr;
-    void inc_refcount() { Py_XINCREF(_py_obj); }
+    void inc_refcount()
+    {
+        PyGILState_STATE state = PyGILState_Ensure();
+        Py_XINCREF(_py_obj);
+        PyGILState_Release(state);
+    }
     void dec_refcount()
     {
+        PyGILState_STATE state = PyGILState_Ensure();
         Py_XDECREF(_py_obj);
+        PyGILState_Release(state);
         _py_obj = nullptr;
     }
 
 public:
     PyObjectWrapper() : _py_obj { nullptr } { }
     PyObjectWrapper(const PyObjectWrapper& other) : _py_obj { other._py_obj } { inc_refcount(); }
     PyObjectWrapper(PyObjectWrapper&& other) : _py_obj { other._py_obj } { inc_refcount(); }
@@ -132,14 +139,18 @@
 
     inline PyObject* py_object() { return _py_obj.py_object(); }
 
     inline auto begin() noexcept { return data(); }
 
     inline auto end() noexcept { return data() + flat_size(); }
 
+    inline const auto begin() const noexcept { return data(); }
+
+    inline const auto end() const noexcept { return data() + flat_size(); }
+
     inline const auto cbegin() const noexcept { return data(); }
 
     inline const auto cend() const noexcept { return data() + flat_size(); }
 
     inline auto front() { return *begin(); }
     inline auto back() { return *(end() - 1); }
 };
```

### Comparing `sciqlopplots-0.2.6/meson.build` & `sciqlopplots-0.3.3/meson.build`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.2.6')
+project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.3.3')
 add_project_arguments(
             '-DCATCH_CONFIG_NO_POSIX_SIGNALS', # workaround for this https://github.com/catchorg/Catch2/issues/2192
             language: 'cpp',
             native: true
 )
 qt_sdk='qt6'
```

### Comparing `sciqlopplots-0.2.6/pyproject.toml` & `sciqlopplots-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/qcustomplot-source/GPL.txt` & `sciqlopplots-0.3.3/qcustomplot-source/GPL.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/qcustomplot-source/changelog.txt` & `sciqlopplots-0.3.3/qcustomplot-source/changelog.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/qcustomplot-source/qcustomplot.cpp` & `sciqlopplots-0.3.3/qcustomplot-source/qcustomplot.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/qcustomplot-source/qcustomplot.h` & `sciqlopplots-0.3.3/qcustomplot-source/qcustomplot.h`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/src/SciQLopColorMap.cpp` & `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopColorMapResampler.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -15,98 +15,149 @@
 -- You should have received a copy of the GNU General Public License
 -- along with this program; if not, write to the Free Software
 -- Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 -------------------------------------------------------------------------------*/
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
-#include "SciQLopPlots/SciQLopColorMap.hpp"
+#pragma once
+
+#include "numpy_wrappers.hpp"
+#include <QMutex>
 #include <cpp_utils/containers/algorithms.hpp>
+#include <qcustomplot.h>
 
-void SciQLopColorMap::_range_changed(const QCPRange& newRange, const QCPRange& oldRange) { }
 
-void SciQLopColorMap::_setDataLinear()
+struct ColormapResampler : public QObject
 {
-    if (std::size(_x) && std::size(_y) && std::size(_z))
+    Q_OBJECT
+    QMutex _mutex;
+    QMutex _range_mutex;
+    NpArray_view _x;
+    NpArray_view _y;
+    NpArray_view _z;
+    QCPRange _data_x_range;
+    std::size_t _line_cnt;
+    QCPAxis::ScaleType _scale_type;
+    QCPColorMapData* _last_data_ptr = nullptr;
+
+
+    inline QCPColorMapData* _setDataLinear(const NpArray_view& x, const NpArray_view& y,const  NpArray_view& z)
+    {
+
+            using namespace cpp_utils;
+            auto data = new QCPColorMapData(std::size(x), std::size(y),
+                { *containers::min(x), *containers::max(x) },
+                { *containers::min(y), *containers::max(y) });
+            auto it = std::cbegin(z);
+            for (const auto i : x)
+            {
+                for (const auto j : y)
+                {
+                    if (it != std::cend(z))
+                    {
+                        data->setData(i, j, *it);
+                        it++;
+                    }
+                }
+            }
+            return data;
+    }
+
+    inline QCPColorMapData* _setDataLog(const NpArray_view& x, const NpArray_view& y, const NpArray_view& z)
     {
         using namespace cpp_utils;
-        auto data = new QCPColorMapData(std::size(_x), std::size(_y),
-            { *containers::min(_x), *containers::max(_x) },
-            { *containers::min(_y), *containers::max(_y) });
-        auto it = std::cbegin(_z);
-        for (const auto i : _x)
+        auto data = new QCPColorMapData(std::size(x), std::size(y),
+            { *containers::min(x), *containers::max(x) },
+            { *containers::min(y), *containers::max(y) });
+        auto it = std::cbegin(z);
+        for (auto i = 0UL; i < std::size(x); i++)
         {
-            for (const auto j : _y)
+            for (auto j = 0UL; j < std::size(y); j++)
             {
-                if (it != std::cend(_z))
+                if (it != std::cend(z))
                 {
-                    data->setData(i, j, *it);
+                    data->setCell(i, j, *it);
                     it++;
                 }
             }
         }
-        this->_cmap->setData(data, false);
+        return data;
     }
-}
 
-void SciQLopColorMap::_setDataLog()
-{
-    using namespace cpp_utils;
-    auto data = new QCPColorMapData(std::size(_x), std::size(_y),
-        { *containers::min(_x), *containers::max(_x) },
-        { *containers::min(_y), *containers::max(_y) });
-    auto it = std::cbegin(_z);
-    for (auto i = 0UL; i < std::size(_x); i++)
+    Q_SIGNAL void _resample_sig(const QCPRange& newRange);
+    inline void _resample_slot(const QCPRange& newRange)
     {
-        for (auto j = 0UL; j < std::size(_y); j++)
         {
-            if (it != std::cend(_z))
+            QMutexLocker lock { &_range_mutex };
+            if (this->_data_x_range != newRange)
+                return;
+        }
+        _mutex.lock();
+        auto x = std::move(_x);
+        auto y = std::move(_y);
+        auto z = std::move(_z);
+        _mutex.unlock();
+        if (std::size(x) && std::size(y) && std::size(z))
+        {
+            if (this->_scale_type == QCPAxis::stLinear)
             {
-                data->setCell(i, j, *it);
-                it++;
+                emit this->refreshPlot(this->_setDataLinear(x,y,z));
             }
+            else
+            {
+                emit this->refreshPlot(this->_setDataLog(std::move(x), std::move(y), std::move(z)));
+            }
+        }
+        else
+        {
+            emit this->refreshPlot(new QCPColorMapData(0, 0, { 0., 0. }, { 0., 0. }));
         }
     }
-    this->_cmap->setData(data, false);
-}
 
-SciQLopColorMap::SciQLopColorMap(QCustomPlot* parent, QCPAxis* keyAxis, QCPAxis* valueAxis,
-    const QString& name, DataOrder dataOrder)
-        : QObject(parent), _keyAxis { keyAxis }, _valueAxis { valueAxis }, _dataOrder { dataOrder }
-{
-    this->_cmap = new QCPColorMap(keyAxis, valueAxis);
-    this->_cmap->setName(name);
-    connect(keyAxis, QOverload<const QCPRange&, const QCPRange&>::of(&QCPAxis::rangeChanged), this,
-        QOverload<const QCPRange&, const QCPRange&>::of(&SciQLopColorMap::_range_changed));
-}
+public:
+    Q_SIGNAL void setGraphData(std::size_t index, QVector<QCPGraphData> data);
+    Q_SIGNAL void refreshPlot(QCPColorMapData* data);
 
-SciQLopColorMap::~SciQLopColorMap()
-{
-    this->_plot()->removePlottable(this->colorMap());
-}
+    ColormapResampler(QCPAxis::ScaleType scale_type) : _scale_type { scale_type }
+    {
+        connect(this, &ColormapResampler::_resample_sig, this, &ColormapResampler::_resample_slot,
+            Qt::QueuedConnection);
+    }
 
-void SciQLopColorMap::setData(NpArray_view&& x, NpArray_view&& y, NpArray_view&& z)
-{
+    inline void resample(const QCPRange& newRange) { emit this->_resample_sig(newRange); }
+
+    inline QCPRange x_range()
     {
-        QMutexLocker locker(&_data_swap_mutex);
-        _x = std::move(x);
-        _y = std::move(y);
-        _z = std::move(z);
+        QMutexLocker locker(&_mutex);
+        return this->_data_x_range;
+    }
 
-        if (std::size(_x) && std::size(_y) && std::size(_z))
+    inline void setData(
+        NpArray_view&& x, NpArray_view&& y, NpArray_view&& z, QCPAxis::ScaleType scale_type)
+    {
+        const auto len = x.flat_size();
         {
-            if (this->_cmap->valueAxis()->scaleType() == QCPAxis::stLinear)
+            QMutexLocker range_lock { &_range_mutex };
+            if (len > 0)
             {
-                this->_setDataLinear();
+                _data_x_range.lower = x.data()[0];
+                _data_x_range.upper = x.data()[len - 1];
             }
             else
             {
-                this->_setDataLog();
+                _data_x_range.lower = std::nan("");
+                _data_x_range.upper = std::nan("");
             }
         }
-        else
         {
-            this->_cmap->setData(new QCPColorMapData(0, 0, { 0., 0. }, { 0., 0. }), false);
+            QMutexLocker data_locker(&_mutex);
+
+            _x = std::move(x);
+            _y = std::move(y);
+            _z = std::move(z);
+
+            _scale_type = scale_type;
         }
+        this->resample(_data_x_range);
     }
-    this->_plot()->replot(QCustomPlot::rpQueuedReplot);
-}
+};
```

### Comparing `sciqlopplots-0.2.6/src/SciQLopGraph.cpp` & `sciqlopplots-0.3.3/include/SciQLopPlots/SciQLopGraphResampler.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,20 @@
 -- You should have received a copy of the GNU General Public License
 -- along with this program; if not, write to the Free Software
 -- Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 -------------------------------------------------------------------------------*/
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
-#include "SciQLopPlots/SciQLopGraph.hpp"
+#pragma once
+
+#include "SciQLopGraph.hpp"
+#include "numpy_wrappers.hpp"
+#include <QMutex>
+#include <qcustomplot.h>
 
 
 template <std::size_t dest_size>
 static inline QVector<QCPGraphData> resample(
     const double* x, const double* y, std::size_t x_size, const int y_incr = 1)
 {
     static_assert(dest_size % 2 == 0);
@@ -63,98 +68,104 @@
     {
         data[i] = QCPGraphData { x[i], *current_y_it };
         current_y_it += y_incr;
     }
     return data;
 }
 
-void SciQLopGraph::_range_changed(const QCPRange& newRange, const QCPRange& oldRange)
-{
-
-    if (!(newRange.contains(_data_x_range.lower) && newRange.contains(_data_x_range.upper)
-            && oldRange.contains(_data_x_range.lower) && oldRange.contains(_data_x_range.upper)))
-        this->_resample(newRange);
-
-    if (!(_data_x_range.contains(newRange.lower) && _data_x_range.contains(newRange.upper)))
-        emit this->range_changed(newRange, true);
-    else
-        emit this->range_changed(newRange, false);
-}
 
-void SciQLopGraph::_resample(const QCPRange& newRange)
+struct GraphResampler : public QObject
 {
-    QMutexLocker locker(&_data_swap_mutex);
-    if (_x.data() != nullptr && _x.flat_size() > 0)
+    Q_OBJECT
+    QMutex _mutex;
+    NpArray_view _x;
+    NpArray_view _y;
+    SciQLopGraph::DataOrder _dataOrder;
+    QCPRange _data_x_range;
+    std::size_t _line_cnt;
+
+    Q_SIGNAL void _resample_sig(const QCPRange& newRange);
+    inline void _resample_slot(const QCPRange& newRange)
     {
-        const auto start_x
-            = std::upper_bound(_x.data(), _x.data() + _x.flat_size(), newRange.lower);
-        const auto end_x = std::lower_bound(_x.data(), _x.data() + _x.flat_size(), newRange.upper);
-        const auto x_window_size = end_x - start_x;
-        if (x_window_size > 0)
+        QMutexLocker locker(&_mutex);
+        if (_x.data() != nullptr && _x.flat_size() > 0)
         {
-            const auto line_cnt = static_cast<std::size_t>(std::size(_graphs));
-            const auto y_incr = (_dataOrder == DataOrder::xFirst) ? 1UL : line_cnt;
-            for (auto line_index = 0UL; line_index < line_cnt; line_index++)
+            const auto start_x
+                = std::upper_bound(_x.data(), _x.data() + _x.flat_size(), newRange.lower);
+            const auto end_x
+                = std::lower_bound(_x.data(), _x.data() + _x.flat_size(), newRange.upper);
+            const auto x_window_size = end_x - start_x;
+            if (x_window_size > 0)
             {
-                const auto start_y = _y.data() + y_incr * (start_x - _x.data())
-                    + (line_index * ((_dataOrder == DataOrder::xFirst) ? _x.flat_size() : 1));
-                if (x_window_size > 10000)
-                {
-                    emit this->_setGraphDataSig(
-                        line_index, resample<10000>(start_x, start_y, x_window_size, y_incr));
-                }
-                else
+                const auto y_incr
+                    = (_dataOrder == SciQLopGraph::DataOrder::xFirst) ? 1UL : _line_cnt;
+                for (auto line_index = 0UL; line_index < _line_cnt; line_index++)
                 {
-                    emit this->_setGraphDataSig(
-                        line_index, copy_data(start_x, start_y, x_window_size, y_incr));
+                    const auto start_y = _y.data() + y_incr * (start_x - _x.data())
+                        + (line_index
+                            * ((_dataOrder == SciQLopGraph::DataOrder::xFirst) ? _x.flat_size()
+                                                                               : 1));
+                    if (x_window_size > 10000)
+                    {
+                        emit this->setGraphData(
+                            line_index, ::resample<10000>(start_x, start_y, x_window_size, y_incr));
+                    }
+                    else
+                    {
+                        emit this->setGraphData(
+                            line_index, copy_data(start_x, start_y, x_window_size, y_incr));
+                    }
                 }
             }
+            emit this->refreshPlot();
         }
     }
-}
 
-void SciQLopGraph::_setGraphData(std::size_t index, QVector<QCPGraphData> data)
-{
-    _graphs[index]->data()->set(data, true);
-}
+public:
+    Q_SIGNAL void setGraphData(std::size_t index, QVector<QCPGraphData> data);
+    Q_SIGNAL void refreshPlot();
 
-SciQLopGraph::SciQLopGraph(QCustomPlot* parent, QCPAxis* keyAxis, QCPAxis* valueAxis,
-    QStringList labels, DataOrder dataOrder)
-        : QObject(parent), _keyAxis { keyAxis }, _valueAxis { valueAxis }, _dataOrder { dataOrder }
-{
-    this->_create_graphs(labels);
-    connect(keyAxis, QOverload<const QCPRange&, const QCPRange&>::of(&QCPAxis::rangeChanged), this,
-        QOverload<const QCPRange&, const QCPRange&>::of(&SciQLopGraph::_range_changed));
-    connect(this, &SciQLopGraph::_setGraphDataSig, this, &SciQLopGraph::_setGraphData,
-        Qt::QueuedConnection);
-}
-
-SciQLopGraph::~SciQLopGraph()
-{
-    for (auto graph : _graphs)
+    GraphResampler(SciQLopGraph::DataOrder dataOrder, std::size_t line_cnt)
+            : _dataOrder { dataOrder }, _line_cnt { line_cnt }
     {
-        this->_plot()->removeGraph(graph);
+
+        connect(this, &GraphResampler::_resample_sig, this, &GraphResampler::_resample_slot,
+            Qt::QueuedConnection);
     }
-}
 
-void SciQLopGraph::setData(NpArray_view&& x, NpArray_view&& y, bool ignoreCurrentRange)
-{
-    {
-        QMutexLocker locker(&_data_swap_mutex);
+    inline void resample(const QCPRange& newRange) { emit this->_resample_sig(newRange); }
 
-        _x = std::move(x);
-        _y = std::move(y);
+    inline QCPRange x_range()
+    {
+        QMutexLocker locker(&_mutex);
+        return this->_data_x_range;
     }
-    const auto len = _x.flat_size();
-    if (len > 0)
+
+    inline void set_line_count(std::size_t line_cnt)
     {
-        _data_x_range.lower = _x.data()[0];
-        _data_x_range.upper = _x.data()[len - 1];
+        QMutexLocker locker(&_mutex);
+        this->_line_cnt = line_cnt;
     }
-    else
+
+    inline void setData(NpArray_view&& x, NpArray_view&& y)
     {
-        _data_x_range.lower = std::nan("");
-        _data_x_range.upper = std::nan("");
+        {
+            QMutexLocker locker(&_mutex);
+
+            _x = std::move(x);
+            _y = std::move(y);
+
+            const auto len = _x.flat_size();
+            if (len > 0)
+            {
+                _data_x_range.lower = _x.data()[0];
+                _data_x_range.upper = _x.data()[len - 1];
+            }
+            else
+            {
+                _data_x_range.lower = std::nan("");
+                _data_x_range.upper = std::nan("");
+            }
+        }
+        this->resample(_data_x_range);
     }
-    this->_resample(_data_x_range);
-    this->_plot()->replot(QCustomPlot::rpQueuedReplot);
-}
+};
```

### Comparing `sciqlopplots-0.2.6/src/SciQLopPlot.cpp` & `sciqlopplots-0.3.3/src/SciQLopPlot.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/src/SciQLopPlotItem.cpp` & `sciqlopplots-0.3.3/src/SciQLopPlotItem.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/src/SciQLopVerticalSpan.cpp` & `sciqlopplots-0.3.3/src/SciQLopVerticalSpan.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/src/numpy_wrappers.cpp` & `sciqlopplots-0.3.3/src/numpy_wrappers.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/tests/manual-tests/QCP_Examples/plots/main.py` & `sciqlopplots-0.3.3/tests/manual-tests/QCP_Examples/plots/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/tests/manual-tests/SciQLopColorMap/main.py` & `sciqlopplots-0.3.3/tests/manual-tests/SciQLopColorMap/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/tests/manual-tests/SciQLopGraph/main.py` & `sciqlopplots-0.3.3/tests/manual-tests/SciQLopGraph/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/tests/manual-tests/SciQLopVerticalSpan/main.py` & `sciqlopplots-0.3.3/tests/manual-tests/SciQLopVerticalSpan/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/tests/manual-tests/StackedGraphs/main.py` & `sciqlopplots-0.3.3/tests/manual-tests/StackedGraphs/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/tests/manual-tests/meson.build` & `sciqlopplots-0.3.3/tests/manual-tests/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.6/PKG-INFO` & `sciqlopplots-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciqlopplots
-Version: 0.2.6
+Version: 0.3.3
 Summary: SciQLop plot API based on QCustomPlot
 Home-page: https://github.com/SciQLop/SciQLopPlots
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
```

