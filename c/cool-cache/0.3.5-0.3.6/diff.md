# Comparing `tmp/cool_cache-0.3.5.tar.gz` & `tmp/cool_cache-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cool_cache-0.3.5.tar", last modified: Thu May 25 20:24:24 2023, max compression
+gzip compressed data, was "cool_cache-0.3.6.tar", last modified: Sun May 28 15:21:29 2023, max compression
```

## Comparing `cool_cache-0.3.5.tar` & `cool_cache-0.3.6.tar`

### file list

```diff
@@ -1,378 +1,378 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.326721 cool_cache-0.3.5/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-05-25 20:24:24.326563 cool_cache-0.3.5/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.240941 cool_cache-0.3.5/cool_cache/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.241777 cool_cache-0.3.5/cool_cache/__dependencies__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6126 2023-04-20 16:21:52.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.242034 cool_cache-0.3.5/cool_cache/__dependencies__/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7125 2023-04-20 04:15:05.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.237298 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.243486 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      428 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.244461 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.245456 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/start
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/subrepo
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.245848 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.248762 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.249504 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/logs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/logs/main.py.log
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.249956 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/main/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.250122 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    12380 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/main/setup.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.250467 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/run/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/run/tests
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/run/tests.ps1
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.250579 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.250825 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.251337 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.252444 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.252881 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.256776 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.258798 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.237011 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.258953 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.235898 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.236052 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.259823 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.261600 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.262535 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.262998 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.263255 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.236739 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.263428 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.263617 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.263822 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.263936 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.264109 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.264279 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.264368 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.264454 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.264542 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.264629 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.266957 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.268123 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.268352 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.268876 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.269240 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.269670 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.269979 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
--rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.270307 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.270612 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/tests/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-05-25 20:23:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/tests/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.272089 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1327 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.273563 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.275027 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/start
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/subrepo
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.275347 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.278985 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-25 20:22:33.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.280353 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/main/.keep
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/main/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.280522 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    12054 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    27813 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      486 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.280680 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.280958 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.282938 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.283722 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.284850 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.296939 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/095_000_customize_tree_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/099_050_finish_spaceship_setup_.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.300696 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.239544 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.302901 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.238163 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.238315 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.303800 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.305713 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.310100 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.311491 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.311758 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.239077 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.311943 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.312132 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.312327 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.312758 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.312934 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.313084 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.313166 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.313258 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.313342 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.313420 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.317531 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.319955 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.320824 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.321571 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.322263 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.324219 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/home/.zshenv
--rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/home/.zshrc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.325010 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.325770 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/tests/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      321 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/tests/output.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)      644 2023-05-25 20:22:34.000000 cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/tests/test.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7304 2023-04-20 04:21:13.000000 cool_cache-0.3.5/cool_cache/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.326214 cool_cache-0.3.5/cool_cache/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4340 2022-12-15 16:26:17.000000 cool_cache-0.3.5/cool_cache/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4530 2023-04-20 04:15:05.000000 cool_cache-0.3.5/cool_cache/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)      242 2023-04-20 16:25:12.000000 cool_cache-0.3.5/cool_cache/settings.json
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:24:24.241667 cool_cache-0.3.5/cool_cache.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-05-25 20:24:23.000000 cool_cache-0.3.5/cool_cache.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)    27085 2023-05-25 20:24:24.000000 cool_cache-0.3.5/cool_cache.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-25 20:24:23.000000 cool_cache-0.3.5/cool_cache.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-05-25 20:24:24.000000 cool_cache-0.3.5/cool_cache.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-25 20:24:24.326764 cool_cache-0.3.5/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1421 2023-05-16 16:55:18.000000 cool_cache-0.3.5/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.414023 cool_cache-0.3.6/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-05-28 15:21:29.413864 cool_cache-0.3.6/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.269079 cool_cache-0.3.6/cool_cache/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.271082 cool_cache-0.3.6/cool_cache/__dependencies__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6126 2023-04-20 16:21:52.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.271608 cool_cache-0.3.6/cool_cache/__dependencies__/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7125 2023-04-20 04:15:05.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.263389 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.276785 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      428 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.280050 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.282394 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.282952 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.289977 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.294691 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/logs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/logs/main.py.log
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.295168 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.295365 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12380 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/main/setup.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.297270 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/run/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/run/tests
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/run/tests.ps1
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.297462 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.298554 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.301053 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.301967 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.303136 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.322400 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.329494 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.263118 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.329650 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.261716 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.261982 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.334559 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.337327 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.339280 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.339809 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.341743 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.262847 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.341991 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.342188 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.343364 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.343508 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.343680 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.344676 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.344831 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.344928 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.345020 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.345106 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.351220 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.354445 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.354656 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.359972 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.363754 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.367088 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.367880 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.368497 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.368640 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/tests/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-05-25 20:23:34.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/tests/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.370859 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1327 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.372102 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.373216 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.373590 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.376589 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.378246 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/main/.keep
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/main/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.378527 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12071 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    27813 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      486 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.378734 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.379010 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.379509 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.380775 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.381542 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.389553 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.394913 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.267008 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.395273 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.264224 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.264372 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.396543 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.398210 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.401173 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.401680 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.401942 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.266774 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.402107 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.402300 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.402773 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.402903 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.403095 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.403618 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.403746 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.403853 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.403949 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.404035 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.406889 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.409167 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.409897 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.410316 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.411102 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.411490 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.411795 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.412963 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/tests/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      321 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/tests/output.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      644 2023-05-28 14:01:00.000000 cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/tests/test.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7304 2023-04-20 04:21:13.000000 cool_cache-0.3.6/cool_cache/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.413479 cool_cache-0.3.6/cool_cache/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4340 2022-12-15 16:26:17.000000 cool_cache-0.3.6/cool_cache/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4530 2023-04-20 04:15:05.000000 cool_cache-0.3.6/cool_cache/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      242 2023-04-20 16:25:12.000000 cool_cache-0.3.6/cool_cache/settings.json
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:21:29.270407 cool_cache-0.3.6/cool_cache.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-05-28 15:21:28.000000 cool_cache-0.3.6/cool_cache.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    27085 2023-05-28 15:21:29.000000 cool_cache-0.3.6/cool_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-28 15:21:28.000000 cool_cache-0.3.6/cool_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-05-28 15:21:29.000000 cool_cache-0.3.6/cool_cache.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-28 15:21:29.414067 cool_cache-0.3.6/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1421 2023-05-16 16:55:18.000000 cool_cache-0.3.6/setup.py
```

### Comparing `cool_cache-0.3.5/PKG-INFO` & `cool_cache-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool_cache
-Version: 0.3.5
+Version: 0.3.6
 Summary: Cache any function to disk
 Home-page: https://github.com/jeff-hykin/cool_cache.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__init__.py` & `cool_cache-0.3.6/cool_cache/__dependencies__/__init__.py`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__pycache__/__init__.cpython-38.pyc` & `cool_cache-0.3.6/cool_cache/__dependencies__/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/.gitignore` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/.gitignore`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/README.md` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/README.md`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/commands` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/commands`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/purge` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/purge`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/shell` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/shell`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/commands/start` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/commands/start`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/documentation/setup.md` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/main/license.txt` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/main/license.txt`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/main/setup.py` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/main/setup.py`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/poetry.lock` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/poetry.lock`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/run/tests` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/run/tests`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/run/tests.ps1` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/run/tests.ps1`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/fornix_core` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/.zshenv` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/file_system_py/tests/main.py` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/file_system_py/tests/main.py`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/.gitignore` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/.gitignore`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/README.md` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/README.md`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/project/commands` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/project/commands`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/project/purge` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/project/purge`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/shell` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/shell`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/commands/start` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/commands/start`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_name.png` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/documentation/setup.md` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/main/license.txt` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/main/license.txt`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/main/setup.py` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/main/setup.py`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             if function_reference is None:
                 continue
             try:
                 instructions = dis.get_instructions(function_reference)
             except TypeError as error:
                 continue
             instruction_hashes.append(function_hashers.instructions_to_hash(instructions))
-            child_names = get_referenced_function_names(instructions)
+            child_names = function_hashers.get_referenced_function_names(instructions)
             for child_name in child_names:
                 if child_name not in closed_set:
                     frontier.add(child_name)
         hash_str = ' '.join(instruction_hashes).encode('utf-8')
         return consistent_hash(hash_str)
     
 try:
```

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/poetry.lock` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/poetry.lock`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/fornix_core` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/home/.zshenv` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__dependencies__/__sources__/super_hash/tests/test.py` & `cool_cache-0.3.6/cool_cache/__dependencies__/__sources__/super_hash/tests/test.py`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__init__.py` & `cool_cache-0.3.6/cool_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__pycache__/__init__.cpython-310.pyc` & `cool_cache-0.3.6/cool_cache/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache/__pycache__/__init__.cpython-38.pyc` & `cool_cache-0.3.6/cool_cache/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/cool_cache.egg-info/PKG-INFO` & `cool_cache-0.3.6/cool_cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool-cache
-Version: 0.3.5
+Version: 0.3.6
 Summary: Cache any function to disk
 Home-page: https://github.com/jeff-hykin/cool_cache.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cool_cache-0.3.5/cool_cache.egg-info/SOURCES.txt` & `cool_cache-0.3.6/cool_cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cool_cache-0.3.5/setup.py` & `cool_cache-0.3.6/setup.py`

 * *Files identical despite different names*

