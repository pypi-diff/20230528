# Comparing `tmp/tox-4.5.1.tar.gz` & `tmp/tox-4.5.2.tar.gz`

## Comparing `tox-4.5.1.tar` & `tox-4.5.2.tar`

### file list

```diff
@@ -1,222 +1,222 @@
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 tox-4.5.1/tox.ini
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/__main__.py
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/provision.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/py.typed
--rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/pytest.py
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/report.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/run.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/__init__.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/main.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/of_type.py
--rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/set_env.py
--rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/sets.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/cli/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/cli/env_var.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/cli/ini.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/cli/parse.py
--rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/cli/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/__init__.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/api.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/convert.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/memory.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/section.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/str_convert.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/stringify.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/ini/__init__.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/ini/factor.py
--rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/loader/ini/replace.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/source/__init__.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/source/api.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/source/discover.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/source/ini.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/source/ini_section.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/source/legacy_toml.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/source/setup_cfg.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/config/source/tox_ini.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/__init__.py
--rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/api.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/pep517_backend.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/request.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/stream.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/util.py
--rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/local_sub_process/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/local_sub_process/read_via_thread.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/local_sub_process/read_via_thread_unix.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/execute/local_sub_process/read_via_thread_windows.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/journal/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/journal/env.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/journal/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/plugin/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/plugin/inline.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/plugin/manager.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/plugin/spec.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/__init__.py
--rw-r--r--   0        0        0    18051 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/env_select.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/__init__.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/depends.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/devenv.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/exec_.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/legacy.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/list_env.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/quickstart.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/show_config.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/version_flag.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/run/__init__.py
--rw-r--r--   0        0        0    16573 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/run/common.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/run/parallel.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/run/sequential.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/session/cmd/run/single.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/__init__.py
--rw-r--r--   0        0        0    20134 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/api.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/errors.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/info.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/installer.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/package.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/register.py
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/runner.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/api.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/package.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/pip/__init__.py
--rw-r--r--   0        0        0    10355 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/pip/pip_install.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/pip/req_file.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/pip/req/__init__.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/pip/req/args.py
--rw-r--r--   0        0        0    19406 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/pip/req/file.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/pip/req/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/virtual_env/api.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/virtual_env/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
--rw-r--r--   0        0        0    17577 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/virtual_env/package/pyproject.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/tox_env/python/virtual_env/package/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/util/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/util/ci.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/util/cpu.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/util/file_view.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/util/graph.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/util/path.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 tox-4.5.1/src/tox/util/spinner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/__init__.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 tox-4.5.1/tests/conftest.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.5.1/tests/test_call_modes.py
--rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 tox-4.5.1/tests/test_provision.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 tox-4.5.1/tests/test_report.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 tox-4.5.1/tests/test_run.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.5.1/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/conftest.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/test_main.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/test_of_types.py
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/test_set_env.py
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/test_sets.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/cli/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/cli/conftest.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/cli/test_cli_env_var.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/cli/test_cli_ini.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/cli/test_parse.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/cli/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/__init__.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/test_loader.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/test_memory_loader.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/test_section.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/test_str_convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/__init__.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/conftest.py
--rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/test_factor.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/test_ini_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/replace/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/replace/conftest.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/replace/test_replace.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/replace/test_replace_env_var.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/replace/test_replace_os_pathsep.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/replace/test_replace_os_sep.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/replace/test_replace_posargs.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/replace/test_replace_tox_env.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/loader/ini/replace/test_replace_tty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/source/__init__.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/source/test_discover.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/source/test_legacy_toml.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/source/test_setup_cfg.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tox-4.5.1/tests/config/source/test_source_ini.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tox-4.5.1/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tox-4.5.1/tests/demo_pkg_inline/build.pyi
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.5.1/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.5.1/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.5.1/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tox-4.5.1/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/conftest.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/test_request.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/test_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/local_subprocess/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/local_subprocess/bad_process.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/local_subprocess/local_subprocess_sigint.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/local_subprocess/test_execute_util.py
--rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/local_subprocess/test_local_subprocess.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tox-4.5.1/tests/execute/local_subprocess/tty_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/journal/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.5.1/tests/journal/test_main_journal.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.5.1/tests/plugin/conftest.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 tox-4.5.1/tests/plugin/test_inline.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 tox-4.5.1/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 tox-4.5.1/tests/plugin/test_plugin_custom_config_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/pytest_/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tox-4.5.1/tests/pytest_/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/__init__.py
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/test_env_select.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/test_session_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_depends.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_devenv.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_exec_.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_legacy.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_list_envs.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_parallel.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_quickstart.py
--rw-r--r--   0        0        0    18713 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_sequential.py
--rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_show_config.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/run/__init__.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tox-4.5.1/tests/session/cmd/run/test_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/test_api.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/test_info.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/test_register.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/test_tox_env_api.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/test_tox_env_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/__init__.py
--rw-r--r--   0        0        0     8593 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/test_python_api.py
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/test_python_runner.py
--rw-r--r--   0        0        0    17036 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/pip/test_pip_install.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/pip/test_req_file.py
--rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/pip/req/test_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/test-pkg/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/virtual_env/test_setuptools.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/virtual_env/test_virtualenv_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/virtual_env/package/conftest.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 tox-4.5.1/tests/tox_env/python/virtual_env/package/test_python_package_util.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tox-4.5.1/tests/type_check/add_config_container_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.1/tests/util/__init__.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 tox-4.5.1/tests/util/test_ci.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tox-4.5.1/tests/util/test_cpu.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.5.1/tests/util/test_graph.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.5.1/tests/util/test_path.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tox-4.5.1/tests/util/test_spinner.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.5.1/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.5.1/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.5.1/README.md
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 tox-4.5.1/pyproject.toml
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 tox-4.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 tox-4.5.2/tox.ini
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/__main__.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/provision.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/py.typed
+-rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/pytest.py
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/report.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/run.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/__init__.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/main.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/of_type.py
+-rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/set_env.py
+-rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/sets.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/env_var.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/ini.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/parse.py
+-rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/__init__.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/api.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/convert.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/memory.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/section.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/str_convert.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/stringify.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/ini/factor.py
+-rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/ini/replace.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/__init__.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/api.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/discover.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/ini.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/ini_section.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/legacy_toml.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/setup_cfg.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/tox_ini.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/__init__.py
+-rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/api.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/pep517_backend.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/request.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/stream.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/util.py
+-rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/local_sub_process/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread_unix.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread_windows.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/journal/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/journal/env.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/journal/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/plugin/__init__.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/plugin/inline.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/plugin/manager.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/plugin/spec.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/__init__.py
+-rw-r--r--   0        0        0    18083 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/env_select.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/depends.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/devenv.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/exec_.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/legacy.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/list_env.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/quickstart.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/show_config.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/version_flag.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0    16573 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/common.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/parallel.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/sequential.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/single.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/__init__.py
+-rw-r--r--   0        0        0    20134 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/api.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/errors.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/info.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/installer.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/package.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/register.py
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/runner.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/api.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/package.py
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/__init__.py
+-rw-r--r--   0        0        0    10355 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/pip_install.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req_file.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req/__init__.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req/args.py
+-rw-r--r--   0        0        0    19406 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req/file.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/api.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
+-rw-r--r--   0        0        0    17577 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/package/pyproject.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/package/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/ci.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/cpu.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/file_view.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/graph.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/path.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/spinner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 tox-4.5.2/tests/conftest.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_call_modes.py
+-rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_provision.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_report.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_run.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/conftest.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_main.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_of_types.py
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_set_env.py
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_sets.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/conftest.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/test_cli_env_var.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/test_cli_ini.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/test_parse.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/__init__.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/test_loader.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/test_memory_loader.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/test_section.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/test_str_convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/conftest.py
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/test_factor.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/test_ini_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/conftest.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_env_var.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_os_pathsep.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_os_sep.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_posargs.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_tox_env.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_tty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/__init__.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/test_discover.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/test_legacy_toml.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/test_setup_cfg.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/test_source_ini.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_inline/build.pyi
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/conftest.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/test_request.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/test_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/bad_process.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/local_subprocess_sigint.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/test_execute_util.py
+-rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/test_local_subprocess.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/tty_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/journal/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.5.2/tests/journal/test_main_journal.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.5.2/tests/plugin/conftest.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 tox-4.5.2/tests/plugin/test_inline.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 tox-4.5.2/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 tox-4.5.2/tests/plugin/test_plugin_custom_config_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/pytest_/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tox-4.5.2/tests/pytest_/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/__init__.py
+-rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/test_env_select.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/test_session_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_depends.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_devenv.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_exec_.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_legacy.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_list_envs.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_parallel.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_quickstart.py
+-rw-r--r--   0        0        0    18713 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_sequential.py
+-rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_show_config.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/run/test_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_api.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_info.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_register.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_tox_env_api.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_tox_env_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/__init__.py
+-rw-r--r--   0        0        0     8593 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/test_python_api.py
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/test_python_runner.py
+-rw-r--r--   0        0        0    17036 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/pip/test_pip_install.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/pip/test_req_file.py
+-rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/pip/req/test_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/test-pkg/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/test_setuptools.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/test_virtualenv_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/conftest.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
+-rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/test_python_package_util.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tox-4.5.2/tests/type_check/add_config_container_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/__init__.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_ci.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_cpu.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_graph.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_path.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_spinner.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.5.2/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.5.2/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.5.2/README.md
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 tox-4.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 tox-4.5.2/PKG-INFO
```

### Comparing `tox-4.5.1/tox.ini` & `tox-4.5.2/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tox]
 requires =
     tox>=4.2
 env_list =
     fix
+    py312
     py311
     py310
     py39
     py38
     py37
     cov
     type
@@ -36,28 +37,28 @@
       tests --durations 5 --run-integration}
     diff-cover --compare-branch {env:DIFF_AGAINST:origin/main} {toxworkdir}{/}coverage.{envname}.xml
 
 [testenv:fix]
 description = format the code base to adhere to our styles, and complain about what we cannot do automatically
 skip_install = true
 deps =
-    pre-commit>=3.2.2
+    pre-commit>=3.3.2
 pass_env =
     {[testenv]passenv}
     PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure {posargs}
     python -c 'print(r"hint: run {envbindir}{/}pre-commit install to add checks as pre-commit hook")'
 
 [testenv:type]
 description = run type check on code base
 deps =
-    mypy==1.2
+    mypy==1.3
     types-cachetools>=5.3.0.5
-    types-chardet>=5.0.4.3
+    types-chardet>=5.0.4.6
 commands =
     mypy src/tox
     mypy tests
 
 [testenv:docs]
 description = build documentation
 extras =
```

### Comparing `tox-4.5.1/src/tox/provision.py` & `tox-4.5.2/src/tox/provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/pytest.py` & `tox-4.5.2/src/tox/pytest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/report.py` & `tox-4.5.2/src/tox/report.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/run.py` & `tox-4.5.2/src/tox/run.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/main.py` & `tox-4.5.2/src/tox/config/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/of_type.py` & `tox-4.5.2/src/tox/config/of_type.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/set_env.py` & `tox-4.5.2/src/tox/config/set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/sets.py` & `tox-4.5.2/src/tox/config/sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/types.py` & `tox-4.5.2/src/tox/config/types.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/cli/env_var.py` & `tox-4.5.2/src/tox/config/cli/env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/cli/ini.py` & `tox-4.5.2/src/tox/config/cli/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/cli/parse.py` & `tox-4.5.2/src/tox/config/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/cli/parser.py` & `tox-4.5.2/src/tox/config/cli/parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/loader/api.py` & `tox-4.5.2/src/tox/config/loader/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/loader/convert.py` & `tox-4.5.2/src/tox/config/loader/convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/loader/memory.py` & `tox-4.5.2/src/tox/config/loader/memory.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/loader/section.py` & `tox-4.5.2/src/tox/config/loader/section.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/loader/str_convert.py` & `tox-4.5.2/src/tox/config/loader/str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/loader/stringify.py` & `tox-4.5.2/src/tox/config/loader/stringify.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/loader/ini/__init__.py` & `tox-4.5.2/src/tox/config/loader/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/loader/ini/factor.py` & `tox-4.5.2/src/tox/config/loader/ini/factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/loader/ini/replace.py` & `tox-4.5.2/src/tox/config/loader/ini/replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/source/api.py` & `tox-4.5.2/src/tox/config/source/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/source/discover.py` & `tox-4.5.2/src/tox/config/source/discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/source/ini.py` & `tox-4.5.2/src/tox/config/source/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/source/ini_section.py` & `tox-4.5.2/src/tox/config/source/ini_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/config/source/legacy_toml.py` & `tox-4.5.2/src/tox/config/source/legacy_toml.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/execute/api.py` & `tox-4.5.2/src/tox/execute/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/execute/pep517_backend.py` & `tox-4.5.2/src/tox/execute/pep517_backend.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/execute/request.py` & `tox-4.5.2/src/tox/execute/request.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/execute/stream.py` & `tox-4.5.2/src/tox/execute/stream.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/execute/util.py` & `tox-4.5.2/src/tox/execute/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/execute/local_sub_process/__init__.py` & `tox-4.5.2/src/tox/execute/local_sub_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/execute/local_sub_process/read_via_thread.py` & `tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/execute/local_sub_process/read_via_thread_unix.py` & `tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread_unix.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/execute/local_sub_process/read_via_thread_windows.py` & `tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread_windows.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/journal/env.py` & `tox-4.5.2/src/tox/journal/env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/journal/main.py` & `tox-4.5.2/src/tox/journal/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/plugin/__init__.py` & `tox-4.5.2/src/tox/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/plugin/inline.py` & `tox-4.5.2/src/tox/plugin/inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/plugin/manager.py` & `tox-4.5.2/src/tox/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/plugin/spec.py` & `tox-4.5.2/src/tox/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/env_select.py` & `tox-4.5.2/src/tox/session/env_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,28 +121,31 @@
     def __init__(self, state: State) -> None:
         # needs core to load the default tox environment list
         # to load the package environments of a run environments we need the run environment builder
         # to load labels we need core + the run environment
         self.on_empty_fallback_py = True
         self._warned_about: set[str] = set()  #: shared set of skipped environments that were already warned about
         self._state = state
-        self._cli_envs: CliEnv | None = getattr(self._state.conf.options, "env", None)
         self._defined_envs_: None | dict[str, _ToxEnvInfo] = None
         self._pkg_env_counter: Counter[str] = Counter()
         from tox.plugin.manager import MANAGER
 
         self._manager = MANAGER
         self._log_handler = self._state._options.log_handler
         self._journal = self._state._journal
         self._provision: None | tuple[bool, str] = None
 
         self._state.conf.core.add_config("labels", Dict[str, EnvList], {}, "core labels")
         tox_env_filter_regex = getattr(state.conf.options, "skip_env", "").strip()
         self._filter_re = re.compile(tox_env_filter_regex) if tox_env_filter_regex else None
 
+    @property
+    def _cli_envs(self) -> CliEnv | None:
+        return getattr(self._state.conf.options, "env", None)
+
     def _collect_names(self) -> Iterator[tuple[Iterable[str], bool]]:
         """:return: sources of tox environments defined with name and if is marked as target to run"""
         if self._provision is not None:  # pragma: no branch
             yield (self._provision[1],), False
         env_list, everything_active = self._state.conf.core["env_list"], False
         if self._cli_envs is None or self._cli_envs.is_default_list:
             yield env_list, True
```

### Comparing `tox-4.5.1/src/tox/session/state.py` & `tox-4.5.2/src/tox/session/state.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/depends.py` & `tox-4.5.2/src/tox/session/cmd/depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/devenv.py` & `tox-4.5.2/src/tox/session/cmd/devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/exec_.py` & `tox-4.5.2/src/tox/session/cmd/exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/legacy.py` & `tox-4.5.2/src/tox/session/cmd/legacy.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,16 @@
     _handle_legacy_only_flags(option, state.envs)
 
     if option.show_config:
         return show_config(state)
     if option.list_envs or option.list_envs_all:
         return list_env(state)
     if option.devenv_path:
+        if option.env.is_default_list:
+            option.env = CliEnv(["py"])
         option.devenv_path = Path(option.devenv_path)
         return devenv(state)
     if option.parallel != 0:  # only 0 means sequential
         return run_parallel(state)
     return run_sequential(state)
```

### Comparing `tox-4.5.1/src/tox/session/cmd/list_env.py` & `tox-4.5.2/src/tox/session/cmd/list_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/quickstart.py` & `tox-4.5.2/src/tox/session/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/show_config.py` & `tox-4.5.2/src/tox/session/cmd/show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/version_flag.py` & `tox-4.5.2/src/tox/session/cmd/version_flag.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/run/common.py` & `tox-4.5.2/src/tox/session/cmd/run/common.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/run/parallel.py` & `tox-4.5.2/src/tox/session/cmd/run/parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/run/sequential.py` & `tox-4.5.2/src/tox/session/cmd/run/sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/session/cmd/run/single.py` & `tox-4.5.2/src/tox/session/cmd/run/single.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/api.py` & `tox-4.5.2/src/tox/tox_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/info.py` & `tox-4.5.2/src/tox/tox_env/info.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/installer.py` & `tox-4.5.2/src/tox/tox_env/installer.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/package.py` & `tox-4.5.2/src/tox/tox_env/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/register.py` & `tox-4.5.2/src/tox/tox_env/register.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/runner.py` & `tox-4.5.2/src/tox/tox_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/util.py` & `tox-4.5.2/src/tox/tox_env/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/api.py` & `tox-4.5.2/src/tox/tox_env/python/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/package.py` & `tox-4.5.2/src/tox/tox_env/python/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/runner.py` & `tox-4.5.2/src/tox/tox_env/python/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/pip/pip_install.py` & `tox-4.5.2/src/tox/tox_env/python/pip/pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/pip/req_file.py` & `tox-4.5.2/src/tox/tox_env/python/pip/req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/pip/req/args.py` & `tox-4.5.2/src/tox/tox_env/python/pip/req/args.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/pip/req/file.py` & `tox-4.5.2/src/tox/tox_env/python/pip/req/file.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/pip/req/util.py` & `tox-4.5.2/src/tox/tox_env/python/pip/req/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/virtual_env/api.py` & `tox-4.5.2/src/tox/tox_env/python/virtual_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/virtual_env/runner.py` & `tox-4.5.2/src/tox/tox_env/python/virtual_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/virtual_env/package/cmd_builder.py` & `tox-4.5.2/src/tox/tox_env/python/virtual_env/package/cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/virtual_env/package/pyproject.py` & `tox-4.5.2/src/tox/tox_env/python/virtual_env/package/pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/tox_env/python/virtual_env/package/util.py` & `tox-4.5.2/src/tox/tox_env/python/virtual_env/package/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/util/ci.py` & `tox-4.5.2/src/tox/util/ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/util/file_view.py` & `tox-4.5.2/src/tox/util/file_view.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/util/graph.py` & `tox-4.5.2/src/tox/util/graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/util/path.py` & `tox-4.5.2/src/tox/util/path.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/src/tox/util/spinner.py` & `tox-4.5.2/src/tox/util/spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/conftest.py` & `tox-4.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/test_provision.py` & `tox-4.5.2/tests/test_provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/test_report.py` & `tox-4.5.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/test_run.py` & `tox-4.5.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/test_version.py` & `tox-4.5.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/test_main.py` & `tox-4.5.2/tests/config/test_main.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/test_of_types.py` & `tox-4.5.2/tests/config/test_of_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/test_set_env.py` & `tox-4.5.2/tests/config/test_set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/test_sets.py` & `tox-4.5.2/tests/config/test_sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/test_types.py` & `tox-4.5.2/tests/config/test_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/cli/conftest.py` & `tox-4.5.2/tests/config/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/cli/test_cli_env_var.py` & `tox-4.5.2/tests/config/cli/test_cli_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/cli/test_cli_ini.py` & `tox-4.5.2/tests/config/cli/test_cli_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/cli/test_parse.py` & `tox-4.5.2/tests/config/cli/test_parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/cli/test_parser.py` & `tox-4.5.2/tests/config/cli/test_parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/test_loader.py` & `tox-4.5.2/tests/config/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/test_memory_loader.py` & `tox-4.5.2/tests/config/loader/test_memory_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/test_section.py` & `tox-4.5.2/tests/config/loader/test_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/test_str_convert.py` & `tox-4.5.2/tests/config/loader/test_str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/conftest.py` & `tox-4.5.2/tests/config/loader/ini/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/test_factor.py` & `tox-4.5.2/tests/config/loader/ini/test_factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/test_ini_loader.py` & `tox-4.5.2/tests/config/loader/ini/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/replace/conftest.py` & `tox-4.5.2/tests/config/loader/ini/replace/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/replace/test_replace.py` & `tox-4.5.2/tests/config/loader/ini/replace/test_replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/replace/test_replace_env_var.py` & `tox-4.5.2/tests/config/loader/ini/replace/test_replace_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/replace/test_replace_os_sep.py` & `tox-4.5.2/tests/config/loader/ini/replace/test_replace_os_sep.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/replace/test_replace_posargs.py` & `tox-4.5.2/tests/config/loader/ini/replace/test_replace_posargs.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/replace/test_replace_tox_env.py` & `tox-4.5.2/tests/config/loader/ini/replace/test_replace_tox_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/loader/ini/replace/test_replace_tty.py` & `tox-4.5.2/tests/config/loader/ini/replace/test_replace_tty.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/source/test_discover.py` & `tox-4.5.2/tests/config/source/test_discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/source/test_setup_cfg.py` & `tox-4.5.2/tests/config/source/test_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/config/source/test_source_ini.py` & `tox-4.5.2/tests/config/source/test_source_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/demo_pkg_inline/build.py` & `tox-4.5.2/tests/demo_pkg_inline/build.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/demo_pkg_inline/build.pyi` & `tox-4.5.2/tests/demo_pkg_inline/build.pyi`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/execute/test_request.py` & `tox-4.5.2/tests/execute/test_request.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/execute/local_subprocess/bad_process.py` & `tox-4.5.2/tests/execute/local_subprocess/bad_process.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/execute/local_subprocess/local_subprocess_sigint.py` & `tox-4.5.2/tests/execute/local_subprocess/local_subprocess_sigint.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/execute/local_subprocess/test_execute_util.py` & `tox-4.5.2/tests/execute/local_subprocess/test_execute_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/execute/local_subprocess/test_local_subprocess.py` & `tox-4.5.2/tests/execute/local_subprocess/test_local_subprocess.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/journal/test_main_journal.py` & `tox-4.5.2/tests/journal/test_main_journal.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/plugin/test_inline.py` & `tox-4.5.2/tests/plugin/test_inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/plugin/test_plugin.py` & `tox-4.5.2/tests/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/plugin/test_plugin_custom_config_set.py` & `tox-4.5.2/tests/plugin/test_plugin_custom_config_set.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/pytest_/test_init.py` & `tox-4.5.2/tests/pytest_/test_init.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/test_env_select.py` & `tox-4.5.2/tests/session/test_env_select.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 import pytest
 
+from tox.config.cli.parse import get_options
 from tox.pytest import MonkeyPatch, ToxProjectCreator
+from tox.session.env_select import CliEnv, EnvSelector
+from tox.session.state import State
 
 
 def test_label_core_can_define(tox_project: ToxProjectCreator) -> None:
     ini = """
         [tox]
         labels =
             test = py3{10,9}
@@ -113,7 +116,15 @@
 
 def test_tox_skip_env_logs(tox_project: ToxProjectCreator, monkeypatch: MonkeyPatch) -> None:
     monkeypatch.setenv("TOX_SKIP_ENV", "m[y]py")
     project = tox_project({"tox.ini": "[tox]\nenv_list = py3{10,9},mypy"})
     outcome = project.run("l", "--no-desc")
     outcome.assert_success()
     outcome.assert_out_err("ROOT: skip environment mypy, matches filter 'm[y]py'\npy310\npy39\n", "")
+
+
+def test_env_select_lazily_looks_at_envs() -> None:
+    state = State(get_options(), [])
+    env_selector = EnvSelector(state)
+    # late-assigning env should be reflected in env_selector
+    state.conf.options.env = CliEnv("py")
+    assert set(env_selector.iter()) == {"py"}
```

### Comparing `tox-4.5.1/tests/session/test_session_common.py` & `tox-4.5.2/tests/session/test_session_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/test_depends.py` & `tox-4.5.2/tests/session/cmd/test_depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/test_devenv.py` & `tox-4.5.2/tests/session/cmd/test_devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/test_exec_.py` & `tox-4.5.2/tests/session/cmd/test_exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/test_legacy.py` & `tox-4.5.2/tests/session/cmd/test_legacy.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,22 +74,35 @@
 
     assert list_env.call_count == 1
     assert outcome.state.conf.options.list_no_description is (verbose < 1)
     assert outcome.state.conf.options.list_default_only is False
     assert outcome.state.conf.options.show_core is False
 
 
-def test_legacy_devenv(tox_project: ToxProjectCreator, mocker: MockerFixture, tmp_path: Path) -> None:
-    devenv = mocker.patch("tox.session.cmd.legacy.devenv")
+@pytest.mark.parametrize(
+    "args",
+    [
+        pytest.param((), id="empty"),
+        pytest.param(("-e", "py"), id="select"),
+    ],
+)
+def test_legacy_devenv(
+    tox_project: ToxProjectCreator,
+    mocker: MockerFixture,
+    tmp_path: Path,
+    args: tuple[str, ...],
+) -> None:
+    run_sequential = mocker.patch("tox.session.cmd.devenv.run_sequential")
     into = tmp_path / "b"
 
-    outcome = tox_project({"tox.ini": ""}).run("le", "--devenv", str(into), "-e", "py")
+    outcome = tox_project({"tox.ini": ""}).run("le", "--devenv", str(into), *args)
 
-    assert devenv.call_count == 1
+    assert run_sequential.call_count == 1
     assert outcome.state.conf.options.devenv_path == into
+    assert set(outcome.state.conf.options.env) == {"py"}
 
 
 def test_legacy_run_parallel(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     run_parallel = mocker.patch("tox.session.cmd.legacy.run_parallel")
 
     tox_project({"tox.ini": ""}).run("le", "-p", "all", "-e", "py")
```

### Comparing `tox-4.5.1/tests/session/cmd/test_list_envs.py` & `tox-4.5.2/tests/session/cmd/test_list_envs.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/test_parallel.py` & `tox-4.5.2/tests/session/cmd/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/test_quickstart.py` & `tox-4.5.2/tests/session/cmd/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/test_sequential.py` & `tox-4.5.2/tests/session/cmd/test_sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/test_show_config.py` & `tox-4.5.2/tests/session/cmd/test_show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/test_state.py` & `tox-4.5.2/tests/session/cmd/test_state.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/session/cmd/run/test_common.py` & `tox-4.5.2/tests/session/cmd/run/test_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/test_api.py` & `tox-4.5.2/tests/tox_env/test_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/test_register.py` & `tox-4.5.2/tests/tox_env/test_register.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/test_tox_env_api.py` & `tox-4.5.2/tests/tox_env/test_tox_env_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/test_tox_env_runner.py` & `tox-4.5.2/tests/tox_env/test_tox_env_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/test_python_api.py` & `tox-4.5.2/tests/tox_env/python/test_python_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/test_python_runner.py` & `tox-4.5.2/tests/tox_env/python/test_python_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/pip/test_pip_install.py` & `tox-4.5.2/tests/tox_env/python/pip/test_pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/pip/test_req_file.py` & `tox-4.5.2/tests/tox_env/python/pip/test_req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/pip/req/test_file.py` & `tox-4.5.2/tests/tox_env/python/pip/req/test_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/virtual_env/test_setuptools.py` & `tox-4.5.2/tests/tox_env/python/virtual_env/test_setuptools.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/virtual_env/test_virtualenv_api.py` & `tox-4.5.2/tests/tox_env/python/virtual_env/test_virtualenv_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/virtual_env/package/conftest.py` & `tox-4.5.2/tests/tox_env/python/virtual_env/package/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py` & `tox-4.5.2/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/virtual_env/package/test_package_pyproject.py` & `tox-4.5.2/tests/tox_env/python/virtual_env/package/test_package_pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/tox_env/python/virtual_env/package/test_python_package_util.py` & `tox-4.5.2/tests/tox_env/python/virtual_env/package/test_python_package_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/util/test_ci.py` & `tox-4.5.2/tests/util/test_ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/util/test_graph.py` & `tox-4.5.2/tests/util/test_graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/tests/util/test_spinner.py` & `tox-4.5.2/tests/util/test_spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/LICENSE` & `tox-4.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/README.md` & `tox-4.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tox-4.5.1/pyproject.toml` & `tox-4.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.14",
+  "hatchling>=1.17",
 ]
 
 [project]
 name = "tox"
 description = "tox is a generic virtualenv management and test command line tool"
 readme.content-type = "text/markdown"
 readme.file = "README.md"
@@ -47,48 +47,48 @@
 dynamic = [
   "version",
 ]
 dependencies = [
   "cachetools>=5.3",
   "chardet>=5.1",
   "colorama>=0.4.6",
-  "filelock>=3.11",
-  'importlib-metadata>=6.4.1; python_version < "3.8"',
+  "filelock>=3.12",
+  'importlib-metadata>=6.6; python_version < "3.8"',
   "packaging>=23.1",
-  "platformdirs>=3.2",
+  "platformdirs>=3.5.1",
   "pluggy>=1",
   "pyproject-api>=1.5.1",
   'tomli>=2.0.1; python_version < "3.11"',
-  'typing-extensions>=4.5; python_version < "3.8"',
-  "virtualenv>=20.21",
+  'typing-extensions>=4.6.2; python_version < "3.8"',
+  "virtualenv>=20.23",
 ]
 optional-dependencies.docs = [
-  "furo>=2023.3.27",
-  "sphinx>=6.1.3",
+  "furo>=2023.5.20",
+  "sphinx>=7.0.1",
   "sphinx-argparse-cli>=1.11",
   "sphinx-autodoc-typehints!=1.23.4,>=1.23",
   "sphinx-copybutton>=0.5.2",
-  "sphinx-inline-tabs>=2022.1.2b11",
+  "sphinx-inline-tabs>=2023.4.21",
   "sphinxcontrib-towncrier>=0.2.1a0",
   "towncrier>=22.12",
 ]
 optional-dependencies.testing = [
   "build[virtualenv]>=0.10",
   "covdefaults>=2.3",
   "devpi-process>=0.3",
   "diff-cover>=7.5",
   "distlib>=0.3.6",
   "flaky>=3.7",
   "hatch-vcs>=0.3",
-  "hatchling>=1.14",
-  "psutil>=5.9.4",
+  "hatchling>=1.17",
+  "psutil>=5.9.5",
   "pytest>=7.3.1",
-  "pytest-cov>=4",
+  "pytest-cov>=4.1",
   "pytest-mock>=3.10",
-  "pytest-xdist>=3.2.1",
+  "pytest-xdist>=3.3.1",
   "re-assert>=1.1",
   'time-machine>=2.9; implementation_name != "pypy"',
   "wheel>=0.40",
 ]
 urls.Documentation = "https://tox.wiki"
 urls.Homepage = "http://tox.readthedocs.org"
 urls."Release Notes" = "https://tox.wiki/en/latest/changelog.html"
```

### Comparing `tox-4.5.1/PKG-INFO` & `tox-4.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox
-Version: 4.5.1
+Version: 4.5.2
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, http://tox.readthedocs.org
 Project-URL: Release Notes, https://tox.wiki/en/latest/changelog.html
 Project-URL: Source, https://github.com/tox-dev/tox
 Project-URL: Tracker, https://github.com/tox-dev/tox/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -29,45 +29,45 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Requires-Dist: cachetools>=5.3
 Requires-Dist: chardet>=5.1
 Requires-Dist: colorama>=0.4.6
-Requires-Dist: filelock>=3.11
-Requires-Dist: importlib-metadata>=6.4.1; python_version < '3.8'
+Requires-Dist: filelock>=3.12
+Requires-Dist: importlib-metadata>=6.6; python_version < '3.8'
 Requires-Dist: packaging>=23.1
-Requires-Dist: platformdirs>=3.2
+Requires-Dist: platformdirs>=3.5.1
 Requires-Dist: pluggy>=1
 Requires-Dist: pyproject-api>=1.5.1
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
-Requires-Dist: typing-extensions>=4.5; python_version < '3.8'
-Requires-Dist: virtualenv>=20.21
+Requires-Dist: typing-extensions>=4.6.2; python_version < '3.8'
+Requires-Dist: virtualenv>=20.23
 Provides-Extra: docs
-Requires-Dist: furo>=2023.3.27; extra == 'docs'
+Requires-Dist: furo>=2023.5.20; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.11; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
-Requires-Dist: sphinx-inline-tabs>=2022.1.2b11; extra == 'docs'
-Requires-Dist: sphinx>=6.1.3; extra == 'docs'
+Requires-Dist: sphinx-inline-tabs>=2023.4.21; extra == 'docs'
+Requires-Dist: sphinx>=7.0.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-towncrier>=0.2.1a0; extra == 'docs'
 Requires-Dist: towncrier>=22.12; extra == 'docs'
 Provides-Extra: testing
 Requires-Dist: build[virtualenv]>=0.10; extra == 'testing'
 Requires-Dist: covdefaults>=2.3; extra == 'testing'
 Requires-Dist: devpi-process>=0.3; extra == 'testing'
 Requires-Dist: diff-cover>=7.5; extra == 'testing'
 Requires-Dist: distlib>=0.3.6; extra == 'testing'
 Requires-Dist: flaky>=3.7; extra == 'testing'
 Requires-Dist: hatch-vcs>=0.3; extra == 'testing'
-Requires-Dist: hatchling>=1.14; extra == 'testing'
-Requires-Dist: psutil>=5.9.4; extra == 'testing'
-Requires-Dist: pytest-cov>=4; extra == 'testing'
+Requires-Dist: hatchling>=1.17; extra == 'testing'
+Requires-Dist: psutil>=5.9.5; extra == 'testing'
+Requires-Dist: pytest-cov>=4.1; extra == 'testing'
 Requires-Dist: pytest-mock>=3.10; extra == 'testing'
-Requires-Dist: pytest-xdist>=3.2.1; extra == 'testing'
+Requires-Dist: pytest-xdist>=3.3.1; extra == 'testing'
 Requires-Dist: pytest>=7.3.1; extra == 'testing'
 Requires-Dist: re-assert>=1.1; extra == 'testing'
 Requires-Dist: time-machine>=2.9; implementation_name != 'pypy' and extra == 'testing'
 Requires-Dist: wheel>=0.40; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # tox
```

