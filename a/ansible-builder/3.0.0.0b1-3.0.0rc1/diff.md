# Comparing `tmp/ansible-builder-3.0.0.0b1.tar.gz` & `tmp/ansible-builder-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-builder-3.0.0.0b1.tar", last modified: Wed Apr 19 15:45:27 2023, max compression
+gzip compressed data, was "ansible-builder-3.0.0rc1.tar", last modified: Tue Apr 25 05:32:44 2023, max compression
```

## Comparing `ansible-builder-3.0.0.0b1.tar` & `ansible-builder-3.0.0rc1.tar`

### file list

```diff
@@ -1,224 +1,220 @@
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.477620 ansible-builder-3.0.0.0b1/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      210 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.cherry_picker.toml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      288 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.coveragerc
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       25 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.dockerignore
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/.github/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2036 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       27 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      623 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/documentation_report.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      600 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       23 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/issue_labeler.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      113 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/patchback.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       37 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/pr_labeler_existing.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       90 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/pr_labeler_new.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/.github/test-scripts/
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)     4597 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/test-scripts/setup_pulp.sh
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/.github/workflows/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4750 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/workflows/ci.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      763 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/workflows/triage_existing.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      734 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/workflows/triage_new.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      334 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.readthedocs.yaml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      547 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.yamllint
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1229 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/AUTHORS
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      306 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/CODEOWNERS
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1176 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/CONTRIBUTING.md
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    17443 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ChangeLog
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      827 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/Containerfile
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     9302 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/LICENSE.md
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     3008 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/Makefile
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2866 2023-04-19 15:45:27.477620 ansible-builder-3.0.0.0b1/PKG-INFO
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1766 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/README.md
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      313 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/SECURITY.md
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      494 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/TODO.org
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/ansible_builder/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/__main__.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/__init__.py
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)     6537 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/assemble
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)     3474 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/check_ansible
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)     1618 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/check_galaxy
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)     1480 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/get-extras-packages
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)     3440 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/install-from-bindep
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    14022 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/introspect.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     8136 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/cli.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      157 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/colors.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1198 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/constants.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    17011 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/containerfile.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    13396 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/ee_schema.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      407 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/exceptions.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     9107 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/main.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4633 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/policies.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     3084 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/requirements.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     8843 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/user_definition.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     6117 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/utils.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2866 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/PKG-INFO
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5263 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        1 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/entry_points.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        1 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/not-zip-safe
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       47 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/pbr.json
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       45 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/requires.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       16 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/top_level.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      211 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/bindep.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/demo/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      257 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/demo/execution-environment.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       31 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/demo/requirements.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       67 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/demo/requirements.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/demo/v3_demo/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1277 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/demo/v3_demo/execution-environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/docs/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      612 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/Makefile
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/docs/_static/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/_static/.gitkeep
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/docs/_templates/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/_templates/.gitkeep
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2581 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/collection_metadata.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5018 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/conf.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    10849 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/definition.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      543 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/glossary.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2082 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/index.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      861 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/installation.rst
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      819 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/make.bat
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       15 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/requirements.in
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      522 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/requirements.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     8293 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/usage.rst
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.457620 ansible-builder-3.0.0.0b1/packaging/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/packaging/rpm/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      257 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/packaging/rpm/Dockerfile.epel-7-x86_64
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      167 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/packaging/rpm/Dockerfile.epel-8-x86_64
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      921 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/packaging/rpm/ansible-builder.spec.j2
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      457 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/packaging/rpm/docker-compose.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      464 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/pytest.ini
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       45 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/requirements.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1134 2023-04-19 15:45:27.477620 ansible-builder-3.0.0.0b1/setup.cfg
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      133 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/setup.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5587 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/conftest.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1857 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/README.md
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      108 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/env/settings
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/execution-environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      577 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/project/ansible.posix.at.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      109 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/requirements.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      255 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/run.sh
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_cfg_for_galaxy/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      420 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_cfg_for_galaxy/ansible-test.cfg
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_cfg_for_galaxy/requirements.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.457620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.457620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/other/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/other/reqfile/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       44 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/other/reqfile/requirements.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.457620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/bindep/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/bindep/MANIFEST.json
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       53 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/bindep/bindep.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        2 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/MANIFEST.json
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/meta/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       59 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/meta/execution-environment.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       13 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/my-requirements.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/reqfile/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        2 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/reqfile/MANIFEST.json
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       73 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/reqfile/extra_req.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       67 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/reqfile/requirements.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/blank/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/blank/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       97 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/blank/env/settings
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       15 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/blank/execution-environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/blank/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       99 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/blank/project/blank.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      237 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/blank/run.sh
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/build_args/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      107 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/build_args/base-image.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       73 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/build_args/execution-environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/build_fail/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       78 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/build_fail/execution-environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/definition_files/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/definition_files/bad.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       12 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/definition_files/invalid.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/definition_files/no_galaxy.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/definition_files/no_python.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/needs_git/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/needs_git/execution-environment.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       82 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/needs_git/requirements.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/nested_galaxy_file/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/nested_galaxy_file/foo/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       20 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/nested_galaxy_file/foo/requirements.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/nested_galaxy_file/nested-galaxy.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pip/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pip/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       95 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/env/settings
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       64 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/execution-environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pip/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      131 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/project/pip.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/project/requirements.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      239 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/run.sh
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/prepend_steps/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       67 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/prepend_steps/execution-environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pytz/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pytz/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       30 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/env/extravars
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       96 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/env/settings
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/execution-environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pytz/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      294 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/project/pytz.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       35 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/requirements.yml
--rwxrwxr-x   0 shrews    (1000) shrews    (1000)      699 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/run.sh
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/subversion/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       53 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/bindep.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/subversion/env/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      102 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/env/settings
--rw-rw-r--   0 shrews    (1000) shrews    (1000)       50 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/execution-environment.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/subversion/project/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      239 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/project/subversion.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      241 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/run.sh
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v2/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5135 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v2/RPM-GPG-KEY-redhat-release
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v2/invalid-keyring
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v2/sig_req/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      397 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v2/sig_req/ee-good.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      289 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v2/sig_req/ee-no-orig.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/test/data/v3/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/check_ansible/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      258 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/check_ansible/ee-missing-ansible.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      254 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/check_ansible/ee-missing-runner.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      235 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/check_ansible/ee-skip.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/complete/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      685 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/complete/ee.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/data/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/data/a.dat
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/data/text_files/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/data/text_files/a.txt
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/random.cfg
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/pre_and_post/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      427 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/pre_and_post/ee.yml
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/pre_and_post/requirements.yml
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/integration/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/conftest.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    10171 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/test_build.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    11995 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/test_create.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1425 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/test_help.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2698 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/test_introspect_cli.py
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/pulp_integration/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     7877 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/pulp_integration/test_policies.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1715 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/pulp_integration/test_v3.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)      114 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/requirements.txt
-drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.477620 ansible-builder-3.0.0.0b1/test/unit/
--rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/__init__.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    10219 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_cli.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4871 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_containerfile.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1228 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_introspect.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     4927 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_main.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     5909 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_policies.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1515 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_requirements.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)    11769 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_user_definition.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     2930 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_utils.py
--rw-rw-r--   0 shrews    (1000) shrews    (1000)     1474 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/tox.ini
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.543171 ansible-builder-3.0.0rc1/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      210 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.cherry_picker.toml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      288 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.coveragerc
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       25 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.dockerignore
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.534170 ansible-builder-3.0.0rc1/.github/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.534170 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2036 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       27 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      623 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/documentation_report.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      600 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       23 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/issue_labeler.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      113 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/patchback.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       37 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/pr_labeler_existing.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       90 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/pr_labeler_new.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.535171 ansible-builder-3.0.0rc1/.github/test-scripts/
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     4597 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/.github/test-scripts/setup_pulp.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.535171 ansible-builder-3.0.0rc1/.github/workflows/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4750 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      763 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/workflows/triage_existing.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      734 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/workflows/triage_new.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      334 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.readthedocs.yaml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      547 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/.yamllint
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      306 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/CODEOWNERS
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1176 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      827 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/Containerfile
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9302 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/LICENSE.md
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       42 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/MANIFEST.in
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3008 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/Makefile
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2865 2023-04-25 05:32:44.543171 ansible-builder-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1766 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/README.md
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      313 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/SECURITY.md
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      494 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/TODO.org
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.536171 ansible-builder-3.0.0rc1/ansible_builder/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/ansible_builder/__init__.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/__main__.py
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.536171 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/__init__.py
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     6537 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/assemble
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     3474 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/check_ansible
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     1618 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/check_galaxy
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     5909 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/entrypoint
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     1480 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/get-extras-packages
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     3440 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/install-from-bindep
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    14022 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/introspect.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8136 2023-04-25 05:05:41.000000 ansible-builder-3.0.0rc1/ansible_builder/cli.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      157 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/ansible_builder/colors.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1198 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/constants.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    17766 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/ansible_builder/containerfile.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    13948 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/ansible_builder/ee_schema.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      407 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/exceptions.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9107 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/main.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4633 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/policies.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3084 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/requirements.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8843 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/user_definition.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6382 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/ansible_builder/utils.py
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.536171 ansible-builder-3.0.0rc1/ansible_builder.egg-info/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2865 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/PKG-INFO
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5217 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        1 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/entry_points.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        1 2023-04-25 05:20:20.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/not-zip-safe
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       47 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/pbr.json
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       45 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/requires.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       16 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/top_level.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      211 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/bindep.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.537171 ansible-builder-3.0.0rc1/demo/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1353 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/demo/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.537171 ansible-builder-3.0.0rc1/docs/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      612 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/Makefile
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.537171 ansible-builder-3.0.0rc1/docs/_static/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/_static/.gitkeep
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.537171 ansible-builder-3.0.0rc1/docs/_templates/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/_templates/.gitkeep
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2581 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/collection_metadata.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5018 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/docs/conf.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    13751 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/docs/definition.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      543 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/glossary.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2082 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/index.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      861 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/docs/installation.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      819 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/make.bat
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       15 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/requirements.in
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      522 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/docs/requirements.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8293 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/docs/usage.rst
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.531170 ansible-builder-3.0.0rc1/packaging/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/packaging/rpm/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      257 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/packaging/rpm/Dockerfile.epel-7-x86_64
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      167 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/packaging/rpm/Dockerfile.epel-8-x86_64
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      921 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/packaging/rpm/ansible-builder.spec.j2
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      457 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/packaging/rpm/docker-compose.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      464 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/pytest.ini
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       45 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/requirements.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1197 2023-04-25 05:32:44.543171 ansible-builder-3.0.0rc1/setup.cfg
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      133 2023-04-24 23:43:10.000000 ansible-builder-3.0.0rc1/setup.py
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/__init__.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5587 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/conftest.py
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1857 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/README.md
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      108 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      577 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/project/ansible.posix.at.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      109 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/requirements.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      255 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible_cfg_for_galaxy/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      420 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/ansible_cfg_for_galaxy/ansible-test.cfg
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/ansible_cfg_for_galaxy/requirements.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.531170 ansible-builder-3.0.0rc1/test/data/ansible_collections/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.531170 ansible-builder-3.0.0rc1/test/data/ansible_collections/other/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible_collections/other/reqfile/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       44 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/other/reqfile/requirements.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.531170 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/bindep/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/bindep/MANIFEST.json
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       53 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/bindep/bindep.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        2 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/MANIFEST.json
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/meta/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       59 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/meta/execution-environment.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       13 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/my-requirements.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/reqfile/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        2 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/reqfile/MANIFEST.json
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       73 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/reqfile/extra_req.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       67 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/reqfile/requirements.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/blank/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/blank/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       97 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/blank/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       15 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/blank/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/blank/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       99 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/blank/project/blank.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      237 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/blank/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/build_args/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      107 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/build_args/base-image.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       73 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/build_args/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/build_fail/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       78 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/build_fail/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/definition_files/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      187 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/definition_files/bad.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       12 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/definition_files/invalid.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/definition_files/no_galaxy.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/definition_files/no_python.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/needs_git/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/needs_git/execution-environment.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       82 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/needs_git/requirements.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/nested_galaxy_file/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/nested_galaxy_file/foo/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       20 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/nested_galaxy_file/foo/requirements.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/nested_galaxy_file/nested-galaxy.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pip/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pip/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       95 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       64 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pip/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      131 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/project/pip.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/project/requirements.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      239 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/prepend_steps/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       67 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/prepend_steps/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pytz/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pytz/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       30 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/env/extravars
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       96 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pytz/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      294 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/project/pytz.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       35 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/requirements.yml
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)      699 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/subversion/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       53 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/bindep.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/subversion/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      102 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       50 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/subversion/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      239 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/project/subversion.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      241 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v2/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5135 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v2/RPM-GPG-KEY-redhat-release
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v2/invalid-keyring
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v2/sig_req/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      397 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v2/sig_req/ee-good.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      289 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v2/sig_req/ee-no-orig.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.532171 ansible-builder-3.0.0rc1/test/data/v3/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/check_ansible/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      258 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/check_ansible/ee-missing-ansible.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      254 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/check_ansible/ee-missing-runner.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      235 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/check_ansible/ee-skip.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/complete/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      685 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/complete/ee.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/complete/files/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/complete/files/data/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/complete/files/data/a.dat
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/complete/files/data/text_files/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/complete/files/data/text_files/a.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/complete/files/random.cfg
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.542171 ansible-builder-3.0.0rc1/test/data/v3/pre_and_post/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      427 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/pre_and_post/ee.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/pre_and_post/requirements.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.542171 ansible-builder-3.0.0rc1/test/integration/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/integration/conftest.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    10171 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/integration/test_build.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    13824 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/test/integration/test_create.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1425 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/integration/test_help.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2698 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/integration/test_introspect_cli.py
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.542171 ansible-builder-3.0.0rc1/test/pulp_integration/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     7877 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/pulp_integration/test_policies.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1715 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/pulp_integration/test_v3.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      114 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/requirements.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.543171 ansible-builder-3.0.0rc1/test/unit/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/unit/__init__.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    10219 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_cli.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4871 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_containerfile.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1228 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_introspect.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4927 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_main.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5909 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_policies.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1515 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/unit/test_requirements.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    11769 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_user_definition.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3425 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/test/unit/test_utils.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1474 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/tox.ini
```

### Comparing `ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/bug_report.yml` & `ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/documentation_report.yml` & `ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/documentation_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/feature_request.yml` & `ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/.github/test-scripts/setup_pulp.sh` & `ansible-builder-3.0.0rc1/.github/test-scripts/setup_pulp.sh`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/.github/workflows/ci.yml` & `ansible-builder-3.0.0rc1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/.github/workflows/triage_existing.yml` & `ansible-builder-3.0.0rc1/.github/workflows/triage_existing.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/.github/workflows/triage_new.yml` & `ansible-builder-3.0.0rc1/.github/workflows/triage_new.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/.yamllint` & `ansible-builder-3.0.0rc1/.yamllint`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/CONTRIBUTING.md` & `ansible-builder-3.0.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/Containerfile` & `ansible-builder-3.0.0rc1/Containerfile`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/LICENSE.md` & `ansible-builder-3.0.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/Makefile` & `ansible-builder-3.0.0rc1/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/PKG-INFO` & `ansible-builder-3.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-builder
-Version: 3.0.0.0b1
+Version: 3.0.0rc1
 Summary: "A tool for building Ansible Execution Environments"
 Home-page: https://ansible-builder.readthedocs.io
 Author: Ansible, Inc.
 Author-email: info@ansible.com
 License: Apache Software License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `ansible-builder-3.0.0.0b1/README.md` & `ansible-builder-3.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/assemble` & `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/assemble`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/check_ansible` & `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/check_ansible`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/check_galaxy` & `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/check_galaxy`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/get-extras-packages` & `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/get-extras-packages`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/install-from-bindep` & `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/install-from-bindep`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/introspect.py` & `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/introspect.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/cli.py` & `ansible-builder-3.0.0rc1/ansible_builder/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/constants.py` & `ansible-builder-3.0.0rc1/ansible_builder/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/containerfile.py` & `ansible-builder-3.0.0rc1/ansible_builder/containerfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,14 +152,20 @@
         # any EE version 3 or above, unless explicitly skipped.
         if self.definition.version >= 3 and not self.definition.options['skip_ansible_check']:
             self.steps.append("RUN /output/scripts/check_ansible $PYCMD")
 
         self._prepare_galaxy_copy_steps()
         self._prepare_system_runtime_deps_steps()
 
+        if self.definition.version >= 3 and self.definition.options['relax_passwd_permissions']:
+            self._relax_etc_passwd_permissions()
+
+        if self.definition.version >= 3 and (final_workdir := self.definition.options['workdir']):
+            self._prepare_final_workdir(final_workdir)
+
         # install init package if specified
         # FUTURE: could move this into the pre-install wheel phase
         if init_pip_pkg := self.definition.container_init.get('package_pip'):
             self.steps.append(f"RUN $PYCMD -m pip install --no-cache-dir '{init_pip_pkg}'")
 
         self._insert_custom_steps('append_final')
         self._prepare_label_steps()
@@ -234,18 +240,18 @@
             copy_file(
                 self.definition.ansible_config,
                 os.path.join(self.build_outputs_dir, 'ansible.cfg')
             )
 
         # HACK: this sucks
         scriptres = importlib.resources.files('ansible_builder._target_scripts')
-        for script in ('assemble', 'get-extras-packages', 'install-from-bindep', 'introspect.py', 'check_galaxy', 'check_ansible'):
+        for script in ('assemble', 'get-extras-packages', 'install-from-bindep', 'introspect.py', 'check_galaxy', 'check_ansible', 'entrypoint'):
             with importlib.resources.as_file(scriptres / script) as script_path:
                 # FIXME: just use builtin copy?
-                copy_file(str(script_path), scripts_dir)
+                copy_file(str(script_path), os.path.join(scripts_dir, script))
 
         # later steps depend on base image containing these scripts
         context_dir = Path(self.build_outputs_dir).stem
         self.steps.append(f'COPY {context_dir}/scripts/ /output/scripts/')
 
     def _handle_additional_build_files(self):
         """
@@ -303,14 +309,29 @@
             if section_steps:
                 if isinstance(section_steps, str):
                     lines = section_steps.strip().splitlines()
                 else:
                     lines = section_steps
                 self.steps.extend(lines)
 
+    def _relax_etc_passwd_permissions(self):
+        self.steps.append(
+            "RUN chmod ug+rw /etc/passwd"
+        )
+
+    def _prepare_final_workdir(self, workdir: str):
+        workdir = workdir.strip()
+        if not workdir:
+            return
+
+        self.steps.extend([
+            f"RUN mkdir -p {workdir} && chgrp 0 {workdir} && chmod -R ug+rwx {workdir}",
+            f"WORKDIR {workdir}"
+        ])
+
     def _prepare_label_steps(self):
         self.steps.extend([
             "LABEL ansible-execution-environment=true",
         ])
 
     def _prepare_build_context(self):
         if any(self.definition.get_dep_abs_path(thing) for thing in ('galaxy', 'system', 'python')):
```

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/ee_schema.py` & `ansible-builder-3.0.0rc1/ansible_builder/ee_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,18 +314,26 @@
         },
 
         "options": {
             "description": "Options that effect runtime behavior",
             "type": "object",
             "additionalProperties": False,
             "properties": {
+                "relax_passwd_permissions": {
+                    "description": "allows GID0 write access to /etc/passwd; currently necessary for many uses",
+                    "type": "boolean",
+                },
                 "skip_ansible_check": {
                     "description": "Disables the check for Ansible/Runner in final image",
                     "type": "boolean",
                 },
+                "workdir": {
+                    "description": "Default working directory, also often the homedir for ephemeral UIDs",
+                    "type": ["string", "null"],
+                },
                 "package_manager_path": {
                     "description": "Path to the system package manager to use",
                     "type": "string",
                 },
                 "container_init": {
                     "description": "Customize container startup behavior",
                     "type": "object",
@@ -402,13 +410,15 @@
     JSONSchema can document a "default" value, but it isn't used for validation.
     This method is used to set any default values for the "options" dictionary
     properties.
     """
     options = ee_def.setdefault('options', {})
 
     options.setdefault('skip_ansible_check', False)
+    options.setdefault('relax_passwd_permissions', True)
+    options.setdefault('workdir', '/runner')
     options.setdefault('package_manager_path', '/usr/bin/dnf')
     options.setdefault('container_init', {
         'package_pip': 'dumb-init==1.2.5',
-        'entrypoint': '["dumb-init"]',
+        'entrypoint': '["/output/scripts/entrypoint", "dumb-init"]',
         'cmd': '["bash"]',
     })
```

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/main.py` & `ansible-builder-3.0.0rc1/ansible_builder/main.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/policies.py` & `ansible-builder-3.0.0rc1/ansible_builder/policies.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/requirements.py` & `ansible-builder-3.0.0rc1/ansible_builder/requirements.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/user_definition.py` & `ansible-builder-3.0.0rc1/ansible_builder/user_definition.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder/utils.py` & `ansible-builder-3.0.0rc1/ansible_builder/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,15 +165,19 @@
 
 def copy_file(source: str, dest: str) -> bool:
     should_copy = False
 
     if os.path.abspath(source) == os.path.abspath(dest):
         logger.info("File %s was placed in build context by user, leaving unmodified.", dest)
         return False
-    elif not os.path.exists(dest):
+    if Path(source).is_dir():
+        raise Exception(f"Source {source} can not be a directory. Please use copy_directory instead.")
+    if Path(dest).is_dir():
+        raise Exception(f"Destination {dest} can not be a directory. Please use copy_directory instead.")
+    if not os.path.exists(dest):
         logger.debug("File %s will be created.", dest)
         should_copy = True
     elif not filecmp.cmp(source, dest, shallow=False):
         logger.warning('File %s had modifications and will be rewritten', dest)
         should_copy = True
     elif os.path.getmtime(source) > os.path.getmtime(dest):
         logger.warning('File %s updated time increased and will be rewritten', dest)
```

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder.egg-info/PKG-INFO` & `ansible-builder-3.0.0rc1/ansible_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-builder
-Version: 3.0.0.0b1
+Version: 3.0.0rc1
 Summary: "A tool for building Ansible Execution Environments"
 Home-page: https://ansible-builder.readthedocs.io
 Author: Ansible, Inc.
 Author-email: info@ansible.com
 License: Apache Software License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `ansible-builder-3.0.0.0b1/ansible_builder.egg-info/SOURCES.txt` & `ansible-builder-3.0.0rc1/ansible_builder.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 .cherry_picker.toml
 .coveragerc
 .dockerignore
 .readthedocs.yaml
 .yamllint
-AUTHORS
 CODEOWNERS
 CONTRIBUTING.md
-ChangeLog
 Containerfile
 LICENSE.md
+MANIFEST.in
 Makefile
 README.md
 SECURITY.md
 TODO.org
 bindep.txt
 pytest.ini
 requirements.txt
@@ -52,21 +51,19 @@
 ansible_builder.egg-info/pbr.json
 ansible_builder.egg-info/requires.txt
 ansible_builder.egg-info/top_level.txt
 ansible_builder/_target_scripts/__init__.py
 ansible_builder/_target_scripts/assemble
 ansible_builder/_target_scripts/check_ansible
 ansible_builder/_target_scripts/check_galaxy
+ansible_builder/_target_scripts/entrypoint
 ansible_builder/_target_scripts/get-extras-packages
 ansible_builder/_target_scripts/install-from-bindep
 ansible_builder/_target_scripts/introspect.py
 demo/execution-environment.yml
-demo/requirements.txt
-demo/requirements.yml
-demo/v3_demo/execution-environment.yml
 docs/Makefile
 docs/collection_metadata.rst
 docs/conf.py
 docs/definition.rst
 docs/glossary.rst
 docs/index.rst
 docs/installation.rst
```

### Comparing `ansible-builder-3.0.0.0b1/docs/Makefile` & `ansible-builder-3.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/docs/collection_metadata.rst` & `ansible-builder-3.0.0rc1/docs/collection_metadata.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/docs/conf.py` & `ansible-builder-3.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/docs/definition.rst` & `ansible-builder-3.0.0rc1/docs/definition.rst`

 * *Files 19% similar despite different names*

```diff
@@ -279,31 +279,79 @@
 
 options
 *******
 
 This section is a dictionary that contains keywords/options that can affect
 builder runtime functionality. Valid keys for this section are:
 
+    ``container_init``
+      A dictionary with keys that allow for customization of the container ``ENTRYPOINT`` and
+      ``CMD`` directives (and related behaviors). Customizing these behaviors is an advanced
+      task, and may result in subtle, difficult-to-debug failures. As the provided defaults for
+      this section control a number of intertwined behaviors, overriding any value will skip all
+      remaining defaults in this dictionary.
+      Valid keys are:
+
+      ``cmd``
+        Literal value for the ``CMD`` Containerfile directive. The default value is ``["bash"]``.
+
+      ``entrypoint``
+        Literal value for the ``ENTRYPOINT`` Containerfile directive. The
+        default entrypoint behavior handles signal propagation to subprocesses, as well as attempting to
+        ensure at runtime that the container user has a proper environment with a valid writeable
+        home directory, represented in ``/etc/passwd``, with the ``HOME`` envvar set to match. The default
+        entrypoint script may emit warnings to ``stderr`` in cases where it is unable to suitably adjust the
+        user runtime environment. This behavior can be ignored or elevated to a fatal error; consult the
+        source for the ``entrypoint`` target script for more details. The default value is
+        ``["/output/scripts/entrypoint", "dumb-init"]``.
+
+      ``package_pip``
+        Package to install via pip for entrypoint support. This package will be installed in the final build image.
+        The default value is ``dumb-init==1.2.5``.
+
     ``package_manager_path``
       A string with the path to the package manager (dnf or microdnf) to use.
       The default is ``/usr/bin/dnf``. This value will be used to install a
       python interpreter, if specified in ``dependencies``, and during the
       build phase by the ``assemble`` script.
 
     ``skip_ansible_check``
       This boolean value controls whether or not the check for an installation
       of Ansible and Ansible Runner is performed on the final image. Set this
       value to ``True`` to not perform this check. The default is ``False``.
 
+    ``relax_passwd_permissions``
+      This boolean value controls whether the ``root`` group (GID 0) is explicitly granted
+      write permission to ``/etc/passwd`` in the final container image. The default entrypoint
+      script may attempt to update ``/etc/passwd`` under some container runtimes with dynamically
+      created users to ensure a fully-functional POSIX user environment and home directory. Disabling
+      this capability can cause failures of software features that require users to be listed in
+      ``/etc/passwd`` with a valid and writeable home directory (eg, ``async`` in ansible-core, and the
+      ``~username`` shell expansion). The default is ``True``.
+
+    ``workdir``
+      Default current working directory for new processes started under the final container
+      image. Some container runtimes also use this value as ``HOME`` for dynamically-created
+      users in the ``root`` (GID 0) group. When this value is specified, the directory will be
+      created (if it doesn't already exist), set to ``root`` group ownership, and ``rwx`` group
+      permissions recursively applied to it. The default value is ``/runner``.
+
+
 Example ``options`` section:
 
 .. code:: yaml
 
     options:
+        container_init:
+            package_pip: dumb-init>=1.2.5
+            entrypoint: '["dumb-init"]'
+            cmd: '["csh"]'
         package_manager_path: /usr/bin/microdnf
-        skip_ansible_check: True
+        relax_password_permissions: false
+        skip_ansible_check: true
+        workdir: /myworkdir
 
 version
 *******
 
 This is an integer value that sets the version of the format being used. This
 must be ``3`` for the v3 version.
```

### Comparing `ansible-builder-3.0.0.0b1/docs/glossary.rst` & `ansible-builder-3.0.0rc1/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/docs/index.rst` & `ansible-builder-3.0.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/docs/installation.rst` & `ansible-builder-3.0.0rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/docs/make.bat` & `ansible-builder-3.0.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/docs/requirements.txt` & `ansible-builder-3.0.0rc1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/docs/usage.rst` & `ansible-builder-3.0.0rc1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/packaging/rpm/ansible-builder.spec.j2` & `ansible-builder-3.0.0rc1/packaging/rpm/ansible-builder.spec.j2`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/setup.cfg` & `ansible-builder-3.0.0rc1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -33,11 +33,16 @@
 console_scripts = 
 	ansible-builder = ansible_builder.cli:run
 
 [files]
 packages = 
 	ansible_builder
 
+[pbr]
+skip_changelog = yes
+skip_authors = yes
+skip_reno = yes
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ansible-builder-3.0.0.0b1/test/conftest.py` & `ansible-builder-3.0.0rc1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/data/README.md` & `ansible-builder-3.0.0rc1/test/data/README.md`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/project/ansible.posix.at.yml` & `ansible-builder-3.0.0rc1/test/data/ansible.posix.at/project/ansible.posix.at.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/data/run.sh` & `ansible-builder-3.0.0rc1/test/data/run.sh`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/data/v2/RPM-GPG-KEY-redhat-release` & `ansible-builder-3.0.0rc1/test/data/v2/RPM-GPG-KEY-redhat-release`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/data/v3/complete/ee.yml` & `ansible-builder-3.0.0rc1/test/data/v3/complete/ee.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/integration/test_build.py` & `ansible-builder-3.0.0rc1/test/integration/test_build.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/integration/test_create.py` & `ansible-builder-3.0.0rc1/test/integration/test_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -240,15 +240,18 @@
     assert 'RUN /output/scripts/check_galaxy' in text
 
     # verify that the ansible/runner check is performed
     assert 'RUN /output/scripts/check_ansible' in text
 
     # verify that the default init is being installed and that ENTRYPOINT is set
     assert "RUN $PYCMD -m pip install --no-cache-dir 'dumb-init==" in text
-    assert 'ENTRYPOINT ["dumb-init"]' in text
+    assert 'WORKDIR /runner' in text
+    assert 'RUN chmod ug+rw /etc/passwd' in text
+    assert 'RUN mkdir -p /runner' in text
+    assert 'ENTRYPOINT ["/output/scripts/entrypoint", "dumb-init"]' in text
 
     # check additional_build_files
     myconfigs_path = tmp_path / constants.user_content_subfolder / "myconfigs"
     assert myconfigs_path.is_dir()
     random_file = myconfigs_path / "random.cfg"
     assert random_file.exists()
 
@@ -325,7 +328,69 @@
     containerfile = tmpdir / "Containerfile"
     assert containerfile.exists()
     text = containerfile.read_text()
 
     assert "pip install --no-cache-dir 'custominit==1.2.3'" in text
     assert 'ENTRYPOINT ["custominit"]' in text
     assert 'CMD ["customcmd"]' in text
+
+
+def test_v3_no_relax_passwd_perms(cli, build_dir_and_ee_yml):
+    """
+    Test that disabling 'options.relax_passwd_permissions' works.
+    """
+    ee = """
+    version: 3
+    options:
+        relax_passwd_permissions: false
+    """
+
+    tmpdir, eeyml = build_dir_and_ee_yml(ee)
+    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile')
+
+    containerfile = tmpdir / "Containerfile"
+    assert containerfile.exists()
+    text = containerfile.read_text()
+
+    assert "/etc/passwd" not in text
+
+
+def test_v3_custom_workdir(cli, build_dir_and_ee_yml):
+    """
+    Test that a custom 'options.workdir' creates the dir and sets it
+    """
+    ee = """
+    version: 3
+    options:
+        workdir: /yourmom
+    """
+
+    tmpdir, eeyml = build_dir_and_ee_yml(ee)
+    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile')
+
+    containerfile = tmpdir / "Containerfile"
+    assert containerfile.exists()
+    text = containerfile.read_text()
+
+    assert "WORKDIR /yourmom" in text
+    assert "mkdir -p /yourmom && chgrp 0 /yourmom && chmod -R ug+rwx /yourmom" in text
+
+
+def test_v3_no_workdir(cli, build_dir_and_ee_yml):
+    """
+    Test that empty 'options.workdir' skips the setting and creation of the default.
+    """
+    ee = """
+    version: 3
+    options:
+        workdir:
+    """
+
+    tmpdir, eeyml = build_dir_and_ee_yml(ee)
+    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile')
+
+    containerfile = tmpdir / "Containerfile"
+    assert containerfile.exists()
+    text = containerfile.read_text()
+
+    assert "WORKDIR" not in text
+    assert "mkdir -p /runner" not in text
```

### Comparing `ansible-builder-3.0.0.0b1/test/integration/test_help.py` & `ansible-builder-3.0.0rc1/test/integration/test_help.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/integration/test_introspect_cli.py` & `ansible-builder-3.0.0rc1/test/integration/test_introspect_cli.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/pulp_integration/test_policies.py` & `ansible-builder-3.0.0rc1/test/pulp_integration/test_policies.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/pulp_integration/test_v3.py` & `ansible-builder-3.0.0rc1/test/pulp_integration/test_v3.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/unit/test_cli.py` & `ansible-builder-3.0.0rc1/test/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/unit/test_containerfile.py` & `ansible-builder-3.0.0rc1/test/unit/test_containerfile.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/unit/test_introspect.py` & `ansible-builder-3.0.0rc1/test/unit/test_introspect.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/unit/test_main.py` & `ansible-builder-3.0.0rc1/test/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/unit/test_policies.py` & `ansible-builder-3.0.0rc1/test/unit/test_policies.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/unit/test_requirements.py` & `ansible-builder-3.0.0rc1/test/unit/test_requirements.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/unit/test_user_definition.py` & `ansible-builder-3.0.0rc1/test/unit/test_user_definition.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0.0b1/test/unit/test_utils.py` & `ansible-builder-3.0.0rc1/test/unit/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,14 +51,29 @@
     new_mtime = stat.st_mtime + 1
     os.utime(source_file, (new_atime, new_mtime))
 
     assert copy_file(source_file, dest_file)
     assert not copy_file(source_file, dest_file)
 
 
+def test_copy_file_with_destination_directory(dest_file, source_file):
+    # Change source file to trigger copy_file
+    source_file.write_text('foo\nbar\nzoo')
+
+    with pytest.raises(Exception) as err:
+        copy_file(source_file, '/tmp')
+    assert "can not be a directory" in str(err.value.args[0])
+
+    with pytest.raises(Exception) as err:
+        copy_file('/tmp', dest_file)
+    assert "can not be a directory" in str(err.value.args[0])
+
+    assert copy_file(source_file, dest_file)
+
+
 @pytest.mark.run_command
 def test_failed_command(mocker):
     mocker.patch('ansible_builder.utils.subprocess.Popen.wait', return_value=1)
     with pytest.raises(SystemExit):
         run_command(['sleep', '--invalidargument'])
```

### Comparing `ansible-builder-3.0.0.0b1/tox.ini` & `ansible-builder-3.0.0rc1/tox.ini`

 * *Files identical despite different names*

