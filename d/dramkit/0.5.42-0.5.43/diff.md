# Comparing `tmp/dramkit-0.5.42.tar.gz` & `tmp/dramkit-0.5.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramkit-0.5.42.tar", last modified: Sun May 21 02:55:36 2023, max compression
+gzip compressed data, was "dramkit-0.5.43.tar", last modified: Sun May 28 15:44:56 2023, max compression
```

## Comparing `dramkit-0.5.42.tar` & `dramkit-0.5.43.tar`

### file list

```diff
@@ -1,188 +1,190 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.663125 dramkit-0.5.42/
--rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.42/LICENSE
--rw-rw-rw-   0        0        0     1095 2023-05-21 02:55:36.663125 dramkit-0.5.42/PKG-INFO
--rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.42/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.505541 dramkit-0.5.42/dramkit/
--rw-rw-rw-   0        0        0      999 2023-04-24 03:43:26.000000 dramkit-0.5.42/dramkit/__init__.py
--rw-rw-rw-   0        0        0      662 2023-05-16 01:56:43.000000 dramkit-0.5.42/dramkit/_pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.552417 dramkit-0.5.42/dramkit/_tmp/
--rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/CRR.py
--rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.42/dramkit/_tmp/CtrlPreTS.py
--rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.42/dramkit/_tmp/NPairSum.py
--rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/PIDtest.py
--rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/PIDtest2.py
--rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/VMD.py
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/__init__.py
--rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/cca_test.py
--rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/dtw_test.py
--rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/explore.py
--rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/gini.py
--rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/merge_sort.py
--rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/mouse_move.py
--rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/mpc_test1.py
--rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/options_Implied_volatility.py
--rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/pf_test.py
--rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/plot_test.py
--rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.42/dramkit/_tmp/plot_test2.py
--rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.42/dramkit/_tmp/simple_smooth.py
--rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.42/dramkit/_tmp/test_async_washs.py
--rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.42/dramkit/_tmp/test_await_timeout.py
--rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/test_backtrader.py
--rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.42/dramkit/_tmp/test_chatgpt_v1.py
--rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/test_code.py
--rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.42/dramkit/_tmp/test_find_peaks.py
--rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.42/dramkit/_tmp/test_get_var_name.py
--rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.42/dramkit/_tmp/test_grading.py
--rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/test_lr.py
--rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.42/dramkit/_tmp/test_maxsort.py
--rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.42/dramkit/_tmp/test_multiprocessing.py
--rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.42/dramkit/_tmp/test_ocr.py
--rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.42/dramkit/_tmp/test_pywechat.py
--rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.42/dramkit/_tmp/test_tree.py
--rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.42/dramkit/_tmp/test_tree2.py
--rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.42/dramkit/_tmp/test_wechat_work.py
--rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/tfDNNCls_test.py
--rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/tmp.py
--rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.42/dramkit/_tmp/tmp_args.py
--rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/transformer_pytorch.py
--rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.42/dramkit/_tmp/utils_SignalDec.py
--rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.42/dramkit/_tmp/utils_TimeSeries.py
--rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.42/dramkit/_tmp/utils_lottery.py
--rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl.py
--rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl2.py
--rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl3.py
--rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl4.py
--rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl5.py
--rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl6.py
--rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl7.py
--rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_sem.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.555408 dramkit-0.5.42/dramkit/backpacks/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/backpacks/__init__.py
--rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.42/dramkit/backpacks/backpack01_float_dy.py
--rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.42/dramkit/backpacks/backpack01_int_dy.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.581339 dramkit-0.5.42/dramkit/chncal/
--rw-rw-rw-   0        0        0      730 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/__init__.py
--rw-rw-rw-   0        0        0    21188 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/apis.py
--rw-rw-rw-   0        0        0    69806 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants.py
--rw-rw-rw-   0        0        0     8480 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_fate.py
--rw-rw-rw-   0        0        0  9509384 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_hko.py
--rw-rw-rw-   0        0        0  3961724 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_trade_dates.py
--rw-rw-rw-   0        0        0     2501 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_wuxing.py
--rw-rw-rw-   0        0        0     8342 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_zodiac_marry.py
--rw-rw-rw-   0        0        0     4570 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/solar_terms.py
--rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.42/dramkit/cryptotools.py
--rw-rw-rw-   0        0        0    34826 2023-05-20 15:37:28.000000 dramkit-0.5.42/dramkit/datetimetools.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.601290 dramkit-0.5.42/dramkit/datsci/
--rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.42/dramkit/datsci/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.42/dramkit/datsci/_utils_ann.py
--rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.42/dramkit/datsci/activate_funcs.py
--rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.42/dramkit/datsci/ahp.py
--rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.42/dramkit/datsci/ahp_sim_ri.py
--rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.42/dramkit/datsci/apriori.py
--rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.42/dramkit/datsci/curvature.py
--rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.42/dramkit/datsci/elm_cls.py
--rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.42/dramkit/datsci/elm_reg.py
--rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.42/dramkit/datsci/entropy_weight.py
--rw-rw-rw-   0        0        0    50084 2023-05-10 02:47:36.000000 dramkit-0.5.42/dramkit/datsci/find_maxmin.py
--rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.42/dramkit/datsci/freq_item_set.py
--rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.42/dramkit/datsci/lr.py
--rw-rw-rw-   0        0        0    20288 2023-05-19 06:29:01.000000 dramkit-0.5.42/dramkit/datsci/preprocess.py
--rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.42/dramkit/datsci/stats.py
--rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.42/dramkit/datsci/time_series.py
--rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.42/dramkit/datsci/topsis.py
--rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.42/dramkit/datsci/utils_lgb.py
--rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.42/dramkit/datsci/utils_ml.py
--rw-rw-rw-   0        0        0    21037 2023-05-11 01:05:22.000000 dramkit-0.5.42/dramkit/datsci/zigzag.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.609269 dramkit-0.5.42/dramkit/find_addends/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/find_addends/__init__.py
--rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_backpack01float.py
--rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_backpack01int.py
--rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_bigfirst.py
--rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_recu.py
--rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_smlfirst.py
--rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_utils.py
--rw-rw-rw-   0        0        0   125549 2023-05-20 16:49:14.000000 dramkit-0.5.42/dramkit/gentools.py
--rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.42/dramkit/install_check.py
--rw-rw-rw-   0        0        0    67350 2023-05-19 01:46:24.000000 dramkit-0.5.42/dramkit/iotools.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.612261 dramkit-0.5.42/dramkit/logtools/
--rw-rw-rw-   0        0        0      139 2023-05-01 07:34:20.000000 dramkit-0.5.42/dramkit/logtools/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.42/dramkit/logtools/logger_general.py
--rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.42/dramkit/logtools/logger_rotating.py
--rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.42/dramkit/logtools/logger_timedrotating.py
--rw-rw-rw-   0        0        0     4214 2023-02-28 10:31:30.000000 dramkit-0.5.42/dramkit/logtools/utils_logger.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.615253 dramkit-0.5.42/dramkit/openai/
--rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.42/dramkit/openai/__init__.py
--rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.42/dramkit/openai/aiedu_chat.py
--rw-rw-rw-   0        0        0    16999 2023-05-08 02:26:05.000000 dramkit-0.5.42/dramkit/openai/openai_chat.py
--rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.42/dramkit/openai/openai_chat_hs.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.627221 dramkit-0.5.42/dramkit/optimizer/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/optimizer/__init__.py
--rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.42/dramkit/optimizer/alo.py
--rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.42/dramkit/optimizer/base_funcs.py
--rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.42/dramkit/optimizer/boa.py
--rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.42/dramkit/optimizer/cs.py
--rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.42/dramkit/optimizer/ga.py
--rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.42/dramkit/optimizer/gwo.py
--rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.42/dramkit/optimizer/hcpsoboa.py
--rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.42/dramkit/optimizer/hho.py
--rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.42/dramkit/optimizer/hpsoboa.py
--rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.42/dramkit/optimizer/pso.py
--rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.42/dramkit/optimizer/utils_heuristic.py
--rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.42/dramkit/optimizer/woa.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.634202 dramkit-0.5.42/dramkit/other/
--rw-rw-rw-   0        0        0     3856 2023-04-30 10:22:45.000000 dramkit-0.5.42/dramkit/other/_Linux_notes.py
--rw-rw-rw-   0        0        0     2947 2023-05-17 06:10:10.000000 dramkit-0.5.42/dramkit/other/_Python_notes.py
--rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.42/dramkit/other/_Vim_notes.py
--rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.42/dramkit/other/__init__.py
--rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.42/dramkit/other/langconv.py
--rw-rw-rw-   0        0        0     8353 2022-12-10 15:26:10.000000 dramkit-0.5.42/dramkit/other/othertools.py
--rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.42/dramkit/other/replace_endblank.py
--rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.42/dramkit/other/zh_wiki.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.640186 dramkit-0.5.42/dramkit/plottools/
--rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.42/dramkit/plottools/__init__.py
--rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.42/dramkit/plottools/plot_barline.py
--rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.42/dramkit/plottools/plot_common.py
--rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.42/dramkit/plottools/plot_histdist.py
--rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.42/dramkit/plottools/plot_scatter.py
--rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.42/dramkit/plottools/utils_plot.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.641183 dramkit-0.5.42/dramkit/pystyles/
--rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.42/dramkit/pystyles/__init__.py
--rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.42/dramkit/pystyles/dramkit_style.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.645169 dramkit-0.5.42/dramkit/sorts/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/sorts/__init__.py
--rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.42/dramkit/sorts/bubble_sort.py
--rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.42/dramkit/sorts/bucket_sort.py
--rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.42/dramkit/sorts/insert_sort.py
--rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.42/dramkit/sorts/insert_sort_bin.py
--rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.42/dramkit/sorts/quick_sort.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.652150 dramkit-0.5.42/dramkit/speedup/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/speedup/__init__.py
--rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.42/dramkit/speedup/_mp_test1.py
--rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.42/dramkit/speedup/_mp_test2.py
--rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.42/dramkit/speedup/_mp_test3.py
--rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.42/dramkit/speedup/iotools_tmp.py
--rw-rw-rw-   0        0        0     3754 2023-04-12 08:17:22.000000 dramkit-0.5.42/dramkit/speedup/multi_process_concurrent.py
--rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.42/dramkit/speedup/multi_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.659136 dramkit-0.5.42/dramkit/sqltools/
--rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.42/dramkit/sqltools/_Hive_notes.py
--rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.42/dramkit/sqltools/_MySQL_notes.py
--rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.42/dramkit/sqltools/_Oracle_notes.py
--rw-rw-rw-   0        0        0      160 2023-05-01 12:57:19.000000 dramkit-0.5.42/dramkit/sqltools/__init__.py
--rw-rw-rw-   0        0        0    20285 2023-05-06 13:49:07.000000 dramkit-0.5.42/dramkit/sqltools/cxoracle.py
--rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.42/dramkit/sqltools/py_hive.py
--rw-rw-rw-   0        0        0    50966 2023-05-06 13:23:21.000000 dramkit-0.5.42/dramkit/sqltools/py_mysql.py
--rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.42/dramkit/sqltools/sql_alchemy.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.660132 dramkit-0.5.42/dramkit/webtools/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/webtools/__init__.py
--rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.5.42/dramkit/webtools/utils_html.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.662123 dramkit-0.5.42/dramkit/wechat/
--rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.42/dramkit/wechat/__init__.py
--rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.42/dramkit/wechat/qywechat.py
-drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.510533 dramkit-0.5.42/dramkit.egg-info/
--rw-rw-rw-   0        0        0     1095 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4877 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 02:55:36.663125 dramkit-0.5.42/setup.cfg
--rw-rw-rw-   0        0        0     1944 2023-05-01 12:58:33.000000 dramkit-0.5.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.441200 dramkit-0.5.43/
+-rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.43/LICENSE
+-rw-rw-rw-   0        0        0     1095 2023-05-28 15:44:56.440202 dramkit-0.5.43/PKG-INFO
+-rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.43/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.315493 dramkit-0.5.43/dramkit/
+-rw-rw-rw-   0        0        0     1017 2023-05-23 01:38:43.000000 dramkit-0.5.43/dramkit/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-05-26 02:30:22.000000 dramkit-0.5.43/dramkit/_pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.355387 dramkit-0.5.43/dramkit/_tmp/
+-rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/CRR.py
+-rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.43/dramkit/_tmp/CtrlPreTS.py
+-rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.43/dramkit/_tmp/NPairSum.py
+-rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/PIDtest.py
+-rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/PIDtest2.py
+-rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/VMD.py
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/__init__.py
+-rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/cca_test.py
+-rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/dtw_test.py
+-rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/explore.py
+-rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/gini.py
+-rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/merge_sort.py
+-rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/mouse_move.py
+-rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/mpc_test1.py
+-rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/options_Implied_volatility.py
+-rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/pf_test.py
+-rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/plot_test.py
+-rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.43/dramkit/_tmp/plot_test2.py
+-rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.43/dramkit/_tmp/simple_smooth.py
+-rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.43/dramkit/_tmp/test_async_washs.py
+-rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.43/dramkit/_tmp/test_await_timeout.py
+-rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/test_backtrader.py
+-rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.43/dramkit/_tmp/test_chatgpt_v1.py
+-rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/test_code.py
+-rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.43/dramkit/_tmp/test_find_peaks.py
+-rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.43/dramkit/_tmp/test_get_var_name.py
+-rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.43/dramkit/_tmp/test_grading.py
+-rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/test_lr.py
+-rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.43/dramkit/_tmp/test_maxsort.py
+-rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.43/dramkit/_tmp/test_multiprocessing.py
+-rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.43/dramkit/_tmp/test_ocr.py
+-rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.43/dramkit/_tmp/test_pywechat.py
+-rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.43/dramkit/_tmp/test_tree.py
+-rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.43/dramkit/_tmp/test_tree2.py
+-rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.43/dramkit/_tmp/test_wechat_work.py
+-rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/tfDNNCls_test.py
+-rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/tmp.py
+-rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.43/dramkit/_tmp/tmp_args.py
+-rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/transformer_pytorch.py
+-rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.43/dramkit/_tmp/utils_SignalDec.py
+-rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.43/dramkit/_tmp/utils_TimeSeries.py
+-rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.43/dramkit/_tmp/utils_lottery.py
+-rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/utils_rl.py
+-rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/utils_rl2.py
+-rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/utils_rl3.py
+-rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/utils_rl4.py
+-rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/utils_rl5.py
+-rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/utils_rl6.py
+-rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/utils_rl7.py
+-rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/_tmp/utils_sem.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.359382 dramkit-0.5.43/dramkit/backpacks/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/backpacks/__init__.py
+-rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.43/dramkit/backpacks/backpack01_float_dy.py
+-rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.43/dramkit/backpacks/backpack01_int_dy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.379365 dramkit-0.5.43/dramkit/chncal/
+-rw-rw-rw-   0        0        0      730 2023-05-22 15:05:56.000000 dramkit-0.5.43/dramkit/chncal/__init__.py
+-rw-rw-rw-   0        0        0    21188 2023-05-22 15:05:56.000000 dramkit-0.5.43/dramkit/chncal/apis.py
+-rw-rw-rw-   0        0        0    69806 2023-05-22 15:05:56.000000 dramkit-0.5.43/dramkit/chncal/constants.py
+-rw-rw-rw-   0        0        0     8480 2023-05-22 15:05:56.000000 dramkit-0.5.43/dramkit/chncal/constants_fate.py
+-rw-rw-rw-   0        0        0  9509384 2023-05-22 15:05:56.000000 dramkit-0.5.43/dramkit/chncal/constants_hko.py
+-rw-rw-rw-   0        0        0  3962978 2023-05-22 15:05:56.000000 dramkit-0.5.43/dramkit/chncal/constants_trade_dates.py
+-rw-rw-rw-   0        0        0     2501 2023-05-22 15:05:56.000000 dramkit-0.5.43/dramkit/chncal/constants_wuxing.py
+-rw-rw-rw-   0        0        0     8342 2023-05-22 15:05:56.000000 dramkit-0.5.43/dramkit/chncal/constants_zodiac_marry.py
+-rw-rw-rw-   0        0        0     4570 2023-05-22 15:05:56.000000 dramkit-0.5.43/dramkit/chncal/solar_terms.py
+-rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.43/dramkit/cryptotools.py
+-rw-rw-rw-   0        0        0    34826 2023-05-20 15:37:28.000000 dramkit-0.5.43/dramkit/datetimetools.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.392332 dramkit-0.5.43/dramkit/datsci/
+-rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.43/dramkit/datsci/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.43/dramkit/datsci/_utils_ann.py
+-rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.43/dramkit/datsci/activate_funcs.py
+-rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.43/dramkit/datsci/ahp.py
+-rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.43/dramkit/datsci/ahp_sim_ri.py
+-rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.43/dramkit/datsci/apriori.py
+-rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.43/dramkit/datsci/curvature.py
+-rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.43/dramkit/datsci/elm_cls.py
+-rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.43/dramkit/datsci/elm_reg.py
+-rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.43/dramkit/datsci/entropy_weight.py
+-rw-rw-rw-   0        0        0    50084 2023-05-10 02:47:36.000000 dramkit-0.5.43/dramkit/datsci/find_maxmin.py
+-rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.43/dramkit/datsci/freq_item_set.py
+-rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.43/dramkit/datsci/lr.py
+-rw-rw-rw-   0        0        0    20288 2023-05-19 06:29:01.000000 dramkit-0.5.43/dramkit/datsci/preprocess.py
+-rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.43/dramkit/datsci/stats.py
+-rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.43/dramkit/datsci/time_series.py
+-rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.43/dramkit/datsci/topsis.py
+-rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.43/dramkit/datsci/utils_lgb.py
+-rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.43/dramkit/datsci/utils_ml.py
+-rw-rw-rw-   0        0        0    21136 2023-05-21 10:05:57.000000 dramkit-0.5.43/dramkit/datsci/zigzag.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.396324 dramkit-0.5.43/dramkit/find_addends/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/find_addends/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.43/dramkit/find_addends/find_addends_backpack01float.py
+-rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.43/dramkit/find_addends/find_addends_backpack01int.py
+-rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.43/dramkit/find_addends/find_addends_bigfirst.py
+-rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.43/dramkit/find_addends/find_addends_recu.py
+-rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.43/dramkit/find_addends/find_addends_smlfirst.py
+-rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.43/dramkit/find_addends/find_addends_utils.py
+-rw-rw-rw-   0        0        0   127908 2023-05-24 02:23:16.000000 dramkit-0.5.43/dramkit/gentools.py
+-rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.43/dramkit/install_check.py
+-rw-rw-rw-   0        0        0    67350 2023-05-19 01:46:24.000000 dramkit-0.5.43/dramkit/iotools.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.399312 dramkit-0.5.43/dramkit/logtools/
+-rw-rw-rw-   0        0        0      139 2023-05-01 07:34:20.000000 dramkit-0.5.43/dramkit/logtools/__init__.py
+-rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.43/dramkit/logtools/logger_general.py
+-rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.43/dramkit/logtools/logger_rotating.py
+-rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.43/dramkit/logtools/logger_timedrotating.py
+-rw-rw-rw-   0        0        0     4494 2023-05-24 02:19:43.000000 dramkit-0.5.43/dramkit/logtools/utils_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.401306 dramkit-0.5.43/dramkit/openai/
+-rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.43/dramkit/openai/__init__.py
+-rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.43/dramkit/openai/aiedu_chat.py
+-rw-rw-rw-   0        0        0    16999 2023-05-08 02:26:05.000000 dramkit-0.5.43/dramkit/openai/openai_chat.py
+-rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.43/dramkit/openai/openai_chat_hs.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.411284 dramkit-0.5.43/dramkit/optimizer/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.43/dramkit/optimizer/alo.py
+-rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.43/dramkit/optimizer/base_funcs.py
+-rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.43/dramkit/optimizer/boa.py
+-rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.43/dramkit/optimizer/cs.py
+-rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.43/dramkit/optimizer/ga.py
+-rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.43/dramkit/optimizer/gwo.py
+-rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.43/dramkit/optimizer/hcpsoboa.py
+-rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.43/dramkit/optimizer/hho.py
+-rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.43/dramkit/optimizer/hpsoboa.py
+-rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.43/dramkit/optimizer/pso.py
+-rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.43/dramkit/optimizer/utils_heuristic.py
+-rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.43/dramkit/optimizer/woa.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.416266 dramkit-0.5.43/dramkit/other/
+-rw-rw-rw-   0        0        0      831 2023-05-21 07:44:53.000000 dramkit-0.5.43/dramkit/other/_Git_notes.py
+-rw-rw-rw-   0        0        0     3856 2023-04-30 10:22:45.000000 dramkit-0.5.43/dramkit/other/_Linux_notes.py
+-rw-rw-rw-   0        0        0     2947 2023-05-17 06:10:10.000000 dramkit-0.5.43/dramkit/other/_Python_notes.py
+-rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.43/dramkit/other/_Vim_notes.py
+-rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.43/dramkit/other/__init__.py
+-rw-rw-rw-   0        0        0     6013 2023-05-27 15:36:26.000000 dramkit-0.5.43/dramkit/other/debt_cal.py
+-rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.43/dramkit/other/langconv.py
+-rw-rw-rw-   0        0        0     8757 2023-05-21 07:05:41.000000 dramkit-0.5.43/dramkit/other/othertools.py
+-rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.43/dramkit/other/replace_endblank.py
+-rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.43/dramkit/other/zh_wiki.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.420260 dramkit-0.5.43/dramkit/plottools/
+-rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.43/dramkit/plottools/__init__.py
+-rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.43/dramkit/plottools/plot_barline.py
+-rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.43/dramkit/plottools/plot_common.py
+-rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.43/dramkit/plottools/plot_histdist.py
+-rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.43/dramkit/plottools/plot_scatter.py
+-rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.43/dramkit/plottools/utils_plot.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.423248 dramkit-0.5.43/dramkit/pystyles/
+-rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.43/dramkit/pystyles/__init__.py
+-rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.43/dramkit/pystyles/dramkit_style.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.426244 dramkit-0.5.43/dramkit/sorts/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/sorts/__init__.py
+-rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.43/dramkit/sorts/bubble_sort.py
+-rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.43/dramkit/sorts/bucket_sort.py
+-rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.43/dramkit/sorts/insert_sort.py
+-rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.43/dramkit/sorts/insert_sort_bin.py
+-rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.43/dramkit/sorts/quick_sort.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.430235 dramkit-0.5.43/dramkit/speedup/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/speedup/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.43/dramkit/speedup/_mp_test1.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.43/dramkit/speedup/_mp_test2.py
+-rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.43/dramkit/speedup/_mp_test3.py
+-rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.43/dramkit/speedup/iotools_tmp.py
+-rw-rw-rw-   0        0        0     3754 2023-04-12 08:17:22.000000 dramkit-0.5.43/dramkit/speedup/multi_process_concurrent.py
+-rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.43/dramkit/speedup/multi_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.435215 dramkit-0.5.43/dramkit/sqltools/
+-rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.43/dramkit/sqltools/_Hive_notes.py
+-rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.43/dramkit/sqltools/_MySQL_notes.py
+-rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.43/dramkit/sqltools/_Oracle_notes.py
+-rw-rw-rw-   0        0        0      160 2023-05-01 12:57:19.000000 dramkit-0.5.43/dramkit/sqltools/__init__.py
+-rw-rw-rw-   0        0        0    20285 2023-05-06 13:49:07.000000 dramkit-0.5.43/dramkit/sqltools/cxoracle.py
+-rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.43/dramkit/sqltools/py_hive.py
+-rw-rw-rw-   0        0        0    50966 2023-05-06 13:23:21.000000 dramkit-0.5.43/dramkit/sqltools/py_mysql.py
+-rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.43/dramkit/sqltools/sql_alchemy.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.437210 dramkit-0.5.43/dramkit/webtools/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.43/dramkit/webtools/__init__.py
+-rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.5.43/dramkit/webtools/utils_html.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.439208 dramkit-0.5.43/dramkit/wechat/
+-rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.43/dramkit/wechat/__init__.py
+-rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.43/dramkit/wechat/qywechat.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:44:56.319483 dramkit-0.5.43/dramkit.egg-info/
+-rw-rw-rw-   0        0        0     1095 2023-05-28 15:44:56.000000 dramkit-0.5.43/dramkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4931 2023-05-28 15:44:56.000000 dramkit-0.5.43/dramkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 15:44:56.000000 dramkit-0.5.43/dramkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-28 15:44:56.000000 dramkit-0.5.43/dramkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 15:44:56.000000 dramkit-0.5.43/dramkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 15:44:56.441200 dramkit-0.5.43/setup.cfg
+-rw-rw-rw-   0        0        0     1944 2023-05-01 12:58:33.000000 dramkit-0.5.43/setup.py
```

### Comparing `dramkit-0.5.42/LICENSE` & `dramkit-0.5.43/LICENSE`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/PKG-INFO` & `dramkit-0.5.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.42
+Version: 0.5.43
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.42/README.md` & `dramkit-0.5.43/README.md`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/__init__.py` & `dramkit-0.5.43/dramkit/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 from .plottools import plot_series
 from .plottools import plot_series_conlabel
 
 from .logtools.utils_logger import logger_show, close_log_file
 from .logtools.logger_general import get_logger as simple_logger
 
-from . import gentools
-from . import iotools
-from . import cryptotools
-from . import datetimetools as dttools
-from .datsci import find_maxmin
-from .openai import openai_chat
-from .other import othertools
-from .speedup import multi_thread, multi_process_concurrent
-from .sqltools import py_mysql
+# from . import gentools
+# from . import iotools
+# from . import cryptotools
+# from . import datetimetools as dttools
+# from .datsci import find_maxmin
+# from .openai import openai_chat
+# from .other import othertools
+# from .speedup import multi_thread, multi_process_concurrent
+# from .sqltools import py_mysql
```

### Comparing `dramkit-0.5.42/dramkit/_pkg_info.py` & `dramkit-0.5.43/dramkit/_pkg_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pkg_info = {
     '__pkgname__': 'dramkit',
-    '__version__': '0.5.42',
+    '__version__': '0.5.43',
     '__license__': 'MIT',
     '__url__': 'https://github.com/Genlovy-Hoo/dramkit/',
     '__urls__':
         {'pypi': 'https://pypi.org/project/dramkit/',
          'github': 'https://github.com/Genlovy-Hoo/dramkit/',
 		 'document': 'http://www.glhyy.cn/dramkit/doc/html/index.html'
         },
```

### Comparing `dramkit-0.5.42/dramkit/_tmp/CRR.py` & `dramkit-0.5.43/dramkit/_tmp/CRR.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/CtrlPreTS.py` & `dramkit-0.5.43/dramkit/_tmp/CtrlPreTS.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/NPairSum.py` & `dramkit-0.5.43/dramkit/_tmp/NPairSum.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/PIDtest.py` & `dramkit-0.5.43/dramkit/_tmp/PIDtest.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/PIDtest2.py` & `dramkit-0.5.43/dramkit/_tmp/PIDtest2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/VMD.py` & `dramkit-0.5.43/dramkit/_tmp/VMD.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/cca_test.py` & `dramkit-0.5.43/dramkit/_tmp/cca_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/dtw_test.py` & `dramkit-0.5.43/dramkit/_tmp/dtw_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/explore.py` & `dramkit-0.5.43/dramkit/_tmp/explore.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/gini.py` & `dramkit-0.5.43/dramkit/_tmp/gini.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/merge_sort.py` & `dramkit-0.5.43/dramkit/_tmp/merge_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/mouse_move.py` & `dramkit-0.5.43/dramkit/_tmp/mouse_move.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/mpc_test1.py` & `dramkit-0.5.43/dramkit/_tmp/mpc_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/options_Implied_volatility.py` & `dramkit-0.5.43/dramkit/_tmp/options_Implied_volatility.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/plot_test.py` & `dramkit-0.5.43/dramkit/_tmp/plot_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/plot_test2.py` & `dramkit-0.5.43/dramkit/_tmp/plot_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/simple_smooth.py` & `dramkit-0.5.43/dramkit/_tmp/simple_smooth.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_async_washs.py` & `dramkit-0.5.43/dramkit/_tmp/test_async_washs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_await_timeout.py` & `dramkit-0.5.43/dramkit/_tmp/test_await_timeout.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_backtrader.py` & `dramkit-0.5.43/dramkit/_tmp/test_backtrader.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_chatgpt_v1.py` & `dramkit-0.5.43/dramkit/_tmp/test_chatgpt_v1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_code.py` & `dramkit-0.5.43/dramkit/_tmp/test_code.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_find_peaks.py` & `dramkit-0.5.43/dramkit/_tmp/test_find_peaks.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_get_var_name.py` & `dramkit-0.5.43/dramkit/_tmp/test_get_var_name.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_grading.py` & `dramkit-0.5.43/dramkit/_tmp/test_grading.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_lr.py` & `dramkit-0.5.43/dramkit/_tmp/test_lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_maxsort.py` & `dramkit-0.5.43/dramkit/_tmp/test_maxsort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_pywechat.py` & `dramkit-0.5.43/dramkit/_tmp/test_pywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_tree.py` & `dramkit-0.5.43/dramkit/_tmp/test_tree.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_tree2.py` & `dramkit-0.5.43/dramkit/_tmp/test_tree2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/test_wechat_work.py` & `dramkit-0.5.43/dramkit/_tmp/test_wechat_work.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/tfDNNCls_test.py` & `dramkit-0.5.43/dramkit/_tmp/tfDNNCls_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/tmp.py` & `dramkit-0.5.43/dramkit/_tmp/tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/tmp_args.py` & `dramkit-0.5.43/dramkit/_tmp/tmp_args.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/transformer_pytorch.py` & `dramkit-0.5.43/dramkit/_tmp/transformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_SignalDec.py` & `dramkit-0.5.43/dramkit/_tmp/utils_SignalDec.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_TimeSeries.py` & `dramkit-0.5.43/dramkit/_tmp/utils_TimeSeries.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_lottery.py` & `dramkit-0.5.43/dramkit/_tmp/utils_lottery.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_rl.py` & `dramkit-0.5.43/dramkit/_tmp/utils_rl.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_rl2.py` & `dramkit-0.5.43/dramkit/_tmp/utils_rl2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_rl3.py` & `dramkit-0.5.43/dramkit/_tmp/utils_rl3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_rl4.py` & `dramkit-0.5.43/dramkit/_tmp/utils_rl4.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_rl5.py` & `dramkit-0.5.43/dramkit/_tmp/utils_rl5.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_rl6.py` & `dramkit-0.5.43/dramkit/_tmp/utils_rl6.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_rl7.py` & `dramkit-0.5.43/dramkit/_tmp/utils_rl7.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/_tmp/utils_sem.py` & `dramkit-0.5.43/dramkit/_tmp/utils_sem.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/backpacks/backpack01_float_dy.py` & `dramkit-0.5.43/dramkit/backpacks/backpack01_float_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/backpacks/backpack01_int_dy.py` & `dramkit-0.5.43/dramkit/backpacks/backpack01_int_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/chncal/__init__.py` & `dramkit-0.5.43/dramkit/chncal/__init__.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/chncal/apis.py` & `dramkit-0.5.43/dramkit/chncal/apis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/chncal/constants.py` & `dramkit-0.5.43/dramkit/chncal/constants.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/chncal/constants_fate.py` & `dramkit-0.5.43/dramkit/chncal/constants_fate.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/chncal/constants_hko.py` & `dramkit-0.5.43/dramkit/chncal/constants_hko.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/chncal/constants_trade_dates.py` & `dramkit-0.5.43/dramkit/chncal/constants_trade_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6101,14 +6101,17 @@
     ("CFFEX", datetime.date(year=2023, month=5, day=13)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=14)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=15)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=16)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=17)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=18)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=19)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=20)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=21)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=22)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=13)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=14)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=15)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=16)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=17)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=18)): 1,
@@ -18008,14 +18011,17 @@
     ("CZCE", datetime.date(year=2023, month=5, day=13)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=14)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=15)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=16)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=17)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=18)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=19)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=20)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=21)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=22)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=1)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=2)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=3)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=4)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=5)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=6)): 0,
     ("DCE", datetime.date(year=1993, month=3, day=7)): 0,
@@ -29044,14 +29050,17 @@
     ("DCE", datetime.date(year=2023, month=5, day=13)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=14)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=15)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=16)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=17)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=18)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=19)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=20)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=21)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=22)): 1,
     ("INE", datetime.date(year=2017, month=5, day=23)): 1,
     ("INE", datetime.date(year=2017, month=5, day=24)): 1,
     ("INE", datetime.date(year=2017, month=5, day=25)): 1,
     ("INE", datetime.date(year=2017, month=5, day=26)): 1,
     ("INE", datetime.date(year=2017, month=5, day=27)): 0,
     ("INE", datetime.date(year=2017, month=5, day=28)): 0,
     ("INE", datetime.date(year=2017, month=5, day=29)): 0,
@@ -31231,14 +31240,17 @@
     ("INE", datetime.date(year=2023, month=5, day=13)): 0,
     ("INE", datetime.date(year=2023, month=5, day=14)): 0,
     ("INE", datetime.date(year=2023, month=5, day=15)): 1,
     ("INE", datetime.date(year=2023, month=5, day=16)): 1,
     ("INE", datetime.date(year=2023, month=5, day=17)): 1,
     ("INE", datetime.date(year=2023, month=5, day=18)): 1,
     ("INE", datetime.date(year=2023, month=5, day=19)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=20)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=21)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=22)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=28)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=29)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=30)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=31)): 1,
     ("SHFE", datetime.date(year=1991, month=6, day=1)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=2)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=3)): 1,
@@ -42910,14 +42922,17 @@
     ("SHFE", datetime.date(year=2023, month=5, day=13)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=14)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=15)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=16)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=17)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=18)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=19)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=20)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=21)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=22)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=19)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=20)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=21)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=22)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=23)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=24)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=25)): 1,
@@ -54750,14 +54765,17 @@
     ("SSE", datetime.date(year=2023, month=5, day=13)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=14)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=15)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=16)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=17)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=18)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=19)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=20)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=21)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=22)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=3)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=4)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=5)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=6)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=7)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=8)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=9)): 1,
@@ -66394,8 +66412,11 @@
     ("SZSE", datetime.date(year=2023, month=5, day=13)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=14)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=15)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=16)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=17)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=18)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=19)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=20)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=21)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=22)): 1,
 }
```

### Comparing `dramkit-0.5.42/dramkit/chncal/constants_wuxing.py` & `dramkit-0.5.43/dramkit/chncal/constants_wuxing.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/chncal/constants_zodiac_marry.py` & `dramkit-0.5.43/dramkit/chncal/constants_zodiac_marry.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/chncal/solar_terms.py` & `dramkit-0.5.43/dramkit/chncal/solar_terms.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/cryptotools.py` & `dramkit-0.5.43/dramkit/cryptotools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datetimetools.py` & `dramkit-0.5.43/dramkit/datetimetools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/_utils_ann.py` & `dramkit-0.5.43/dramkit/datsci/_utils_ann.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/activate_funcs.py` & `dramkit-0.5.43/dramkit/datsci/activate_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/ahp.py` & `dramkit-0.5.43/dramkit/datsci/ahp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/ahp_sim_ri.py` & `dramkit-0.5.43/dramkit/datsci/ahp_sim_ri.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/apriori.py` & `dramkit-0.5.43/dramkit/datsci/apriori.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/curvature.py` & `dramkit-0.5.43/dramkit/datsci/curvature.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/elm_cls.py` & `dramkit-0.5.43/dramkit/datsci/elm_cls.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/elm_reg.py` & `dramkit-0.5.43/dramkit/datsci/elm_reg.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/entropy_weight.py` & `dramkit-0.5.43/dramkit/datsci/entropy_weight.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/find_maxmin.py` & `dramkit-0.5.43/dramkit/datsci/find_maxmin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/freq_item_set.py` & `dramkit-0.5.43/dramkit/datsci/freq_item_set.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/lr.py` & `dramkit-0.5.43/dramkit/datsci/lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/preprocess.py` & `dramkit-0.5.43/dramkit/datsci/preprocess.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/stats.py` & `dramkit-0.5.43/dramkit/datsci/stats.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/time_series.py` & `dramkit-0.5.43/dramkit/datsci/time_series.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/topsis.py` & `dramkit-0.5.43/dramkit/datsci/topsis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/utils_lgb.py` & `dramkit-0.5.43/dramkit/datsci/utils_lgb.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/utils_ml.py` & `dramkit-0.5.43/dramkit/datsci/utils_ml.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/datsci/zigzag.py` & `dramkit-0.5.43/dramkit/datsci/zigzag.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     up_min_val = min_val if isnull(up_min_val) else up_min_val
     up_max_pct = max_pct if isnull(up_max_pct) else up_max_pct
     up_max_val = max_val if isnull(up_max_val) else up_max_val
     down_min_pct = -1*min_pct if (isnull(down_min_pct) and not isnull(min_pct)) else down_min_pct
     down_min_val = -1*min_val if (isnull(down_min_val) and not isnull(min_val)) else down_min_val
     down_max_pct = -1*max_pct if (isnull(down_max_pct) and not isnull(max_pct)) else down_max_pct
     down_max_val = -1*max_val if (isnull(down_max_val) and not isnull(max_val)) else down_max_val
+    
     # 上涨-长时最小幅度参数
     assert not (isnull(up_min_pct) and isnull(up_min_val)), \
         '必须设置`up_min_pct`或`up_min_val`, 若要忽略此参数，可将其设置为负数'
     if not isnull(up_min_pct) and not isnull(up_min_val):
         logger_show('同时设置`up_min_pct`和`up_min_val`，以`up_min_pct`为准！',
                     logger, 'warn')
         up_min_val = None
@@ -441,15 +442,15 @@
         plot_candle(data, cols_other_upleft=cols_other_upleft,
                     cols_to_label_info=cols_to_label_info,
                     **kwargs)
     
     
     tr = TimeRecoder()
     
-    # '''
+    '''
     # 二次曲线叠加正弦余弦
     N = 200
     t = np.linspace(0, 1, N)
     s = 6*t*t + np.cos(10*2*np.pi*t*t) + np.sin(6*2*np.pi*t)
     df = pd.DataFrame(s, columns=['test'])
 
     # t_min = None
@@ -473,15 +474,15 @@
                     'test': [
                         ['zigzag', (-1, 1), ('r^', 'gv'), None]
                         ]},
                 figsize=(8, 3))
     # '''
 
 
-    # '''
+    '''
     fpath = '../_test/510050.SH_daily_qfq.csv'
     his_data = load_csv(fpath)
     his_data.rename(columns={'date': 'time'}, inplace=True)
     his_data.set_index('time', drop=False, inplace=True)
 
     # N = his_data.shape[0]
     N = 100
@@ -510,19 +511,23 @@
                    args_ma=None,
                    args_boll=None,
                    plot_below=None,
                    figsize=(10, 6))
     
     high_col, low_col = 'high', 'low'
     min_pct = -1/100
+    # min_pct = None
     t_min = 15
+    # t_min = None
+    min_val = None
     params = {'high_col': high_col,
               'low_col': low_col,
               'min_pct': min_pct,
-              't_min': t_min
+              't_min': t_min,
+              'min_val': min_val
               }    
     
     df['zigzag'] = zigzag(df, **params)
     plot_candle_zz(df,
                    args_ma=None,
                    # args_boll=[15, 2],
                    args_boll=None,
```

### Comparing `dramkit-0.5.42/dramkit/find_addends/find_addends_backpack01float.py` & `dramkit-0.5.43/dramkit/find_addends/find_addends_backpack01float.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/find_addends/find_addends_backpack01int.py` & `dramkit-0.5.43/dramkit/find_addends/find_addends_backpack01int.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/find_addends/find_addends_bigfirst.py` & `dramkit-0.5.43/dramkit/find_addends/find_addends_bigfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/find_addends/find_addends_recu.py` & `dramkit-0.5.43/dramkit/find_addends/find_addends_recu.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/find_addends/find_addends_smlfirst.py` & `dramkit-0.5.43/dramkit/find_addends/find_addends_smlfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/find_addends/find_addends_utils.py` & `dramkit-0.5.43/dramkit/find_addends/find_addends_utils.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/gentools.py` & `dramkit-0.5.43/dramkit/gentools.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,37 +415,97 @@
                     if sleep_seconds > 0:
                         time.sleep(sleep_seconds)
                 return result
         return repeater
     return transfunc
 
 
+def catch_error(logger=None, raise_error=True):
+    '''
+    作为装饰器捕获函数运行错误
+    
+    Parameters
+    ----------
+    logger : None, logging.Logger
+        日志记录器，若为None，则会优先使用被调用函数参数中的logger
+    
+    Examples
+    --------
+    .. code-block:: python
+        :linenos:
+
+        from dramkit import simple_logger
+        logger = simple_logger()
+
+        @catch_error(logger)
+        def test_error():
+            print('test_error...') 
+            raise ValueError('test raise')
+            
+        @catch_error()
+        def test_error1(logger=None):
+            print('test_error1...')
+            raise ValueError('test raise1')
+            
+        @catch_error(simple_logger(logname='test'))
+        @capture_print()
+        def test_error2(logger=None):
+            print('test_error2...')
+            
+        @catch_error(False)
+        def test_error3(logger=None):
+            print('test_error3...')
+            raise ValueError('test raise3')
+
+    >>> test_error()
+    >>> test_error1(logger=simple_logger('./_test/catch_error_test.log'))
+    >>> test_error2(logger=simple_logger('./_test/catch_error_test.log'))    
+    >>> test_error3()    
+    '''
+    def transfunc(func):
+        @wraps(func)
+        def catcher(*args, **kwargs):
+            '''运行func并捕获错误信息'''
+            try:
+                return func(*args, **kwargs)
+            except:
+                err = 'func `%s` error info:\n%s'%(func.__name__, traceback.format_exc())
+                if isnull(logger) and 'logger' in kwargs:
+                    logger_show(err, kwargs['logger'], 'error', err_exc_info=False)
+                else:
+                    logger_show(err, logger, 'error', err_exc_info=False)
+                if raise_error:
+                    raise
+                else:
+                    return None
+        return catcher
+    return transfunc
+
+
 def capture_print(logger=None, del_last_blank=True):
     '''
     作为装饰器捕获函数中的print内容
     
     Parameters
     ----------
     logger : None, logging.Logger
         日志记录器，若为None，则会优先使用被调用函数参数中的logger
     
-
     Examples
     --------
     .. code-block:: python
         :linenos:
 
         from dramkit import simple_logger
         logger = simple_logger()
 
         @capture_print(logger)
         def test_print():
             print('test_print...')
             
-            
         @capture_print()
         def test_print1(logger=None):
             print('test_print1...')
             
         @capture_print(simple_logger(logname='test'))
         def test_print2(logger=None):
             print('test_print2...')
@@ -460,15 +520,15 @@
     >>> test_print1(logger=simple_logger('./_test/capture_print_test.log'))
     >>> test_print2(logger=simple_logger('./_test/capture_print_test.log'))    
     >>> test_print3()
     '''
     def transfunc(func):
         @wraps(func)
         def capturer(*args, **kwargs):
-            '''运行func并记录用时'''
+            '''运行func并捕获print内容'''
             # 替换默认的标准输出流
             output = StringIO()
             sys.stdout = output
             result = func(*args, **kwargs)
             # 恢复标准输出流，捕获内容
             sys.stdout = sys.__stdout__
             strs = output.getvalue()
@@ -503,16 +563,15 @@
         from dramkit import simple_logger
         logger = simple_logger()
 
         @log_used_time(logger)
         def wait():
             print('wait...')
             time.sleep(3)
-            
-            
+
         @log_used_time()
         def wait1(logger=None):
             print('wait...')
             time.sleep(3)
             
         @log_used_time(simple_logger(logname='test'))
         def wait2(logger=None):
@@ -3475,31 +3534,34 @@
             #     # 会解析成文本列表：arg = ['l1', 'l2', 'l3']
             #     args_info.append((['--%s'%arg], {'required': True, 'nargs': '+'}))
             if func_args['annotations'][arg].__name__.lower()  in native_eval_types:
                 # 传参命令写法：按照python正常写法即可，但是不能有空格，如：
                 # list: --arg ['a',2,{'a':3}]
                 # tuple: --arg ('a',2,{'a':3})
                 # dict: --arg {'k1':'v1','k2':2}
-                args_info.append((['--%s'%arg], {'required': True, 'type': lambda x: eval(x)}))
+                args_info.append((['--%s'%arg], {'required': True, 'type': lambda x: eval(x), 'help': '入参按照python正常写法写，但是不能有空格。'}))
             else:
                 args_info.append((['--%s'%arg], {'required': True, 'type': func_args['annotations'][arg]}))
     for arg, default in defaults.items():
         if arg not in func_args['annotations']:
             args_info.append((['--%s'%arg], {'default': default}))
         else:
             if func_args['annotations'][arg].__name__ == 'bool':
                 if not default:
                     args_info.append((['--%s'%arg], {'action': 'store_true', 'default': default}))
                 else:
                     args_info.append((['--%s'%arg], {'action': 'store_false', 'default': default}))
             elif func_args['annotations'][arg].__name__.lower()  in native_eval_types:
-                args_info.append((['--%s'%arg], {'default': default, 'type': lambda x: eval(x)}))
+                args_info.append((['--%s'%arg], {'default': default, 'type': lambda x: eval(x), 'help': '入参按照python正常写法写，但是不能有空格。'}))
             else:
                 args_info.append((['--%s'%arg], {'default': default, 'type': func_args['annotations'][arg]}))
-    return parse_args(args_info)
+    # kwargs，按字典处理
+    if not isnull(func_args['varkw']):
+        args_info.append((['--%s'%func_args['varkw']], {'default': {}, 'type': lambda x: eval(x), 'help': '入参按照python正常写法写，但是不能有空格。'}))
+    return parse_args(args_info), func_args
 
 
 def get_topn_names(df, n=1, max_or_min='max',
                    col_or_row='col'):
     '''
     获取df中值最大/小的前n列/行的名称
```

### Comparing `dramkit-0.5.42/dramkit/install_check.py` & `dramkit-0.5.43/dramkit/install_check.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/iotools.py` & `dramkit-0.5.43/dramkit/iotools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/logtools/logger_general.py` & `dramkit-0.5.43/dramkit/logtools/logger_general.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/logtools/logger_rotating.py` & `dramkit-0.5.43/dramkit/logtools/logger_rotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/logtools/logger_timedrotating.py` & `dramkit-0.5.43/dramkit/logtools/logger_timedrotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/logtools/utils_logger.py` & `dramkit-0.5.43/dramkit/logtools/utils_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,46 +17,50 @@
 # '''%(asctime)s -%(levelname)s:
 # --%(message)s''')
 formatter = logging.Formatter(
 '''%(message)s
     [%(levelname)s: %(asctime)s]''')
 
 
-def logger_show(log_str, logger=None, level='info'):
+def logger_show(log_str, logger=None, level='info',
+                err_exc_info=True, **kwargs):
     '''
     显示|记录日志信息
 
     parameters
     ----------
     log_str : str
         日志内容字符串
     logger : logging.Logger, None, nan, False
         - 若为False，则不显示|记录日志信息
         - 若为None或nan，则用print打印log_str
         - 若为logging.Logger对象，则根据level设置进行日志显示|记录
     level : str
         支持'info', 'warn', 'error'三个日志级别
+    err_exec_info : bool
+        显示错误信息时是否写入错误信息
+        注：若log_str中已经包含了错误信息，可将其设置为False以避免重复记录错误日志
 
 
     .. todo::
         - 添加更多level和设置
     '''
     if isnull(logger):
         print(log_str)
         print('    [time: {}]'.format(
         datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f')))
     elif logger is False:
         return
     elif isinstance(logger, logging.Logger):
         if level == 'info':
-            logger.info(log_str)
+            logger.info(log_str, **kwargs)
         elif level in ['warn', 'warning']:
-            logger.warning(log_str)
+            logger.warning(log_str, **kwargs)
         elif level in ['error', 'err']:
-            logger.error(log_str, exc_info=True)
+            logger.error(log_str, exc_info=err_exc_info, **kwargs)
         else:
             raise ValueError('未识别的日志级别设置！')
     else:
         raise ValueError('未识别的logger！')
 
 
 def close_log_file(logger):
```

### Comparing `dramkit-0.5.42/dramkit/openai/aiedu_chat.py` & `dramkit-0.5.43/dramkit/openai/aiedu_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/openai/openai_chat.py` & `dramkit-0.5.43/dramkit/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/openai/openai_chat_hs.py` & `dramkit-0.5.43/dramkit/openai/openai_chat_hs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/alo.py` & `dramkit-0.5.43/dramkit/optimizer/alo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/base_funcs.py` & `dramkit-0.5.43/dramkit/optimizer/base_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/boa.py` & `dramkit-0.5.43/dramkit/optimizer/boa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/cs.py` & `dramkit-0.5.43/dramkit/optimizer/cs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/ga.py` & `dramkit-0.5.43/dramkit/optimizer/ga.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/gwo.py` & `dramkit-0.5.43/dramkit/optimizer/gwo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/hcpsoboa.py` & `dramkit-0.5.43/dramkit/optimizer/hcpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/hho.py` & `dramkit-0.5.43/dramkit/optimizer/hho.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/hpsoboa.py` & `dramkit-0.5.43/dramkit/optimizer/hpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/pso.py` & `dramkit-0.5.43/dramkit/optimizer/pso.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/utils_heuristic.py` & `dramkit-0.5.43/dramkit/optimizer/utils_heuristic.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/optimizer/woa.py` & `dramkit-0.5.43/dramkit/optimizer/woa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/other/_Linux_notes.py` & `dramkit-0.5.43/dramkit/other/_Linux_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/other/_Python_notes.py` & `dramkit-0.5.43/dramkit/other/_Python_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/other/_Vim_notes.py` & `dramkit-0.5.43/dramkit/other/_Vim_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/other/langconv.py` & `dramkit-0.5.43/dramkit/other/langconv.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/other/othertools.py` & `dramkit-0.5.43/dramkit/other/othertools.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 Uncommonly used utility functions
 '''
 
 import os
 import sys
 import subprocess
 import pandas as pd
-from dramkit.gentools import cut_df_by_con_val, isnull
+from dramkit.gentools import cut_df_by_con_val, isnull, check_list_arg
 from dramkit.iotools import read_lines, load_csv, logger_show
-from dramkit.iotools import find_dir_include_str
+from dramkit.iotools import find_dir_include_str, del_specified_subdir
 
 from dramkit.other.langconv import Converter
 
 
 def traditional2simplified(content):
     '''
     | 繁体转简体
@@ -204,14 +204,23 @@
     for fdir in pkg_paths:
         files.append(find_dir_include_str(tgt_str, root_dir=fdir,
                                           file_types='.py', **kwargs))
     files = pd.concat(files, axis=0)
     return files
 
 
+def _drop_pypkgs_dir(dirname='__pycache__', pkgs=None, **kwargs):
+    pkgs = check_list_arg(pkgs, allow_none=True)
+    if isnull(pkgs):
+        pkgs = ['DramKit', 'FinFactory', 'ChnCal']
+    pkg_paths = [x for x in sys.path if any([y in os.path.basename(x) for y in pkgs])]
+    for fdir in pkg_paths:
+        del_specified_subdir(fdir, dirname, **kwargs)
+
+
 def install_pkg(pkg_name, version=None, upgrade=False,
                 ignore_exist=False, logger=None):
     '''
     安装python库
 
     Parameters
     ----------
```

### Comparing `dramkit-0.5.42/dramkit/other/replace_endblank.py` & `dramkit-0.5.43/dramkit/other/replace_endblank.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/other/zh_wiki.py` & `dramkit-0.5.43/dramkit/other/zh_wiki.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/plottools/plot_barline.py` & `dramkit-0.5.43/dramkit/plottools/plot_barline.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/plottools/plot_common.py` & `dramkit-0.5.43/dramkit/plottools/plot_common.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/plottools/plot_histdist.py` & `dramkit-0.5.43/dramkit/plottools/plot_histdist.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/plottools/plot_scatter.py` & `dramkit-0.5.43/dramkit/plottools/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/plottools/utils_plot.py` & `dramkit-0.5.43/dramkit/plottools/utils_plot.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/pystyles/dramkit_style.py` & `dramkit-0.5.43/dramkit/pystyles/dramkit_style.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sorts/bubble_sort.py` & `dramkit-0.5.43/dramkit/sorts/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sorts/bucket_sort.py` & `dramkit-0.5.43/dramkit/sorts/bucket_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sorts/insert_sort.py` & `dramkit-0.5.43/dramkit/sorts/insert_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sorts/insert_sort_bin.py` & `dramkit-0.5.43/dramkit/sorts/insert_sort_bin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sorts/quick_sort.py` & `dramkit-0.5.43/dramkit/sorts/quick_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/speedup/_mp_test1.py` & `dramkit-0.5.43/dramkit/speedup/_mp_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/speedup/_mp_test2.py` & `dramkit-0.5.43/dramkit/speedup/_mp_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/speedup/_mp_test3.py` & `dramkit-0.5.43/dramkit/speedup/_mp_test3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/speedup/iotools_tmp.py` & `dramkit-0.5.43/dramkit/speedup/iotools_tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/speedup/multi_process_concurrent.py` & `dramkit-0.5.43/dramkit/speedup/multi_process_concurrent.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/speedup/multi_thread.py` & `dramkit-0.5.43/dramkit/speedup/multi_thread.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sqltools/_Hive_notes.py` & `dramkit-0.5.43/dramkit/sqltools/_Hive_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sqltools/_MySQL_notes.py` & `dramkit-0.5.43/dramkit/sqltools/_MySQL_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sqltools/_Oracle_notes.py` & `dramkit-0.5.43/dramkit/sqltools/_Oracle_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sqltools/cxoracle.py` & `dramkit-0.5.43/dramkit/sqltools/cxoracle.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sqltools/py_hive.py` & `dramkit-0.5.43/dramkit/sqltools/py_hive.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sqltools/py_mysql.py` & `dramkit-0.5.43/dramkit/sqltools/py_mysql.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/sqltools/sql_alchemy.py` & `dramkit-0.5.43/dramkit/sqltools/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/webtools/utils_html.py` & `dramkit-0.5.43/dramkit/webtools/utils_html.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit/wechat/qywechat.py` & `dramkit-0.5.43/dramkit/wechat/qywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.42/dramkit.egg-info/PKG-INFO` & `dramkit-0.5.43/dramkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.42
+Version: 0.5.43
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.42/dramkit.egg-info/SOURCES.txt` & `dramkit-0.5.43/dramkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -120,18 +120,20 @@
 dramkit/optimizer/gwo.py
 dramkit/optimizer/hcpsoboa.py
 dramkit/optimizer/hho.py
 dramkit/optimizer/hpsoboa.py
 dramkit/optimizer/pso.py
 dramkit/optimizer/utils_heuristic.py
 dramkit/optimizer/woa.py
+dramkit/other/_Git_notes.py
 dramkit/other/_Linux_notes.py
 dramkit/other/_Python_notes.py
 dramkit/other/_Vim_notes.py
 dramkit/other/__init__.py
+dramkit/other/debt_cal.py
 dramkit/other/langconv.py
 dramkit/other/othertools.py
 dramkit/other/replace_endblank.py
 dramkit/other/zh_wiki.py
 dramkit/plottools/__init__.py
 dramkit/plottools/plot_barline.py
 dramkit/plottools/plot_common.py
```

### Comparing `dramkit-0.5.42/setup.py` & `dramkit-0.5.43/setup.py`

 * *Files identical despite different names*

