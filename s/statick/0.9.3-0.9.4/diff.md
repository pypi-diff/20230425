# Comparing `tmp/statick-0.9.3.tar.gz` & `tmp/statick-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statick-0.9.3.tar", last modified: Mon Jan 30 23:18:35 2023, max compression
+gzip compressed data, was "statick-0.9.4.tar", last modified: Tue Apr 25 02:32:41 2023, max compression
```

## Comparing `statick-0.9.3.tar` & `statick-0.9.4.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:18:35.537791 statick-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-01-30 23:18:11.000000 statick-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41517 2023-01-30 23:18:35.537791 statick-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40851 2023-01-30 23:18:11.000000 statick-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 23:18:35.537791 statick-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-01-30 23:18:11.000000 statick-0.9.3/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1583 2023-01-30 23:18:11.000000 statick-0.9.3/statick
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:18:35.521791 statick-0.9.3/statick.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41517 2023-01-30 23:18:35.000000 statick-0.9.3/statick.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-01-30 23:18:35.000000 statick-0.9.3/statick.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 23:18:35.000000 statick-0.9.3/statick.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-30 23:18:35.000000 statick-0.9.3/statick.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-30 23:18:35.000000 statick-0.9.3/statick.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:18:35.525791 statick-0.9.3/statick_tool/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugin_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:18:35.525791 statick-0.9.3/statick_tool/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:18:35.529791 statick-0.9.3/statick_tool/plugins/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/c_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/c_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/cmake_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/cmake_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/groovy_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/groovy_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/java_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/java_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/maven_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/maven_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/perl_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/perl_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/python_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/python_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/ros_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/ros_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/shell_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/shell_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/xml_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/xml_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/yaml_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/discovery/yaml_discovery_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:18:35.529791 statick-0.9.3/statick_tool/plugins/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/code_climate_reporting_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/code_climate_reporting_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/do_nothing_reporting_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/do_nothing_reporting_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/json_reporting_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/json_reporting_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/print_to_console_reporting_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/print_to_console_reporting_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/write_jenkins_warnings_ng_reporting_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/reporting/write_jenkins_warnings_ng_reporting_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:18:35.537791 statick-0.9.3/statick_tool/plugins/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/bandit_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/bandit_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/black_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/black_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/catkin_lint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/catkin_lint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/cccc_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/cccc_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/clang_format_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/clang_format_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/clang_format_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/clang_tidy_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/clang_tidy_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/cmakelint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/cmakelint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/cppcheck_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/cppcheck_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/cpplint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/cpplint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/do_nothing_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/do_nothing_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/docformatter_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/docformatter_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/flawfinder_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/flawfinder_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/groovylint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/groovylint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/isort_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/isort_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/lizard_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/lizard_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/make_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/make_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/mypy_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/mypy_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/perlcritic_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/perlcritic_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/pycodestyle_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/pycodestyle_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/pydocstyle_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/pydocstyle_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/pyflakes_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/pyflakes_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/pylint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/pylint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/ruff_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/ruff_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/shellcheck_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/shellcheck_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/spotbugs_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/spotbugs_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/uncrustify_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/uncrustify_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/xmllint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/xmllint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/yamllint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/plugins/tool/yamllint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/reporting_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:18:35.537791 statick-0.9.3/statick_tool/rsc/
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/.groovylintrc.json
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/CMakeLists.txt.in
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/_clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/cccc.opt
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/discovery_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/exceptions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/gauntlet_ignore.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:18:35.537791 statick-0.9.3/statick_tool/rsc/plugin_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/plugin_mapping/clang-tidy.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/plugin_mapping/code_climate.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/plugin_mapping/cppcheck.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/plugin_mapping/make.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/plugin_mapping/perlcritic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/plugin_mapping/spotbugs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/profile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/sei_cert.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/self_check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/spotbugs-security.xml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/ultimate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/rsc/uncrustify.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/statick.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-01-30 23:18:11.000000 statick-0.9.3/statick_tool/tool_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:32:41.049269 statick-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-25 02:32:18.000000 statick-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41773 2023-04-25 02:32:41.049269 statick-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    41107 2023-04-25 02:32:18.000000 statick-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 02:32:41.053269 statick-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-25 02:32:18.000000 statick-0.9.4/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1583 2023-04-25 02:32:18.000000 statick-0.9.4/statick
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:32:41.033269 statick-0.9.4/statick.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41773 2023-04-25 02:32:40.000000 statick-0.9.4/statick.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-25 02:32:41.000000 statick-0.9.4/statick.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:32:40.000000 statick-0.9.4/statick.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-25 02:32:40.000000 statick-0.9.4/statick.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 02:32:40.000000 statick-0.9.4/statick.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:32:41.033269 statick-0.9.4/statick_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugin_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:32:41.033269 statick-0.9.4/statick_tool/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:32:41.037269 statick-0.9.4/statick_tool/plugins/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/c_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/c_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/cmake_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/cmake_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/groovy_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/groovy_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/java_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/java_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/maven_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/maven_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/perl_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/perl_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/python_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/python_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/ros_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/ros_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/shell_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/shell_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/xml_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/xml_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/yaml_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/discovery/yaml_discovery_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:32:41.041269 statick-0.9.4/statick_tool/plugins/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/code_climate_reporting_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/code_climate_reporting_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/do_nothing_reporting_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/do_nothing_reporting_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/json_reporting_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/json_reporting_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/print_to_console_reporting_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/print_to_console_reporting_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/write_jenkins_warnings_ng_reporting_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/reporting/write_jenkins_warnings_ng_reporting_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:32:41.049269 statick-0.9.4/statick_tool/plugins/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/bandit_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/bandit_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/black_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/black_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/catkin_lint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/catkin_lint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/cccc_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/cccc_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/clang_format_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/clang_format_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/clang_format_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/clang_tidy_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/clang_tidy_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/cmakelint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/cmakelint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/cppcheck_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/cppcheck_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/cpplint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/cpplint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/do_nothing_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/do_nothing_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/docformatter_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/docformatter_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/flawfinder_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/flawfinder_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/groovylint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/groovylint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/isort_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/isort_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/lizard_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/lizard_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/make_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/make_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/mypy_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/mypy_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/perlcritic_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/perlcritic_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/pycodestyle_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/pycodestyle_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/pydocstyle_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/pydocstyle_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/pyflakes_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/pyflakes_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/pylint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/pylint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/ruff_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/ruff_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/shellcheck_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/shellcheck_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/spotbugs_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/spotbugs_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/uncrustify_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/uncrustify_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/xmllint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/xmllint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/yamllint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/plugins/tool/yamllint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/reporting_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:32:41.049269 statick-0.9.4/statick_tool/rsc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/.groovylintrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/CMakeLists.txt.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/_clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/cccc.opt
+-rw-r--r--   0 runner    (1001) docker     (123)    18847 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/discovery_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/exceptions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/gauntlet_ignore.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:32:41.049269 statick-0.9.4/statick_tool/rsc/plugin_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/plugin_mapping/clang-tidy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/plugin_mapping/code_climate.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/plugin_mapping/cppcheck.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/plugin_mapping/make.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/plugin_mapping/perlcritic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/plugin_mapping/spotbugs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/sei_cert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/self_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/spotbugs-security.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/ultimate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/rsc/uncrustify.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/statick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-25 02:32:18.000000 statick-0.9.4/statick_tool/tool_plugin.py
```

### Comparing `statick-0.9.3/LICENSE` & `statick-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/PKG-INFO` & `statick-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statick
-Version: 0.9.3
+Version: 0.9.4
 Summary: Making code quality easier.
 Home-page: https://github.com/sscpac/statick
 Author: SSC Pacific
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -248,14 +248,18 @@
                        commas: disable,
                        document-start: disable,
                        line-length: disable}}'"
       cmakelint:
         flags: "--spaces=2 --filter=-linelength,-whitespace/indent"
 ```
 
+Statick supports the use of some multi-line yaml syntax, namely the `>` syntax.
+See [Stack Overflow](https://stackoverflow.com/questions/3790454/how-do-i-break-a-string-in-yaml-over-multiple-lines)
+and the unit tests for the `config` module for examples.
+
 ### Profiles
 
 _Profiles_ govern how each package will be analyzed by mapping _packages_ to _levels_.
 A default _level_ is specified, then any packages that should be run at a non-default _level_ can be listed.
 
 Multiple profiles can exist, and you can specify which one to use with the `--profile` argument.
 For example, you can have a `profile_objective.yaml` with stricter levels to run for packages.
```

### Comparing `statick-0.9.3/README.md` & `statick-0.9.4/statick.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: statick
+Version: 0.9.4
+Summary: Making code quality easier.
+Home-page: https://github.com/sscpac/statick
+Author: SSC Pacific
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Testing
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # Statick
 
 ![Unit Tests](https://github.com/sscpac/statick/workflows/Statick/badge.svg)
 [![Codecov](https://codecov.io/gh/sscpac/statick/branch/master/graphs/badge.svg)](https://codecov.io/gh/sscpac/statick/)
 [![PyPI version](https://badge.fury.io/py/statick.svg)](https://badge.fury.io/py/statick)
 ![Python Versions](https://img.shields.io/pypi/pyversions/statick.svg)
 ![License](https://img.shields.io/pypi/l/statick.svg)
@@ -230,14 +248,18 @@
                        commas: disable,
                        document-start: disable,
                        line-length: disable}}'"
       cmakelint:
         flags: "--spaces=2 --filter=-linelength,-whitespace/indent"
 ```
 
+Statick supports the use of some multi-line yaml syntax, namely the `>` syntax.
+See [Stack Overflow](https://stackoverflow.com/questions/3790454/how-do-i-break-a-string-in-yaml-over-multiple-lines)
+and the unit tests for the `config` module for examples.
+
 ### Profiles
 
 _Profiles_ govern how each package will be analyzed by mapping _packages_ to _levels_.
 A default _level_ is specified, then any packages that should be run at a non-default _level_ can be listed.
 
 Multiple profiles can exist, and you can specify which one to use with the `--profile` argument.
 For example, you can have a `profile_objective.yaml` with stricter levels to run for packages.
```

### Comparing `statick-0.9.3/setup.py` & `statick-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick` & `statick-0.9.4/statick`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick.egg-info/PKG-INFO` & `statick-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: statick
-Version: 0.9.3
-Summary: Making code quality easier.
-Home-page: https://github.com/sscpac/statick
-Author: SSC Pacific
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Testing
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # Statick
 
 ![Unit Tests](https://github.com/sscpac/statick/workflows/Statick/badge.svg)
 [![Codecov](https://codecov.io/gh/sscpac/statick/branch/master/graphs/badge.svg)](https://codecov.io/gh/sscpac/statick/)
 [![PyPI version](https://badge.fury.io/py/statick.svg)](https://badge.fury.io/py/statick)
 ![Python Versions](https://img.shields.io/pypi/pyversions/statick.svg)
 ![License](https://img.shields.io/pypi/l/statick.svg)
@@ -248,14 +230,18 @@
                        commas: disable,
                        document-start: disable,
                        line-length: disable}}'"
       cmakelint:
         flags: "--spaces=2 --filter=-linelength,-whitespace/indent"
 ```
 
+Statick supports the use of some multi-line yaml syntax, namely the `>` syntax.
+See [Stack Overflow](https://stackoverflow.com/questions/3790454/how-do-i-break-a-string-in-yaml-over-multiple-lines)
+and the unit tests for the `config` module for examples.
+
 ### Profiles
 
 _Profiles_ govern how each package will be analyzed by mapping _packages_ to _levels_.
 A default _level_ is specified, then any packages that should be run at a non-default _level_ can be listed.
 
 Multiple profiles can exist, and you can specify which one to use with the `--profile` argument.
 For example, you can have a `profile_objective.yaml` with stricter levels to run for packages.
```

### Comparing `statick-0.9.3/statick.egg-info/SOURCES.txt` & `statick-0.9.4/statick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/args.py` & `statick-0.9.4/statick_tool/args.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/config.py` & `statick-0.9.4/statick_tool/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,21 @@
                 return configs
         return default
 
     def get_tool_config(
         self, plugin: str, level: str, key: str, default: Optional[str] = None
     ) -> Optional[str]:
         """Get tool flags to use for a plugin at a certain level."""
-        return self.get_plugin_config("tool", plugin, level, key, default)
+        tool_flags = self.get_plugin_config("tool", plugin, level, key, default)
+        # Make sure the flags are on a single line string and remove double-quotes and
+        # whitespace that might have been added from yaml multi-line syntax.
+        if tool_flags is not None:
+            tool_flags = " ".join(tool_flags.split()).strip('"').strip()
+
+        return tool_flags
 
     def get_discovery_config(
         self, plugin: str, level: str, key: str, default: Optional[str] = None
     ) -> Optional[str]:
         """Get discovery flags to use for a plugin at a certain level."""
         return self.get_plugin_config("discovery", plugin, level, key, default)
```

### Comparing `statick-0.9.3/statick_tool/discovery_plugin.py` & `statick-0.9.4/statick_tool/discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/exceptions.py` & `statick-0.9.4/statick_tool/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Exceptions interface.
 
-Exceptions allow for ignoring detected issues. This is commonly done to
-suppress false positives or to ignore issues that a group has no intention
-of addressing.
-
-The two types of exceptions are a list of filenames or regular expressions.
-If using filename matching for the exception it is required that the
-reported issue contain the absolute path to the file containing the issue
-to be ignored. The path for the issue is set in the tool plugin that
-generates the issues.
+Exceptions allow for ignoring detected issues. This is commonly done to suppress false
+positives or to ignore issues that a group has no intention of addressing.
+
+The two types of exceptions are a list of filenames or regular expressions. If using
+filename matching for the exception it is required that the reported issue contain the
+absolute path to the file containing the issue to be ignored. The path for the issue is
+set in the tool plugin that generates the issues.
 """
 import fnmatch
 import logging
 import os
 import re
 from typing import Any, Dict, List, Match, Optional, Pattern
 
@@ -191,16 +189,26 @@
             to_remove: List[Issue] = []
             for issue in tool_issues:
                 if not os.path.isabs(issue.filename):
                     if not warning_printed:
                         self.print_exception_warning(tool)
                         warning_printed = True
                     continue
-                with open(issue.filename, encoding="utf-8") as fid:
-                    lines = fid.readlines()
+                try:
+                    with open(issue.filename, encoding="utf-8") as fid:
+                        try:
+                            lines = fid.readlines()
+                        except UnicodeDecodeError as exc:
+                            logging.warning(
+                                "Could not read %s: %s", issue.filename, exc
+                            )
+                            continue
+                except FileNotFoundError as exc:
+                    logging.warning("Could not read %s: %s", issue.filename, exc)
+                    continue
                 if len(lines) <= 0:
                     continue
                 line_number = int(issue.line_number) - 1
                 if line_number < len(lines) and "NOLINT" in lines[line_number]:
                     to_remove.append(issue)
             issues[tool] = [issue for issue in tool_issues if issue not in to_remove]
         return issues
```

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/c_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/c_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/cmake_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/cmake_discovery_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Discovery plugin to find CMake-based projects.
 
-From the CMake manual, valid CMake files are named `CMakeLists.txt` and `*.cmake`.
-This module will find those files and make them available as part of the package data.
+From the CMake manual, valid CMake files are named `CMakeLists.txt` and `*.cmake`. This
+module will find those files and make them available as part of the package data.
+
 
 https://cmake.org/cmake/help/latest/manual/cmake-language.7.html
 
 The contents of `CMakeLists.txt` is used to discover make targets and header files
 for the current package. That information is made available as part of the package data.
 """
 import argparse
```

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/groovy_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/groovy_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/java_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/java_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/maven_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/maven_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/perl_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/perl_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/python_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/python_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/ros_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/ros_discovery_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         keys: str,
         default: Optional[str] = None,
     ) -> Any:
         """Safe way to check for a value in a nested dict.
 
         Copied from:
 
+
         https://stackoverflow.com/questions/25833613/python-safe-method-to-get-value-of-nested-dictionary
         """
         return reduce(
             lambda d, key: d.get(key, default) if isinstance(d, dict) else default,
             keys.split("."),
             dictionary,
         )
```

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/shell_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/shell_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/xml_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/xml_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/discovery/yaml_discovery_plugin.py` & `statick-0.9.4/statick_tool/plugins/discovery/yaml_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/reporting/code_climate_reporting_plugin.py` & `statick-0.9.4/statick_tool/plugins/reporting/code_climate_reporting_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/reporting/do_nothing_reporting_plugin.py` & `statick-0.9.4/statick_tool/plugins/reporting/do_nothing_reporting_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/reporting/json_reporting_plugin.py` & `statick-0.9.4/statick_tool/plugins/reporting/json_reporting_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/reporting/print_to_console_reporting_plugin.py` & `statick-0.9.4/statick_tool/plugins/reporting/print_to_console_reporting_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/reporting/write_jenkins_warnings_ng_reporting_plugin.py` & `statick-0.9.4/statick_tool/plugins/reporting/write_jenkins_warnings_ng_reporting_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/bandit_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/bandit_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/black_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/black_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/catkin_lint_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/catkin_lint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/cccc_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/cccc_tool_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""Apply CCCC tool and gather results.
 
 To run the CCCC tool locally (without Statick) one way to do so is:
 
-    find . -name \*.h -print -o -name \*.cpp -print | xargs cccc
+find . -name \*.h -print -o -name \*.cpp -print | xargs cccc
 
-That will generate several reports, including HTML. The results can be viewd
-in a web browser.
+That will generate several reports, including HTML. The results can be viewd in a web
+browser.
 """
 import argparse
 import csv
 import logging
 import subprocess
 from pathlib import Path
 from typing import Any, Dict, List, Optional
@@ -170,16 +170,16 @@
 
         return issues
 
     @classmethod
     def parse_config(cls, config_file: str) -> Dict[str, str]:
         """Parse CCCC configuration file.
 
-        Gets warning and error thresholds for all the metrics.
-        An explanation to dump default values to a configuration file is at:
+        Gets warning and error thresholds for all the metrics. An explanation to dump
+        default values to a configuration file is at:
         http://sarnold.github.io/cccc/CCCC_User_Guide.html#config
 
         `cccc --opt_outfile=cccc.opt`
         """
         config: Dict[Any, Any] = {}
 
         if config_file is None:
```

### Comparing `statick-0.9.3/statick_tool/plugins/tool/clang_format_parser.py` & `statick-0.9.4/statick_tool/plugins/tool/clang_format_parser.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/clang_format_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/clang_format_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/clang_tidy_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/clang_tidy_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/cmakelint_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/cmakelint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/cppcheck_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/cppcheck_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/cpplint_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/cpplint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/do_nothing_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/do_nothing_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/docformatter_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/docformatter_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/flawfinder_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/flawfinder_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/groovylint_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/groovylint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/isort_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/isort_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/lizard_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/lizard_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/make_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/make_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/mypy_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/mypy_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/perlcritic_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/perlcritic_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/pycodestyle_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/pycodestyle_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/pydocstyle_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/pydocstyle_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/pyflakes_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/pyflakes_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/pylint_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/pylint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/ruff_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/ruff_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/shellcheck_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/shellcheck_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/spotbugs_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/spotbugs_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/uncrustify_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/uncrustify_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/xmllint_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/xmllint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/plugins/tool/yamllint_tool_plugin.py` & `statick-0.9.4/statick_tool/plugins/tool/yamllint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/profile.py` & `statick-0.9.4/statick_tool/profile.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/reporting_plugin.py` & `statick-0.9.4/statick_tool/reporting_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/resources.py` & `statick-0.9.4/statick_tool/resources.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/.clang-format` & `statick-0.9.4/statick_tool/rsc/.clang-format`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/CMakeLists.txt.in` & `statick-0.9.4/statick_tool/rsc/CMakeLists.txt.in`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/_clang-format` & `statick-0.9.4/statick_tool/rsc/_clang-format`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/cccc.opt` & `statick-0.9.4/statick_tool/rsc/cccc.opt`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/exceptions.yaml` & `statick-0.9.4/statick_tool/rsc/exceptions.yaml`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/gauntlet_ignore.yaml` & `statick-0.9.4/statick_tool/rsc/gauntlet_ignore.yaml`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/plugin_mapping/clang-tidy.txt` & `statick-0.9.4/statick_tool/rsc/plugin_mapping/clang-tidy.txt`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/plugin_mapping/code_climate.txt` & `statick-0.9.4/statick_tool/rsc/plugin_mapping/code_climate.txt`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/plugin_mapping/cppcheck.txt` & `statick-0.9.4/statick_tool/rsc/plugin_mapping/cppcheck.txt`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/spotbugs-security.xml` & `statick-0.9.4/statick_tool/rsc/spotbugs-security.xml`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/rsc/uncrustify.cfg` & `statick-0.9.4/statick_tool/rsc/uncrustify.cfg`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/statick.py` & `statick-0.9.4/statick_tool/statick.py`

 * *Files identical despite different names*

### Comparing `statick-0.9.3/statick_tool/tool_plugin.py` & `statick-0.9.4/statick_tool/tool_plugin.py`

 * *Files identical despite different names*

