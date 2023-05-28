# Comparing `tmp/pyflp-2.1.1.tar.gz` & `tmp/pyflp-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflp-2.1.1.tar", last modified: Wed May 24 15:45:42 2023, max compression
+gzip compressed data, was "pyflp-2.2.0.tar", last modified: Sun May 28 11:44:37 2023, max compression
```

## Comparing `pyflp-2.1.1.tar` & `pyflp-2.2.0.tar`

### file list

```diff
@@ -1,315 +1,317 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.411817 pyflp-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-24 15:45:22.000000 pyflp-2.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.371812 pyflp-2.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-24 15:45:22.000000 pyflp-2.1.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-24 15:45:22.000000 pyflp-2.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-24 15:45:22.000000 pyflp-2.1.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-05-24 15:45:22.000000 pyflp-2.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-24 15:45:22.000000 pyflp-2.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 15:45:22.000000 pyflp-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-24 15:45:22.000000 pyflp-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21713 2023-05-24 15:45:42.411817 pyflp-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-05-24 15:45:22.000000 pyflp-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.375813 pyflp-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.375813 pyflp-2.1.1/docs/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/architecture/flp-format.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/architecture/how-it-works.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/architecture/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/features.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.375813 pyflp-2.1.1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/guides/plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/guides/reversing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/guides.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/handbook.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/helping.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.371812 pyflp-2.1.1/docs/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.375813 pyflp-2.1.1/docs/img/arrangement/
--rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/preview.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/time-signature.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.375813 pyflp-2.1.1/docs/img/arrangement/timemarker/
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/timemarker/action.png
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/timemarker/preview.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.375813 pyflp-2.1.1/docs/img/arrangement/track/
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/color.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/enabled.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/grouped.gif
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/icon.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/locked.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/motion.png
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/performance-settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/press.png
--rw-r--r--   0 runner    (1001) docker     (123)    22957 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/preview.png
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/arrangement/track/sync.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.379813 pyflp-2.1.1/docs/img/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/arp.png
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/automation.png
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/color.gif
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/content.png
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/delay.png
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/enabled.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/envelope.png
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/filter.png
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/fx1.png
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/fx2.png
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/icon.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/keyboard.png
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/layer.png
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/level-adjusts.png
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/lfo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/locked.gif
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/playback.png
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/polyphony.png
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/rack.png
--rw-r--r--   0 runner    (1001) docker     (123)    47255 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/sampler.png
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/stretch-mode.png
--rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/stretching.png
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/time.png
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/toolbar.png
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/tracking.png
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/channel/zipped.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.383814 pyflp-2.1.1/docs/img/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/contributing/pytest.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/contributing/readthedocs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/contributing/vscode.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.383814 pyflp-2.1.1/docs/img/controller/
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/controller/remote.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.383814 pyflp-2.1.1/docs/img/features/
--rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/features/images-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    25798 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/features/images-light.png
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/features/tables-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/features/tables-light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.367812 pyflp-2.1.1/docs/img/guides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.383814 pyflp-2.1.1/docs/img/guides/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/guides/plugin/1-parameters.png
--rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/guides/plugin/2-load-plugin.png
--rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/guides/plugin/3-observe-knob-positions.png
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/guides/plugin/4-hint-panel.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.383814 pyflp-2.1.1/docs/img/guides/reversing/
--rw-r--r--   0 runner    (1001) docker     (123)    41307 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/guides/reversing/flpedit.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.383814 pyflp-2.1.1/docs/img/helping/
--rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/helping/open-issue-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    23706 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/helping/open-issue-light.png
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/helping/star-repo-dark.gif
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/helping/star-repo-light.gif
--rw-r--r--   0 runner    (1001) docker     (123)    42665 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/helping/watch-repo-dark.gif
--rw-r--r--   0 runner    (1001) docker     (123)    42617 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/helping/watch-repo-light.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.383814 pyflp-2.1.1/docs/img/mixer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.387814 pyflp-2.1.1/docs/img/mixer/insert/
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/insert/dock.png
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/insert/enabled.gif
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/insert/eq.png
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/insert/input.png
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/insert/locked.gif
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/insert/output.png
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/insert/pan.gif
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/insert/preview.png
--rw-r--r--   0 runner    (1001) docker     (123)   111613 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/preview.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.387814 pyflp-2.1.1/docs/img/mixer/slot/
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/slot/color.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/slot/enabled.gif
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/slot/icon.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/slot/locked.gif
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/mixer/slots.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.387814 pyflp-2.1.1/docs/img/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/pattern/color.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.387814 pyflp-2.1.1/docs/img/pattern/note/
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/pattern/note/group.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.387814 pyflp-2.1.1/docs/img/plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.387814 pyflp-2.1.1/docs/img/plugin/effects/
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/effects/fruity-balance.png
--rw-r--r--   0 runner    (1001) docker     (123)    42770 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/effects/fruity-blood-overdrive.png
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/effects/fruity-center.png
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/effects/fruity-fast-dist.png
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/effects/fruity-notebook2.png
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/effects/fruity-send.png
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/effects/fruity-soft-clipper.png
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/effects/fruity-stereo-enhancer.png
--rw-r--r--   0 runner    (1001) docker     (123)    35054 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/effects/soundgoodizer.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.387814 pyflp-2.1.1/docs/img/plugin/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/generators/boobass.png
--rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/generators/fruit-kick.png
--rw-r--r--   0 runner    (1001) docker     (123)    47669 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/generators/plucked.png
--rw-r--r--   0 runner    (1001) docker     (123)    52803 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/maximize.gif
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/toolbar_collapse.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.391815 pyflp-2.1.1/docs/img/plugin/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/wrapper/page.gif
--rw-r--r--   0 runner    (1001) docker     (123)    37229 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/wrapper/processing.png
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/wrapper/settings-gui.png
--rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/wrapper/settings-midi.png
--rw-r--r--   0 runner    (1001) docker     (123)    48421 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/wrapper/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/plugin/wrapper/troubleshooting.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.391815 pyflp-2.1.1/docs/img/project/
--rw-r--r--   0 runner    (1001) docker     (123)    36725 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/project/info.png
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/project/ppq.png
--rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/project/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/project/tempo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/project/time-spent.png
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/img/project/version.png
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.391815 pyflp-2.1.1/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.391815 pyflp-2.1.1/docs/reference/arrangement/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/arrangement/arrangement.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/arrangement/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/arrangement/playlist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/arrangement/track.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.395815 pyflp-2.1.1/docs/reference/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/channel/automation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/channel/channel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/channel/display-group.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/channel/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/channel/instrument.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/channel/layer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/channel/sampler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/channel/shared.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/controllers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/exceptions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.395815 pyflp-2.1.1/docs/reference/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/mixer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/mixer/insert.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/mixer/slot.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.395815 pyflp-2.1.1/docs/reference/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/patterns/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/patterns/pattern.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.395815 pyflp-2.1.1/docs/reference/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/plugins/effects.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/plugins/generators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/plugins/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/plugins/vst.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference/timemarkers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 15:45:22.000000 pyflp-2.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.399815 pyflp-2.1.1/pyflp/
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:45:42.000000 pyflp-2.1.1/pyflp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/arrangement.py
--rw-r--r--   0 runner    (1001) docker     (123)    50633 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20662 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    34994 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19127 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyflp/timemarker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.399815 pyflp-2.1.1/pyflp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21713 2023-05-24 15:45:42.000000 pyflp-2.1.1/pyflp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-05-24 15:45:42.000000 pyflp-2.1.1/pyflp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:45:42.000000 pyflp-2.1.1/pyflp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-24 15:45:42.000000 pyflp-2.1.1/pyflp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 15:45:42.000000 pyflp-2.1.1/pyflp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-24 15:45:22.000000 pyflp-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 15:45:22.000000 pyflp-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:45:42.411817 pyflp-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.399815 pyflp-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.399815 pyflp-2.1.1/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   190128 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/FL 20.8.4.flp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.403816 pyflp-2.1.1/tests/assets/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/+4800-cents.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/-4800-cents.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/100%-left.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/100%-right.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/arp.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/automation-lfo.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/automation-points.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/colored.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/cut-groups.fst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/delay.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/disabled.fst
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/envelope.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/full-volume.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/iconified.fst
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/keyboard.fst
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/layer-crossfade.fst
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/layer-random.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/level-adjusts.fst
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/lfo.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/locked.fst
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/polyphony.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/routed.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/sampler-content.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/sampler-filter.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/sampler-fx.fst
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/sampler-path.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/sampler-playback.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/sampler-stretching.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/time.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/tracking.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/channels/zero-volume.fst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.407816 pyflp-2.1.1/tests/assets/corrupted/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/corrupted/invalid-data-magic.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/corrupted/invalid-event-size.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/corrupted/invalid-format.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/corrupted/invalid-header-magic.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/corrupted/invalid-header-size.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/corrupted/invalid-ppq.flp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.407816 pyflp-2.1.1/tests/assets/inserts/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/100%-left.fst
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/100%-merged.fst
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/100%-right.fst
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/100%-separated.fst
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/50ms-input-latency.fst
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/50ms-track-latency.fst
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/armed.fst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/channels-swapped.fst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/colored.fst
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/disabled.fst
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/effects-bypassed.fst
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/iconified.fst
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/locked.fst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/polarity-reversed.fst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/post-eq.fst
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/separator.fst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/inserts/zero-volume.fst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.411817 pyflp-2.1.1/tests/assets/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/c-major-scale.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/c5-1bar.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/color-9.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/common-group.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/empty.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/fine-pitch-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/modx-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/mody-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)   115522 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/multi-channel.flp
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/pan-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/release-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/slide-note.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/patterns/velocity-min-max.fsc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:45:42.411817 pyflp-2.1.1/tests/assets/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/boobass.fst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/fruit-kick.fst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/fruity-balance.fst
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/fruity-blood-overdrive.fst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/fruity-center.fst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/fruity-fast-dist.fst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/fruity-send.fst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/fruity-soft-clipper.fst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/fruity-stereo-enhancer.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/fruity-wrapper.fst
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/plucked.fst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/soundgoodizer.fst
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/assets/plugins/xfer-djmfilter.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/test_arrangement.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/test_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/test_corrupted.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/test_mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-24 15:45:22.000000 pyflp-2.1.1/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-24 15:45:22.000000 pyflp-2.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.257686 pyflp-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-28 11:44:21.000000 pyflp-2.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-28 11:44:21.000000 pyflp-2.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-28 11:44:21.000000 pyflp-2.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-28 11:44:21.000000 pyflp-2.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26412 2023-05-28 11:44:21.000000 pyflp-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-28 11:44:21.000000 pyflp-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 11:44:21.000000 pyflp-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-28 11:44:21.000000 pyflp-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-05-28 11:44:37.257686 pyflp-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20297 2023-05-28 11:44:21.000000 pyflp-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/architecture/flp-format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/architecture/how-it-works.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/architecture/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/guides/plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/guides/reversing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/guides.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/handbook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/helping.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.225686 pyflp-2.2.0/docs/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/img/arrangement/
+-rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/preview.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/time-signature.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/img/arrangement/timemarker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/timemarker/action.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/timemarker/preview.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/img/arrangement/track/
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/color.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/enabled.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/grouped.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/icon.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/locked.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/motion.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/performance-settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/press.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22957 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/preview.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/sync.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.233686 pyflp-2.2.0/docs/img/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/arp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/automation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/color.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/content.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/delay.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/enabled.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/envelope.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/filter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/fx1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/fx2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/icon.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/keyboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/layer.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/level-adjusts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/lfo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/locked.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/playback.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/polyphony.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/rack.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47255 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/sampler.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/stretch-mode.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/stretching.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/time.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/toolbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/tracking.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/zipped.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.233686 pyflp-2.2.0/docs/img/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/contributing/pytest.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/contributing/readthedocs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/contributing/vscode.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.233686 pyflp-2.2.0/docs/img/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/controller/remote.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/features/
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/features/images-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25798 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/features/images-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/features/tables-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/features/tables-light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.225686 pyflp-2.2.0/docs/img/guides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/guides/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/plugin/1-parameters.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/plugin/2-load-plugin.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/plugin/3-observe-knob-positions.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/plugin/4-hint-panel.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/guides/reversing/
+-rw-r--r--   0 runner    (1001) docker     (123)    41307 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/reversing/flpedit.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/helping/
+-rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/open-issue-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23706 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/open-issue-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/star-repo-dark.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/star-repo-light.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    42665 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/watch-repo-dark.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    42617 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/watch-repo-light.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/mixer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/mixer/insert/
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/dock.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/enabled.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/eq.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/input.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/locked.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/output.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/pan.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/preview.png
+-rw-r--r--   0 runner    (1001) docker     (123)   111613 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/preview.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/mixer/slot/
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slot/color.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slot/enabled.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slot/icon.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slot/locked.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slots.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/pattern/color.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/pattern/note/
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/pattern/note/group.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/img/plugin/effects/
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-balance.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42770 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-blood-overdrive.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-center.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-fast-dist.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-notebook2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-send.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-soft-clipper.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-stereo-enhancer.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35054 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/soundgoodizer.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/img/plugin/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/generators/boobass.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/generators/fruit-kick.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47669 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/generators/plucked.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52803 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/maximize.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/toolbar_collapse.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/img/plugin/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/page.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    37229 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/processing.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/settings-gui.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/settings-midi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48421 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/troubleshooting.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/img/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    36725 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/info.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/ppq.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/tempo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/time-spent.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/version.png
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/arrangement/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/arrangement/arrangement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/arrangement/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/arrangement/playlist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/arrangement/track.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/automation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/channel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/display-group.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/instrument.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/layer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/sampler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/shared.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/controllers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/exceptions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/mixer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/mixer/insert.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/mixer/slot.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/patterns/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/patterns/pattern.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/plugins/effects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/plugins/generators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/plugins/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/plugins/vst.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/timemarkers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/pyflp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19152 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/arrangement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50356 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34899 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/timemarker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.249686 pyflp-2.2.0/pyflp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-28 11:44:21.000000 pyflp-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 11:44:37.257686 pyflp-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.249686 pyflp-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.249686 pyflp-2.2.0/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   190128 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/FL 20.8.4.flp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.253686 pyflp-2.2.0/tests/assets/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/+4800-cents.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/-4800-cents.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/100%-left.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/100%-right.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/arp.fst
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/automation-lfo.fst
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/automation-points.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/colored.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/cut-groups.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/delay.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/disabled.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/envelope.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/full-volume.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/iconified.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/keyboard.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/layer-crossfade.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/layer-random.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/level-adjusts.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/lfo.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/locked.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/polyphony.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/routed.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-content.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-filter.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-fx.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-path.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-playback.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-stretching.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/time.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/tracking.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/zero-volume.fst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.253686 pyflp-2.2.0/tests/assets/corrupted/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-data-magic.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-event-size.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-format.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-header-magic.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-header-size.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-ppq.flp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.257686 pyflp-2.2.0/tests/assets/inserts/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/100%-left.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/100%-merged.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/100%-right.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/100%-separated.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/50ms-input-latency.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/50ms-track-latency.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/armed.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/channels-swapped.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/colored.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/disabled.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/effects-bypassed.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/iconified.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/locked.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/polarity-reversed.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/post-eq.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/separator.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/zero-volume.fst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.257686 pyflp-2.2.0/tests/assets/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/c-major-scale.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/c5-1bar.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/color-9.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/common-group.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/empty.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/fine-pitch-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/modx-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/mody-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)   115522 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/multi-channel.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/pan-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/release-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/slide-note.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/velocity-min-max.fsc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.257686 pyflp-2.2.0/tests/assets/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/boobass.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruit-kick.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-balance.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-blood-overdrive.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-center.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-fast-dist.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-send.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-soft-clipper.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-stereo-enhancer.fst
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-wrapper.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/plucked.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/soundgoodizer.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/xfer-djmfilter.fst
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_arrangement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_corrupted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-28 11:44:21.000000 pyflp-2.2.0/tox.ini
```

### Comparing `pyflp-2.1.1/.vscode/extensions.json` & `pyflp-2.2.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/.vscode/settings.json` & `pyflp-2.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/.vscode/tasks.json` & `pyflp-2.2.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/CHANGELOG.md` & `pyflp-2.2.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,32 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.0] - 2023-05-28
+
+### Changed
+
+- All event parsing happens during `pyflp.parse` itself.
+- `colour.Color` replaced with `pyflp.types.RGBA`.
+- Increase *line-length* of 100.
+
+### Fixed
+
+- Backtracking issues in nested dictionaries.
+
+### Removed
+
+- Python 3.7 support.
+- Bunch of intermediate `EventBase` subclasses.
+- Removed dependency on `colour` library.
+
 ## [2.1.1] - 2023-05-24
 
 ### Changed
 
 - Refactored `VSTPluginEvent` sub-event handling into `_VSTPluginProp`.
 - All `VSTPluginEvent` string sub-events decoded as UTF8.
```

### Comparing `pyflp-2.1.1/CODE_OF_CONDUCT.md` & `pyflp-2.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/LICENSE` & `pyflp-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/PKG-INFO` & `pyflp-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: pyflp
-Version: 2.1.1
+Version: 2.2.0
 Summary: FL Studio project file parser
 Author-email: demberto <demberto@protonmail.com>
 License: GPL-3.0
 Project-URL: Source, https://github.com/demberto/PyFLP
 Project-URL: Changelog, https://github.com/demberto/PyFLP/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://pyflp.rtfd.io
 Project-URL: Bug Tracker, https://github.com/demberto/PyFLP/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # PyFLP
 
 PyFLP is an unofficial parser for [FL Studio](https://www.image-line.com/fl-studio/)
@@ -40,15 +39,14 @@
     <col style="width: 10%;"/>
     <col style="width: 90%;"/>
   </colgroup>
   <tbody>
     <tr>
       <th>CI</th>
       <td>
-        <img alt="build" src="https://github.com/demberto/PyFLP/actions/workflows/publish.yml/badge.svg"/>
         <a href="https://pyflp.readthedocs.io/en/latest/">
           <img alt="Documentation Build Status" src="https://img.shields.io/readthedocs/pyflp/latest?logo=read-the-docs"/>
         </a>
         <a href="https://results.pre-commit.ci/latest/github/demberto/PyFLP/master">
           <img alt="pre-commit-ci" src="https://results.pre-commit.ci/badge/github/demberto/PyFLP/master.svg"/>
         </a>
       </td>
@@ -337,15 +335,15 @@
     </td>
   </tr>
 </table>
 <!-- markdownlint-restore -->
 
 ## ⏬ Installation
 
-CPython 3.7+ / PyPy 3.8+ required.
+CPython 3.8+ / PyPy 3.8+ required.
 
 ```none
 python -m pip install -U pyflp
 ```
 
 ## ▶ Usage
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1 Name: pyflp Version: 2.1.1 Summary: FL Studio project
+Metadata-Version: 2.1 Name: pyflp Version: 2.2.0 Summary: FL Studio project
 file parser Author-email: demberto
 protonmail.com> License: GPL-3.0 Project-URL: Source, https://github.com/
 demberto/PyFLP Project-URL: Changelog, https://github.com/demberto/PyFLP/blob/
 master/CHANGELOG.md Project-URL: Documentation, https://pyflp.rtfd.io Project-
 URL: Bug Tracker, https://github.com/demberto/PyFLP/issues Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Multimedia
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev License-File: LICENSE # PyFLP PyFLP is an
-unofficial parser for [FL Studio](https://www.image-line.com/fl-studio/
-) project and preset files written in Python.
-CI       [build] [Documentation_Build_Status] [pre-commit-ci]
+:: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Multimedia Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python: >=3.8
+Description-Content-Type: text/markdown Provides-Extra: dev License-File:
+LICENSE # PyFLP PyFLP is an unofficial parser for [FL Studio](https://
+www.image-line.com/fl-studio/) project and preset files written in Python.
+CI       [Documentation_Build_Status] [pre-commit-ci]
 PyPI     [PyPI_-_Package_Version] [PyPI_-_Supported_Python_Versions] [PyPI_-
          Supported_Implementations] [PyPI_-_Wheel]
 Activity [Maintenance] [PyPI_-_Downloads]
 QA       [codecov] [CodeFactor_Grade] [Checked_with_mypy] [pre-commit]
          [Security_Status]
 Other    [License] [GitHub top language] [Code_Style:_Black] [covenant]
  From a very general point-of-view, this is the state of what is currently
@@ -65,15 +64,15 @@
 Plugins                                         issues]
                                                 [plugin-3rdparty_issues]
                           VST_2/3               [closed_plugin-3rdparty
                                                 issues]
                                                 [open_project-general
 Project - Settings and song metadata            issues] [closed_project-
                                                 general_issues]
- ## â¬ Installation CPython 3.7+ / PyPy 3.8+ required. ```none python -m pip
+ ## â¬ Installation CPython 3.8+ / PyPy 3.8+ required. ```none python -m pip
 install -U pyflp ``` ## â¶ Usage [Load](https://pyflp.readthedocs.io/en/
 latest/reference.html#pyflp.parse) a project file: ```py import pyflp project =
 pyflp.parse("/path/to/parse.flp") ``` > If you get any sort of errors or
 warnings while doing this, please open an > [issue](https://github.com/
 demberto/PyFLP/issues). [Save](https://pyflp.readthedocs.io/en/latest/
 reference.html#pyflp.save) the project: ```py pyflp.save(project, "/path/to/
 save.flp") ``` > It is advised to do a backup of your projects before doing any
```

### Comparing `pyflp-2.1.1/README.md` & `pyflp-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     <col style="width: 10%;"/>
     <col style="width: 90%;"/>
   </colgroup>
   <tbody>
     <tr>
       <th>CI</th>
       <td>
-        <img alt="build" src="https://github.com/demberto/PyFLP/actions/workflows/publish.yml/badge.svg"/>
         <a href="https://pyflp.readthedocs.io/en/latest/">
           <img alt="Documentation Build Status" src="https://img.shields.io/readthedocs/pyflp/latest?logo=read-the-docs"/>
         </a>
         <a href="https://results.pre-commit.ci/latest/github/demberto/PyFLP/master">
           <img alt="pre-commit-ci" src="https://results.pre-commit.ci/badge/github/demberto/PyFLP/master.svg"/>
         </a>
       </td>
@@ -307,15 +306,15 @@
     </td>
   </tr>
 </table>
 <!-- markdownlint-restore -->
 
 ## ⏬ Installation
 
-CPython 3.7+ / PyPy 3.8+ required.
+CPython 3.8+ / PyPy 3.8+ required.
 
 ```none
 python -m pip install -U pyflp
 ```
 
 ## ▶ Usage
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # PyFLP PyFLP is an unofficial parser for [FL Studio](https://www.image-
 line.com/fl-studio/) project and preset files written in Python.
-CI       [build] [Documentation_Build_Status] [pre-commit-ci]
+CI       [Documentation_Build_Status] [pre-commit-ci]
 PyPI     [PyPI_-_Package_Version] [PyPI_-_Supported_Python_Versions] [PyPI_-
          Supported_Implementations] [PyPI_-_Wheel]
 Activity [Maintenance] [PyPI_-_Downloads]
 QA       [codecov] [CodeFactor_Grade] [Checked_with_mypy] [pre-commit]
          [Security_Status]
 Other    [License] [GitHub top language] [Code_Style:_Black] [covenant]
  From a very general point-of-view, this is the state of what is currently
@@ -47,15 +47,15 @@
 Plugins                                         issues]
                                                 [plugin-3rdparty_issues]
                           VST_2/3               [closed_plugin-3rdparty
                                                 issues]
                                                 [open_project-general
 Project - Settings and song metadata            issues] [closed_project-
                                                 general_issues]
- ## â¬ Installation CPython 3.7+ / PyPy 3.8+ required. ```none python -m pip
+ ## â¬ Installation CPython 3.8+ / PyPy 3.8+ required. ```none python -m pip
 install -U pyflp ``` ## â¶ Usage [Load](https://pyflp.readthedocs.io/en/
 latest/reference.html#pyflp.parse) a project file: ```py import pyflp project =
 pyflp.parse("/path/to/parse.flp") ``` > If you get any sort of errors or
 warnings while doing this, please open an > [issue](https://github.com/
 demberto/PyFLP/issues). [Save](https://pyflp.readthedocs.io/en/latest/
 reference.html#pyflp.save) the project: ```py pyflp.save(project, "/path/to/
 save.flp") ``` > It is advised to do a backup of your projects before doing any
```

### Comparing `pyflp-2.1.1/docs/Makefile` & `pyflp-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/architecture/flp-format.rst` & `pyflp-2.2.0/docs/architecture/flp-format.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/architecture/how-it-works.rst` & `pyflp-2.2.0/docs/architecture/how-it-works.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/architecture/reference.rst` & `pyflp-2.2.0/docs/architecture/reference.rst`

 * *Files 9% similar despite different names*

```diff
@@ -59,22 +59,20 @@
     .. autoclass:: U32Event
     .. autoclass:: I32Event
     .. autoclass:: ColorEvent
     .. autoclass:: U16TupleEvent
 
 .. dropdown:: 192-255
 
-    .. autoclass:: VarintEventBase
     .. autoclass:: StrEventBase
     .. autoclass:: AsciiEvent
     .. autoclass:: UnicodeEvent
-    .. autoclass:: DataEventBase
-    .. autoclass:: UnknownDataEvent
     .. autoclass:: StructEventBase
     .. autoclass:: ListEventBase
+    .. autoclass:: UnknownDataEvent
 
 EventTree
 ^^^^^^^^^
 
 .. autoclass:: EventTree
    :members:
 
@@ -99,7 +97,12 @@
 2. Are ``__dunder__`` methods provided by Python used whenever possible?
 3. Is either :class:`ModelReprMixin` subclassed or ``__repr__`` implemented?
 
 Descriptors
 -----------
 
 .. automodule:: pyflp._descriptors
+
+Adapters
+--------
+
+.. automodule:: pyflp._adapters
```

### Comparing `pyflp-2.1.1/docs/conf.py` & `pyflp-2.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from __future__ import annotations
 
 import enum
 import importlib.metadata
 import inspect
 import re
 
-import colour
 import m2r2
 
 from pyflp._descriptors import EventProp, FlagProp, NestedProp, StructProp
-from pyflp._events import EventEnum
+from pyflp._events import EventEnum, RGBA
 from pyflp._models import ModelBase
 from pyflp.arrangement import _TrackColorProp
 
 BITLY_LINK = re.compile(r"!\[.*\]\((https://bit\.ly/[A-z0-9]*)\)")
 """Shortened URLs for links to in-docstring images and docs."""
 
 NEW_IN_FL = re.compile(r"\*New in FL Studio v([^\*]*)\*[\.:](.*)")
@@ -125,15 +124,15 @@
 
 def add_annotations(app, what, name, obj, options, signature, return_annotation):
     """Add type annotations for descriptors."""
     if what == "class" and issubclass(obj, ModelBase):
         annotations = {}
         for name_, type in vars(obj).items():
             if isinstance(type, _TrackColorProp):
-                annotations[name_] = colour.Color
+                annotations[name_] = RGBA
             elif isinstance(type, NestedProp):
                 annotations[name_] = type._type
             elif isinstance(type, FlagProp):
                 annotations[name_] = bool | None
             elif hasattr(type, "__orig_class__"):
                 annotations[name_] = type.__orig_class__.__args__[0]
```

### Comparing `pyflp-2.1.1/docs/contributing.rst` & `pyflp-2.2.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/faq.rst` & `pyflp-2.2.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/features.rst` & `pyflp-2.2.0/docs/features.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/guides/plugin.rst` & `pyflp-2.2.0/docs/guides/plugin.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/guides/reversing.rst` & `pyflp-2.2.0/docs/guides/reversing.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/handbook.rst` & `pyflp-2.2.0/docs/handbook.rst`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,19 @@
    While this will work for 3rd party samples *unless there's 2 samples with
    the same name*, FL Studio doesn't store the full path inside an FLP for
    stock samples. See :attr:`pyflp.channel.Sampler.sample_path` for more info.
 
 🔓 Unlocking demo version FLPs
 -------------------------------
 
+.. caution::
+
+   This doesn't work for FL Studio 21 projects.
+   See `#146 <https://github.com/demberto/PyFLP/discussions/146>`
+
 FLPs saved with a trial version of FL Studio cannot be reopened again without
 saving in a registered version. The state of demo versions of native plugins'
 is not retained either.
 
 .. hint::
 
    This section **doesn't** explain how to make 3rd party plugin demos
@@ -93,19 +98,19 @@
 .. code-block:: python
 
    import pyflp
 
    project = pyflp.parse("/path/to/myflp.flp")
 
    # Unlock the FLP itself
-   project.registered = True
+   project.licensed = True
 
    # Unlock trial version native plugins
    for instument in project.channels.instruments:
-       instrument.demo_mode = False
+       instrument.plugin.demo_mode = False
 
    for insert in project.mixer:
        for slot in insert:
            if slot.plugin is not None:
               slot.plugin.demo_mode = False
 
    pyflp.save(project, "/path/to/myflp_unlocked.flp")
```

### Comparing `pyflp-2.1.1/docs/helping.rst` & `pyflp-2.2.0/docs/helping.rst`

 * *Files 6% similar despite different names*

```diff
@@ -76,11 +76,10 @@
 
 🙌 You can also open a new discussion to tell me what you made with PyFLP and
 how it helped you. I am more than glad to find how PyFLP is getting used.
 
 Help the tools that power **PyFLP**
 -----------------------------------
 
-- `colour <https://github.com/vaab/colour>`_
 - `construct <https://github.com/construct/construct>`_
 - `f-enum <https://github.com/Bobronium/fastenum>`_
 - `sortedcontainers <https://github.com/grantjenks/python-sortedcontainers>`_
```

### Comparing `pyflp-2.1.1/docs/img/arrangement/preview.jpg` & `pyflp-2.2.0/docs/img/arrangement/preview.jpg`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/time-signature.png` & `pyflp-2.2.0/docs/img/arrangement/time-signature.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/timemarker/action.png` & `pyflp-2.2.0/docs/img/arrangement/timemarker/action.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/timemarker/preview.png` & `pyflp-2.2.0/docs/img/arrangement/timemarker/preview.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/color.gif` & `pyflp-2.2.0/docs/img/arrangement/track/color.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/enabled.gif` & `pyflp-2.2.0/docs/img/arrangement/track/enabled.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/grouped.gif` & `pyflp-2.2.0/docs/img/arrangement/track/grouped.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/icon.gif` & `pyflp-2.2.0/docs/img/arrangement/track/icon.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/locked.gif` & `pyflp-2.2.0/docs/img/arrangement/track/locked.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/motion.png` & `pyflp-2.2.0/docs/img/arrangement/track/motion.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/performance-settings.png` & `pyflp-2.2.0/docs/img/arrangement/track/performance-settings.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/press.png` & `pyflp-2.2.0/docs/img/arrangement/track/press.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/preview.png` & `pyflp-2.2.0/docs/img/arrangement/track/preview.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/arrangement/track/sync.png` & `pyflp-2.2.0/docs/img/arrangement/track/sync.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/arp.png` & `pyflp-2.2.0/docs/img/channel/arp.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/automation.png` & `pyflp-2.2.0/docs/img/channel/automation.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/color.gif` & `pyflp-2.2.0/docs/img/channel/color.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/content.png` & `pyflp-2.2.0/docs/img/channel/content.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/delay.png` & `pyflp-2.2.0/docs/img/channel/delay.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/enabled.gif` & `pyflp-2.2.0/docs/img/channel/enabled.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/envelope.png` & `pyflp-2.2.0/docs/img/channel/envelope.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/filter.png` & `pyflp-2.2.0/docs/img/channel/filter.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/fx1.png` & `pyflp-2.2.0/docs/img/channel/fx1.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/fx2.png` & `pyflp-2.2.0/docs/img/channel/fx2.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/icon.gif` & `pyflp-2.2.0/docs/img/channel/icon.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/keyboard.png` & `pyflp-2.2.0/docs/img/channel/keyboard.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/layer.png` & `pyflp-2.2.0/docs/img/channel/layer.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/level-adjusts.png` & `pyflp-2.2.0/docs/img/channel/level-adjusts.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/lfo.png` & `pyflp-2.2.0/docs/img/channel/lfo.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/locked.gif` & `pyflp-2.2.0/docs/img/channel/locked.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/playback.png` & `pyflp-2.2.0/docs/img/channel/playback.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/polyphony.png` & `pyflp-2.2.0/docs/img/channel/polyphony.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/rack.png` & `pyflp-2.2.0/docs/img/channel/rack.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/sampler.png` & `pyflp-2.2.0/docs/img/channel/sampler.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/stretch-mode.png` & `pyflp-2.2.0/docs/img/channel/stretch-mode.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/stretching.png` & `pyflp-2.2.0/docs/img/channel/stretching.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/time.png` & `pyflp-2.2.0/docs/img/channel/time.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/toolbar.png` & `pyflp-2.2.0/docs/img/channel/toolbar.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/tracking.png` & `pyflp-2.2.0/docs/img/channel/tracking.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/channel/zipped.png` & `pyflp-2.2.0/docs/img/channel/zipped.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/contributing/pytest.svg` & `pyflp-2.2.0/docs/img/contributing/pytest.svg`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/contributing/readthedocs.svg` & `pyflp-2.2.0/docs/img/contributing/readthedocs.svg`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/contributing/vscode.svg` & `pyflp-2.2.0/docs/img/contributing/vscode.svg`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/controller/remote.png` & `pyflp-2.2.0/docs/img/controller/remote.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/features/images-dark.png` & `pyflp-2.2.0/docs/img/features/images-dark.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/features/images-light.png` & `pyflp-2.2.0/docs/img/features/images-light.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/features/tables-dark.png` & `pyflp-2.2.0/docs/img/features/tables-dark.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/features/tables-light.png` & `pyflp-2.2.0/docs/img/features/tables-light.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/guides/plugin/1-parameters.png` & `pyflp-2.2.0/docs/img/guides/plugin/1-parameters.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/guides/plugin/2-load-plugin.png` & `pyflp-2.2.0/docs/img/guides/plugin/2-load-plugin.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/guides/plugin/3-observe-knob-positions.png` & `pyflp-2.2.0/docs/img/guides/plugin/3-observe-knob-positions.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/guides/plugin/4-hint-panel.png` & `pyflp-2.2.0/docs/img/guides/plugin/4-hint-panel.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/guides/reversing/flpedit.png` & `pyflp-2.2.0/docs/img/guides/reversing/flpedit.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/helping/open-issue-dark.png` & `pyflp-2.2.0/docs/img/helping/open-issue-dark.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/helping/open-issue-light.png` & `pyflp-2.2.0/docs/img/helping/open-issue-light.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/helping/star-repo-dark.gif` & `pyflp-2.2.0/docs/img/helping/star-repo-dark.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/helping/star-repo-light.gif` & `pyflp-2.2.0/docs/img/helping/star-repo-light.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/helping/watch-repo-dark.gif` & `pyflp-2.2.0/docs/img/helping/watch-repo-dark.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/helping/watch-repo-light.gif` & `pyflp-2.2.0/docs/img/helping/watch-repo-light.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/insert/dock.png` & `pyflp-2.2.0/docs/img/mixer/insert/dock.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/insert/enabled.gif` & `pyflp-2.2.0/docs/img/mixer/insert/enabled.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/insert/eq.png` & `pyflp-2.2.0/docs/img/mixer/insert/eq.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/insert/input.png` & `pyflp-2.2.0/docs/img/mixer/insert/input.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/insert/locked.gif` & `pyflp-2.2.0/docs/img/mixer/insert/locked.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/insert/output.png` & `pyflp-2.2.0/docs/img/mixer/insert/output.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/insert/pan.gif` & `pyflp-2.2.0/docs/img/mixer/insert/pan.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/insert/preview.png` & `pyflp-2.2.0/docs/img/mixer/insert/preview.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/preview.png` & `pyflp-2.2.0/docs/img/mixer/preview.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/slot/color.gif` & `pyflp-2.2.0/docs/img/mixer/slot/color.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/slot/enabled.gif` & `pyflp-2.2.0/docs/img/mixer/slot/enabled.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/slot/icon.gif` & `pyflp-2.2.0/docs/img/mixer/slot/icon.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/slot/locked.gif` & `pyflp-2.2.0/docs/img/mixer/slot/locked.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/mixer/slots.png` & `pyflp-2.2.0/docs/img/mixer/slots.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/pattern/color.gif` & `pyflp-2.2.0/docs/img/pattern/color.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/pattern/note/group.gif` & `pyflp-2.2.0/docs/img/pattern/note/group.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/effects/fruity-balance.png` & `pyflp-2.2.0/docs/img/plugin/effects/fruity-balance.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/effects/fruity-blood-overdrive.png` & `pyflp-2.2.0/docs/img/plugin/effects/fruity-blood-overdrive.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/effects/fruity-center.png` & `pyflp-2.2.0/docs/img/plugin/effects/fruity-center.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/effects/fruity-fast-dist.png` & `pyflp-2.2.0/docs/img/plugin/effects/fruity-fast-dist.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/effects/fruity-notebook2.png` & `pyflp-2.2.0/docs/img/plugin/effects/fruity-notebook2.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/effects/fruity-send.png` & `pyflp-2.2.0/docs/img/plugin/effects/fruity-send.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/effects/fruity-soft-clipper.png` & `pyflp-2.2.0/docs/img/plugin/effects/fruity-soft-clipper.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/effects/fruity-stereo-enhancer.png` & `pyflp-2.2.0/docs/img/plugin/effects/fruity-stereo-enhancer.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/effects/soundgoodizer.png` & `pyflp-2.2.0/docs/img/plugin/effects/soundgoodizer.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/generators/boobass.png` & `pyflp-2.2.0/docs/img/plugin/generators/boobass.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/generators/fruit-kick.png` & `pyflp-2.2.0/docs/img/plugin/generators/fruit-kick.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/generators/plucked.png` & `pyflp-2.2.0/docs/img/plugin/generators/plucked.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/maximize.gif` & `pyflp-2.2.0/docs/img/plugin/maximize.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/toolbar_collapse.gif` & `pyflp-2.2.0/docs/img/plugin/toolbar_collapse.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/wrapper/page.gif` & `pyflp-2.2.0/docs/img/plugin/wrapper/page.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/wrapper/processing.png` & `pyflp-2.2.0/docs/img/plugin/wrapper/processing.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/wrapper/settings-gui.png` & `pyflp-2.2.0/docs/img/plugin/wrapper/settings-gui.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/wrapper/settings-midi.png` & `pyflp-2.2.0/docs/img/plugin/wrapper/settings-midi.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/wrapper/settings.png` & `pyflp-2.2.0/docs/img/plugin/wrapper/settings.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/plugin/wrapper/troubleshooting.png` & `pyflp-2.2.0/docs/img/plugin/wrapper/troubleshooting.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/project/info.png` & `pyflp-2.2.0/docs/img/project/info.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/project/ppq.png` & `pyflp-2.2.0/docs/img/project/ppq.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/project/settings.png` & `pyflp-2.2.0/docs/img/project/settings.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/project/tempo.png` & `pyflp-2.2.0/docs/img/project/tempo.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/project/time-spent.png` & `pyflp-2.2.0/docs/img/project/time-spent.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/img/project/version.png` & `pyflp-2.2.0/docs/img/project/version.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/limitations.rst` & `pyflp-2.2.0/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/make.bat` & `pyflp-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/reference/arrangement/track.rst` & `pyflp-2.2.0/docs/reference/arrangement/track.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/reference/channel/sampler.rst` & `pyflp-2.2.0/docs/reference/channel/sampler.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/reference/events.rst` & `pyflp-2.2.0/docs/reference/events.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/reference/plugins/vst.rst` & `pyflp-2.2.0/docs/reference/plugins/vst.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/docs/reference/project.rst` & `pyflp-2.2.0/docs/reference/project.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/pyflp/__init__.py` & `pyflp-2.2.0/pyflp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import os
 import pathlib
 import struct
 import sys
 
 import construct as c
 
-from ._events import (
+from pyflp._events import (
     DATA,
     DWORD,
     NEW_TEXT_IDS,
     TEXT,
     WORD,
     AnyEvent,
     AsciiEvent,
@@ -50,31 +50,29 @@
     IndexedEvent,
     U8Event,
     U16Event,
     U32Event,
     UnicodeEvent,
     UnknownDataEvent,
 )
-from .exceptions import HeaderCorrupted, VersionNotDetected
-from .plugin import PluginID, get_event_by_internal_name
-from .project import VALID_PPQS, FileFormat, Project, ProjectID
+from pyflp.exceptions import HeaderCorrupted, VersionNotDetected
+from pyflp.plugin import PluginID, get_event_by_internal_name
+from pyflp.project import VALID_PPQS, FileFormat, Project, ProjectID
 
 __all__ = ["parse", "save"]
 
 FLP_HEADER = struct.Struct("4sIh2H")
 
 if sys.version_info < (3, 11):  # https://github.com/Bobronium/fastenum/issues/2
     import fastenum
 
     fastenum.enable()  # 33% faster parse()
 
 
 def parse(file: pathlib.Path | str) -> Project:
-    # pylint: disable=too-many-branches
-    # pylint: disable=too-many-statements
     """Parses an FL Studio project file and returns a parsed :class:`Project`.
 
     Args:
         file: Path to the FLP.
 
     Raises:
         HeaderCorrupted: When an invalid value is found in the file header.
```

### Comparing `pyflp-2.1.1/pyflp/_events.py` & `pyflp-2.2.0/pyflp/_events.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,80 +17,52 @@
 and unmarshalling.
 """
 
 from __future__ import annotations
 
 import abc
 import enum
-import sys
 import warnings
+from collections import UserDict, UserList
+from collections.abc import Callable, Iterable, Iterator, Sequence
 from dataclasses import dataclass, field
 from itertools import zip_longest
-from typing import (
-    Any,
-    Callable,
-    ClassVar,
-    Generic,
-    Iterable,
-    Iterator,
-    NoReturn,
-    Tuple,
-    TypeVar,
-    cast,
-)
-
-if sys.version_info >= (3, 8):
-    from typing import Final
-else:
-    from typing_extensions import Final
-
-if sys.version_info >= (3, 10):
-    from typing import Concatenate, ParamSpec
-else:
-    from typing_extensions import Concatenate, ParamSpec
+from typing import TYPE_CHECKING, Any, ClassVar, Final, Generic, Tuple, cast
 
-import colour
 import construct as c
 from sortedcontainers import SortedList
+from typing_extensions import Concatenate, TypeAlias
 
-from .exceptions import (
+from pyflp.exceptions import (
     EventIDOutOfRange,
     InvalidEventChunkSize,
-    ListEventNotParsed,
     PropertyCannotBeSet,
 )
+from pyflp.types import RGBA, P, T
 
 BYTE: Final = 0
 WORD: Final = 64
 DWORD: Final = 128
 TEXT: Final = 192
 DATA: Final = 208
 NEW_TEXT_IDS: Final = (
     TEXT + 49,  # ArrangementID.Name
     TEXT + 39,  # DisplayGroupID.Name
     TEXT + 47,  # TrackID.Name
 )
 
-P = ParamSpec("P")
-T = TypeVar("T")
-T_co = TypeVar("T_co", covariant=True)
-FourByteBool: c.ExprAdapter[int, int, bool, int] = c.ExprAdapter(
-    c.Int32ul, lambda obj_, *_: bool(obj_), lambda obj_, *_: int(obj_)  # type: ignore
-)
-
 
 class _EventEnumMeta(enum.EnumMeta):
-    # pylint: disable=bad-mcs-method-argument
     def __contains__(self, obj: object) -> bool:
         """Whether ``obj`` is one of the integer values of enum members.
 
         Args:
             obj: Can be an ``int`` or an ``EventEnum``.
         """
-        return obj in tuple(self)  # type: ignore
+        return obj in tuple(self)
 
 
 class EventEnum(int, enum.Enum, metaclass=_EventEnumMeta):
     """IDs used by events.
 
     Event values are stored as a tuple of event ID and its designated type.
     The types are used to serialise/deserialise events by the parser.
@@ -124,91 +96,83 @@
                 new_member._name_ = str(value)
                 new_member._value_ = value
                 pseudo_member = cls._value2member_map_.setdefault(value, new_member)
             return cast(EventEnum, pseudo_member)
         # Raises ValueError in Enum.__new__
 
 
-class EventBase(Generic[T]):  # pylint: disable=eq-without-hash
+class EventBase(Generic[T]):
     """Generic ABC representing an event."""
 
-    def __init__(self, id: EventEnum, data: bytes) -> None:
-        self.id: Final = EventEnum(id)
-        self._data: bytes = data
+    STRUCT: c.Construct[T, T]
+    ALLOWED_IDS: ClassVar[Sequence[int]] = []
+
+    def __init__(self, id: EventEnum, data: bytes, **kwds: Any) -> None:
+        if self.ALLOWED_IDS and id not in self.ALLOWED_IDS:
+            raise EventIDOutOfRange(id, *self.ALLOWED_IDS)
+
+        if id < TEXT:
+            if id < WORD:
+                expected_size = 1
+            elif id < DWORD:
+                expected_size = 2
+            else:
+                expected_size = 4
+
+            if len(data) != expected_size:
+                raise InvalidEventChunkSize(expected_size, len(data))
+
+        self.id = EventEnum(id)
+        self._kwds = kwds
+        self.value = self.STRUCT.parse(data, **self._kwds)
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, EventBase):
             raise TypeError(f"Cannot find equality of an {type(o)} and {type(self)!r}")
-        return self.id == o.id and self._data == o._data
+        return self.id == o.id and self.value == cast(EventBase[T], o).value
 
     def __ne__(self, o: object) -> bool:
         if not isinstance(o, EventBase):
             raise TypeError(f"Cannot find inequality of a {type(o)} and {type(self)!r}")
-        return self.id != o.id or self._data != o._data
+        return self.id != o.id or self.value != cast(EventBase[T], o).value
 
-    @abc.abstractmethod
     def __bytes__(self) -> bytes:
-        ...
-
-    @property
-    @abc.abstractmethod
-    def size(self) -> int:
-        """Serialised event size (in bytes)."""  # noqa: D402
-
-    @property
-    def value(self) -> T:
-        """Deserialized event-type specific value."""
-        raise NotImplementedError
-
-    @value.setter
-    def value(self, value: T) -> None:
-        """Converts Python types into bytes/bytes objects and stores it."""
-
-
-AnyEvent = EventBase[Any]
-
-
-class PODEventBase(EventBase[T]):
-    """Base class for events whose size is predetermined (POD types)."""
-
-    ID_RANGE: ClassVar[tuple[int, int]]
-    CODEC: c.Construct[Any, Any]
-
-    def __init__(self, id: EventEnum, data: bytes) -> None:
-        if id not in range(*self.ID_RANGE):
-            raise EventIDOutOfRange(id, *self.ID_RANGE)
-
-        if len(data) != self.CODEC.sizeof():
-            raise InvalidEventChunkSize(self.CODEC.sizeof(), len(data))
+        id = c.Byte.build(self.id)
+        data = self.STRUCT.build(self.value, **self._kwds)
 
-        super().__init__(id, data)
+        if self.id < TEXT:
+            return id + data
 
-    def __bytes__(self) -> bytes:
-        return c.Byte.build(self.id) + self._data
+        length = c.VarInt.build(len(data))
+        return id + length + data
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}(id={self.id!r}, value={self.value!r})"
+        return f"<{type(self)!r}(id={self.id!r}, value={self.value!r})>"
 
     @property
     def size(self) -> int:
-        return 1 + self.CODEC.sizeof()
+        """Serialised event size (in bytes)."""
+
+        if self.id >= TEXT:
+            return len(bytes(self))
+        elif self.id >= DWORD:
+            return 5
+        elif self.id >= WORD:
+            return 3
+        else:
+            return 2
 
-    @property
-    def value(self) -> T:
-        return self.CODEC.parse(self._data)
 
-    @value.setter
-    def value(self, value: T) -> None:
-        self._data = self.CODEC.build(value)
+AnyEvent: TypeAlias = EventBase[Any]
 
 
-class ByteEventBase(PODEventBase[T]):
+class ByteEventBase(EventBase[T]):
     """Base class of events used for storing 1 byte data."""
 
-    ID_RANGE = (BYTE, WORD)
+    ALLOWED_IDS = range(BYTE, WORD)
 
     def __init__(self, id: EventEnum, data: bytes) -> None:
         """
         Args:
             id: **0** to **63**.
             data: Event data of size 1.
 
@@ -218,63 +182,63 @@
         """
         super().__init__(id, data)
 
 
 class BoolEvent(ByteEventBase[bool]):
     """An event used for storing a boolean."""
 
-    CODEC = c.Flag
+    STRUCT = c.Flag
 
 
 class I8Event(ByteEventBase[int]):
     """An event used for storing a 1 byte signed integer."""
 
-    CODEC = c.Int8sl
+    STRUCT = c.Int8sl
 
 
 class U8Event(ByteEventBase[int]):
     """An event used for storing a 1 byte unsigned integer."""
 
-    CODEC = c.Int8ul
+    STRUCT = c.Int8ul
 
 
-class WordEventBase(PODEventBase[T], abc.ABC):
+class WordEventBase(EventBase[int], abc.ABC):
     """Base class of events used for storing 2 byte data."""
 
-    ID_RANGE = (WORD, DWORD)
+    ALLOWED_IDS = range(WORD, DWORD)
 
     def __init__(self, id: EventEnum, data: bytes) -> None:
         """
         Args:
             id: **64** to **127**.
             data: Event data of size 2.
 
         Raises:
             EventIDOutOfRangeError: When ``id`` is not in range of 64-127.
             InvalidEventChunkSizeError: When size of `data` is not 2.
         """
         super().__init__(id, data)
 
 
-class I16Event(WordEventBase[int]):
+class I16Event(WordEventBase):
     """An event used for storing a 2 byte signed integer."""
 
-    CODEC = c.Int16sl
+    STRUCT = c.Int16sl
 
 
-class U16Event(WordEventBase[int]):
+class U16Event(WordEventBase):
     """An event used for storing a 2 byte unsigned integer."""
 
-    CODEC = c.Int16ul
+    STRUCT = c.Int16ul
 
 
-class DWordEventBase(PODEventBase[T], abc.ABC):
+class DWordEventBase(EventBase[T], abc.ABC):
     """Base class of events used for storing 4 byte data."""
 
-    ID_RANGE = (DWORD, TEXT)
+    ALLOWED_IDS = range(DWORD, TEXT)
 
     def __init__(self, id: EventEnum, data: bytes) -> None:
         """
         Args:
             id: **128** to **191**.
             data: Event data of size 4.
 
@@ -284,285 +248,145 @@
         """
         super().__init__(id, data)
 
 
 class F32Event(DWordEventBase[float]):
     """An event used for storing 4 byte floats."""
 
-    CODEC = c.Float32l
+    STRUCT = c.Float32l
 
 
 class I32Event(DWordEventBase[int]):
     """An event used for storing a 4 byte signed integer."""
 
-    CODEC = c.Int32sl
+    STRUCT = c.Int32sl
 
 
 class U32Event(DWordEventBase[int]):
     """An event used for storing a 4 byte unsigned integer."""
 
-    CODEC = c.Int32ul
+    STRUCT = c.Int32ul
 
 
 class U16TupleEvent(DWordEventBase[Tuple[int, int]]):
     """An event used for storing a two-tuple of 2 byte unsigned integers."""
 
-    CODEC: c.ExprAdapter[  # pyright: ignore
-        c.ListContainer[int], c.ListContainer[int], tuple[int, int], list[int]
-    ] = c.ExprAdapter(
+    STRUCT = c.ExprAdapter(
         c.Int16ul[2],
         lambda obj_, *_: tuple(obj_),  # type: ignore
         lambda obj_, *_: list(obj_),  # type: ignore
     )
 
 
-class ColorEvent(DWordEventBase[colour.Color]):
+class ColorEvent(DWordEventBase[RGBA]):
     """A 4 byte event which stores a color."""
 
-    CODEC: c.ExprAdapter[bytes, bytes, colour.Color, colour.Color] = c.ExprAdapter(
+    STRUCT = c.ExprAdapter(
         c.Bytes(4),
-        lambda obj, *_: ColorEvent.decode(obj),  # type: ignore
-        lambda obj, *_: ColorEvent.encode(obj),  # type: ignore
+        lambda obj, *_: RGBA.from_bytes(obj),  # type: ignore
+        lambda obj, *_: bytes(obj),  # type: ignore
     )
 
-    @staticmethod
-    def decode(buf: bytes | bytes) -> colour.Color:
-        r, g, b = (c / 255 for c in buf[:3])
-        return colour.Color(rgb=(r, g, b))
-
-    @staticmethod
-    def encode(color: colour.Color) -> bytes:
-        return bytes(int(c * 255) for c in color.get_rgb()) + b"\x00"
-
-
-class VarintEventBase(EventBase[T]):
-    @staticmethod
-    def _varint_len(buflen: int) -> int:
-        ret = bytearray()
-        while True:
-            towrite = buflen & 0x7F
-            buflen >>= 7
-            towrite |= 0x80
-            ret.append(towrite)
-            if buflen <= 0:
-                break
-        return len(ret)
 
-    @property
-    def size(self) -> int:
-        if self._data:
-            return 1 + self._varint_len(len(self._data)) + len(self._data)
-        return 2
-
-    def __bytes__(self) -> bytes:
-        id = c.Byte.build(self.id)
-
-        if self._data:
-            return id + c.VarInt.build(len(self._data)) + self._data
-        return id + b"\x00"
-
-
-class StrEventBase(VarintEventBase[str]):
+class StrEventBase(EventBase[str]):
     """Base class of events used for storing strings."""
 
+    ALLOWED_IDS = (*range(TEXT, DATA), *NEW_TEXT_IDS)
+
     def __init__(self, id: EventEnum, data: bytes) -> None:
         """
         Args:
             id: **192** to **207** or in :attr:`NEW_TEXT_IDS`.
             data: ASCII or UTF16 encoded string data.
 
         Raises:
             ValueError: When ``id`` is not in 192-207 or in :attr:`NEW_TEXT_IDS`.
         """
-        if id not in {*range(TEXT, DATA), *NEW_TEXT_IDS}:
-            raise ValueError(f"Unexpected ID{id!r}")
-
         super().__init__(id, data)
 
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}(id={self.id!r}, string={self.value!r})"
-
 
 class AsciiEvent(StrEventBase):
-    @property
-    def value(self) -> str:
-        return self._data.decode("ascii").rstrip("\0")
-
-    @value.setter
-    def value(self, value: str) -> None:
-        if value:
-            self._data = value.encode("ascii") + b"\0"
+    if TYPE_CHECKING:
+        STRUCT: c.ExprAdapter[str, str, str, str]
+    else:
+        STRUCT = c.ExprAdapter(
+            c.GreedyString("ascii"),
+            lambda obj, *_: obj.rstrip("\0"),
+            lambda obj, *_: obj + "\0",
+        )
 
 
 class UnicodeEvent(StrEventBase):
-    @property
-    def value(self) -> str:
-        return self._data.decode("utf-16-le").rstrip("\0")
-
-    @value.setter
-    def value(self, value: str) -> None:
-        if value:
-            self._data = value.encode("utf-16-le") + b"\0\0"
-
-
-class DataEventBase(VarintEventBase[bytes]):
-    def __init__(self, id: EventEnum, data: bytes) -> None:
-        """
-        Args:
-            id: **208** to **255**.
-            data: Event data (no size limit).
-
-        Raises:
-            EventIDOutOfRange: ``id`` is not in the range of 208-255.
-        """
-        if id < DATA:
-            raise EventIDOutOfRange(id, DATA, 256)
-
-        super().__init__(id, data)
-
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}(id={self.id!r}, size={len(self._data)})"
+    if TYPE_CHECKING:
+        STRUCT: c.ExprAdapter[str, str, str, str]
+    else:
+        STRUCT = c.ExprAdapter(
+            c.GreedyString("utf-16-le"),
+            lambda obj, *_: obj.rstrip("\0"),
+            lambda obj, *_: obj + "\0",
+        )
 
 
-# TODO Due to construct's poor implementation of LazyStruct, this is no longer lazy
-class StructEventBase(DataEventBase):
+class StructEventBase(EventBase[c.Container[Any]], UserDict[str, Any]):
     """Base class for events used for storing fixed size structured data.
 
     Consists of a collection of POD types like int, bool, float, but not strings.
     Its size is determined by the event as well as FL version.
     """
 
-    STRUCT: ClassVar[c.Construct[c.Container[Any], Any]]
-
     def __init__(self, id: EventEnum, data: bytes) -> None:
-        super().__init__(id, data)
-        self._struct = self.STRUCT.parse(data, len=len(self._data))
-
-    def __bytes__(self) -> bytes:
-        # pylint: disable=access-member-before-definition
-        # pylint: disable=attribute-defined-outside-init
-        new_data = self.STRUCT.build(self._struct, len=len(self._data))
-        if len(new_data) != len(self._data):
-            warnings.warn(
-                "{} built a stream of incorrect size {}; expected {}.".format(
-                    type(self).__name__, len(new_data), len(self._data)
-                ),
-                BytesWarning,
-                stacklevel=0,
-            )
-        # Effectively, overwrite new data over old one to ensure the stream
-        # size remains unmodified
-        self._data = new_data + self._data[len(new_data) :]
-        return super().__bytes__()
-
-    def __contains__(self, prop: str) -> bool:
-        return prop in self._struct
-
-    def __getitem__(self, key: str):
-        return self._struct[key]
+        super().__init__(id, data, len=len(data))
+        self.data = self.value  # Akin to UserDict.__init__
 
     def __setitem__(self, key: str, value: Any) -> None:
-        if key not in self or self[key] is None:
-            raise PropertyCannotBeSet
-        self._struct[key] = value
-
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}(id={self.id}, size={len(self._data)})"
+        if key not in self:
+            raise KeyError
 
-    @property  # type: ignore[override]
-    def value(self) -> NoReturn:
-        raise NotImplementedError
+        if self[key] is None:
+            raise PropertyCannotBeSet
 
-    @value.setter
-    def value(self, value: bytes) -> NoReturn:
-        raise NotImplementedError
+        self.data[key] = value
 
 
-class ListEventBase(DataEventBase):
+class ListEventBase(EventBase[c.ListContainer[Any]], UserList[c.Container[Any]]):
     """Base class for events storing an array of structured data.
 
     Attributes:
         kwds: Keyword args passed to :meth:`STRUCT.parse` & :meth:`STRUCT.build`.
     """
 
-    STRUCT: ClassVar[c.Construct[c.Container[Any], Any]]
+    STRUCT: c.Subconstruct[Any, Any, Any, Any]
     SIZES: ClassVar[list[int]] = []
     """Manual :meth:`STRUCT.sizeof` override(s)."""
 
     def __init__(self, id: EventEnum, data: bytes, **kwds: Any) -> None:
-        super().__init__(id, data)
+        super().__init__(id, data, **kwds)
         self._struct_size: int | None = None
-        self.kwds = kwds
 
         if not self.SIZES:
-            self._struct_size = self.STRUCT.sizeof()
+            self._struct_size = self.STRUCT.subcon.sizeof()
 
         for size in self.SIZES:
             if not len(data) % size:
                 self._struct_size = size
                 break
 
         if self._struct_size is None:  # pragma: no cover
             warnings.warn(
                 f"Cannot parse event {id} as event size {len(data)} "
                 f"is not a multiple of struct size(s) {self.SIZES}"
             )
+        else:
+            self.data = self.value  # Akin to UserList.__init__
 
-    def __len__(self) -> int:
-        if self._struct_size is None:  # pragma: no cover
-            raise ListEventNotParsed
-
-        return len(self._data) // self._struct_size
-
-    def __getitem__(self, index: int) -> c.Container[Any]:
-        if self._struct_size is None:  # pragma: no cover
-            raise ListEventNotParsed
 
-        if index > len(self):
-            raise IndexError(index)
-
-        start = self._struct_size * index
-        count = self._struct_size
-        return self.STRUCT.parse(self._data[start : start + count], **self.kwds)
-
-    def __setitem__(self, index: int, item: c.Container[Any]) -> None:
-        if self._struct_size is None:
-            raise ListEventNotParsed
-
-        if index > len(self):
-            raise IndexError(index)
-
-        start = self._struct_size * index
-        count = self._struct_size
-        self._data = (  # pylint: disable=attribute-defined-outside-init
-            self._data[:start]
-            + self.STRUCT.build(item, **self.kwds)
-            + self._data[start + count :]
-        )
-
-    def __iter__(self) -> Iterator[c.Container[Any]]:
-        for i in range(len(self)):
-            yield self[i]
-
-    def __repr__(self) -> str:
-        return "{}(id={}, size={}, {} items)".format(
-            type(self).__name__, self.id, len(self._data), len(self)
-        )
-
-
-class UnknownDataEvent(DataEventBase):
+class UnknownDataEvent(EventBase[bytes]):
     """Used for events whose structure is unknown as of yet."""
 
-    @property
-    def value(self) -> bytes:
-        return self._data
-
-    @value.setter
-    def value(self, value: bytes) -> None:
-        self._data = value
+    STRUCT = c.GreedyBytes
 
 
 @dataclass(order=True)
 class IndexedEvent:
     r: int
     """Root index of occurence of :attr:`e`."""
 
@@ -757,15 +581,15 @@
         """
         el: list[IndexedEvent] = []
         for ie in self.lst:
             if not repeat:
                 return
 
             result = select(ie.e)
-            if result is False:  # pylint: disable=compare-to-zero
+            if result is False:
                 yield EventTree(self, el)
                 el = [ie]  # Don't skip current event
                 repeat -= 1
             elif result is not None:
                 el.append(ie)
 
     @property
```

### Comparing `pyflp-2.1.1/pyflp/_models.py` & `pyflp-2.2.0/pyflp/_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,44 +12,44 @@
 # <https://www.gnu.org/licenses/>.
 
 """Contains the ABCs used by model classes and some shared classes."""
 
 from __future__ import annotations
 
 import abc
-import dataclasses
 import functools
-import sys
-from typing import Any, Callable, Generic, Iterable, Sequence, TypeVar, overload
-
-if sys.version_info >= (3, 8):
-    from typing import Protocol, runtime_checkable
-else:
-    from typing_extensions import Protocol, runtime_checkable
+from typing import (
+    Any,
+    Callable,
+    Generic,
+    Iterable,
+    Protocol,
+    Sequence,
+    TypeVar,
+    Union,
+    overload,
+    runtime_checkable,
+)
 
 import construct as c
 
-from ._events import DataEventBase, EventTree, ListEventBase
+from pyflp._events import EventTree, ListEventBase, StructEventBase
 
-DE = TypeVar("DE", bound=DataEventBase)
+VE = TypeVar("VE", bound=Union[StructEventBase, ListEventBase])
 
 
 class ModelBase(abc.ABC):
-    def __init__(
-        self, *args: Any, **kw: Any
-    ) -> None:  # pylint: disable=unused-argument
+    def __init__(self, *args: Any, **kw: Any) -> None:
         self._kw = kw
 
 
-class ItemModel(ModelBase, Generic[DE]):
+class ItemModel(ModelBase, Generic[VE]):
     """Base class for event-less models."""
 
-    def __init__(
-        self, item: c.Container[Any], index: int, parent: DE, **kw: Any
-    ) -> None:
+    def __init__(self, item: c.Container[Any], index: int, parent: VE, **kw: Any) -> None:
         """Create a new item model.
 
         Args:
             item: Parsed :class:`construct.Struct` instance from :attr:`parent`.
             index: 0-based index used to propagate changes back to :attr:`parent`.
             parent: A :class:`StructEventBase` or :class:`ListEventBase` instance.
         """
@@ -83,17 +83,15 @@
 
 
 MT_co = TypeVar("MT_co", bound=ModelBase, covariant=True)
 EMT_co = TypeVar("EMT_co", bound=EventModel, covariant=True)
 
 
 @runtime_checkable
-class ModelCollection(  # pylint: disable=abstract-method
-    Iterable[MT_co], Protocol[MT_co]
-):
+class ModelCollection(Iterable[MT_co], Protocol[MT_co]):
     @overload
     def __getitem__(self, i: int | str) -> MT_co:
         ...
 
     @overload
     def __getitem__(self, i: slice) -> Sequence[MT_co]:
         ...
@@ -109,17 +107,15 @@
     @overload
     def wrapper(self: ModelCollection[MT_co], i: slice) -> Sequence[MT_co]:
         ...
 
     @functools.wraps(func)
     def wrapper(self: Any, i: Any) -> MT_co | Sequence[MT_co]:
         if isinstance(i, slice):
-            return [
-                model for idx, model in enumerate(self) if idx in range(i.start, i.stop)
-            ]
+            return [model for idx, model in enumerate(self) if idx in range(i.start, i.stop)]
         return func(self, i)
 
     return wrapper
 
 
 class ModelReprMixin:
     """I am too lazy to make one `__repr__()` for every model."""
@@ -127,21 +123,7 @@
     def __repr__(self) -> str:
         mapping: dict[str, Any] = {}
         for var in [var for var in vars(type(self)) if not var.startswith("_")]:
             mapping[var] = getattr(self, var, None)
 
         params = ", ".join([f"{k}={v!r}" for k, v in mapping.items()])
         return f"{type(self).__name__}({params})"
-
-
-@dataclasses.dataclass(frozen=True, order=True)
-class FLVersion:
-    major: int
-    minor: int = 0
-    patch: int = 0
-    build: int | None = None
-
-    def __str__(self) -> str:
-        version = f"{self.major}.{self.minor}.{self.patch}"
-        if self.build is not None:
-            return f"{version}.{self.build}"
-        return version
```

### Comparing `pyflp-2.1.1/pyflp/arrangement.py` & `pyflp-2.2.0/pyflp/arrangement.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,94 +12,82 @@
 # <https://www.gnu.org/licenses/>.
 
 """Contains the types used by tracks and arrangements."""
 
 from __future__ import annotations
 
 import enum
-import sys
-from typing import Any, Iterator, Optional, cast
+from typing import Any, Iterator, Literal, Optional, cast
 
-if sys.version_info >= (3, 8):
-    from typing import Literal, TypedDict
-else:
-    from typing_extensions import Literal, TypedDict
-
-if sys.version_info >= (3, 11):
-    from typing import Unpack
-else:
-    from typing_extensions import Unpack
-
-import colour
 import construct as c
 import construct_typed as ct
+from typing_extensions import TypedDict, Unpack
 
-from ._descriptors import EventProp, NestedProp, StdEnum, StructProp
-from ._events import (
+from pyflp._adapters import FourByteBool, StdEnum
+from pyflp._descriptors import EventProp, NestedProp, StructProp
+from pyflp._events import (
     DATA,
     DWORD,
     TEXT,
     WORD,
     AnyEvent,
-    ColorEvent,
     EventEnum,
     EventTree,
-    FourByteBool,
     ListEventBase,
     StructEventBase,
     U8Event,
     U16Event,
     U16TupleEvent,
 )
-from ._models import (
+from pyflp._models import (
     EventModel,
-    FLVersion,
     ItemModel,
     ModelCollection,
     ModelReprMixin,
     supports_slice,
 )
-from .channel import Channel, ChannelRack
-from .exceptions import ModelNotFound, NoModelsFound, PropertyCannotBeSet
-from .pattern import Pattern, Patterns
-from .timemarker import TimeMarker, TimeMarkerID
+from pyflp.channel import Channel, ChannelRack
+from pyflp.exceptions import ModelNotFound, NoModelsFound, PropertyCannotBeSet
+from pyflp.pattern import Pattern, Patterns
+from pyflp.timemarker import TimeMarker, TimeMarkerID
+from pyflp.types import RGBA, FLVersion
 
 __all__ = [
     "Arrangements",
     "Arrangement",
     "Track",
     "TrackMotion",
     "TrackPress",
     "TrackSync",
     "ChannelPLItem",
     "PatternPLItem",
 ]
 
 
 class PLSelectionEvent(StructEventBase):
-    STRUCT = c.Struct(
-        "start" / c.Optional(c.Int32ul), "end" / c.Optional(c.Int32ul)
-    ).compile()
+    STRUCT = c.Struct("start" / c.Optional(c.Int32ul), "end" / c.Optional(c.Int32ul)).compile()
 
 
 class PlaylistEvent(ListEventBase):
-    STRUCT = c.Struct(
-        "position" / c.Int32ul,  # 4
-        "pattern_base" / c.Int16ul * "Always 20480",  # 6
-        "item_index" / c.Int16ul,  # 8
-        "length" / c.Int32ul,  # 12
-        "track_rvidx" / c.Int16ul * "Stored reversed i.e. Track 1 would be 499",  # 14
-        "group" / c.Int16ul,  # 16
-        "_u1" / c.Bytes(2) * "Always (120, 0)",  # 18
-        "item_flags" / c.Int16ul * "Always (64, 0)",  # 20
-        "_u2" / c.Bytes(4) * "Always (64, 100, 128, 128)",  # 24
-        "start_offset" / c.Float32l,  # 28
-        "end_offset" / c.Float32l,  # 32
-        "_u3" / c.If(c.this._params["new"], c.Bytes(28)) * "New in FL 21",  # 60
-    ).compile()
+    STRUCT = c.GreedyRange(
+        c.Struct(
+            "position" / c.Int32ul,  # 4
+            "pattern_base" / c.Int16ul * "Always 20480",  # 6
+            "item_index" / c.Int16ul,  # 8
+            "length" / c.Int32ul,  # 12
+            "track_rvidx" / c.Int16ul * "Stored reversed i.e. Track 1 would be 499",  # 14
+            "group" / c.Int16ul,  # 16
+            "_u1" / c.Bytes(2) * "Always (120, 0)",  # 18
+            "item_flags" / c.Int16ul * "Always (64, 0)",  # 20
+            "_u2" / c.Bytes(4) * "Always (64, 100, 128, 128)",  # 24
+            "start_offset" / c.Float32l,  # 28
+            "end_offset" / c.Float32l,  # 32
+            "_u3" / c.If(c.this._params["new"], c.Bytes(28)) * "New in FL 21",  # 60
+        )
+    )
     SIZES = [32, 60]
 
     def __init__(self, id: EventEnum, data: bytes) -> None:
         super().__init__(id, data, new=not len(data) % 60)
 
 
 @enum.unique
@@ -239,23 +227,22 @@
 
     @pattern.setter
     def pattern(self, pattern: Pattern) -> None:
         self._kw["pattern"] = pattern
         self["item_index"] = pattern.iid + self["pattern_base"]
 
 
-class _TrackColorProp(StructProp[colour.Color]):
-    def _get(self, ev_or_ins: Any) -> colour.Color | None:
+class _TrackColorProp(StructProp[RGBA]):
+    def _get(self, ev_or_ins: Any) -> RGBA | None:
         value = cast(Optional[int], super()._get(ev_or_ins))
         if value is not None:
-            return ColorEvent.decode(bytearray(value.to_bytes(4, "little")))
+            return RGBA.from_bytes(value.to_bytes(4, "little"))
 
-    def _set(self, ev_or_ins: Any, value: colour.Color) -> None:
-        color_u32 = int.from_bytes(ColorEvent.encode(value), "little")
-        super()._set(ev_or_ins, color_u32)  # type: ignore
+    def _set(self, ev_or_ins: Any, value: RGBA) -> None:
+        super()._set(ev_or_ins, int.from_bytes(bytes(value), "little"))  # type: ignore
 
 
 class _TrackKW(TypedDict):
     items: list[PLItemBase]
 
 
 class Track(EventModel, ModelCollection[PLItemBase]):
@@ -381,27 +368,29 @@
 
     @property
     def timemarkers(self) -> Iterator[TimeMarker]:
         yield from (TimeMarker(ed) for ed in self.events.group(*TimeMarkerID))
 
     @property
     def tracks(self) -> Iterator[Track]:
-        pl_evt = raw_items = None
+        pl_evt = None
         max_idx = 499 if self._kw["version"] >= FLVersion(12, 9, 1) else 198
         channels = {channel.iid: channel for channel in self._kw["channels"]}
         patterns = {pattern.iid: pattern for pattern in self._kw["patterns"]}
 
         if ArrangementID.Playlist in self.events.ids:
             pl_evt = cast(PlaylistEvent, self.events.first(ArrangementID.Playlist))
-            raw_items = tuple(pl_evt)  # Repeating this is quite slow
 
         for track_idx, ed in enumerate(self.events.divide(TrackID.Data, *TrackID)):
+            if pl_evt is None:
+                yield Track(ed, items=[])
+                continue
+
             items: list[PLItemBase] = []
-            for i, item in enumerate(raw_items or []):
-                pl_evt = cast(PlaylistEvent, pl_evt)
+            for i, item in enumerate(pl_evt):
                 if max_idx - item["track_rvidx"] != track_idx:
                     continue
 
                 if item["item_index"] <= item["pattern_base"]:
                     iid = item["item_index"]
                     items.append(ChannelPLItem(item, i, pl_evt, channel=channels[iid]))
                 else:
@@ -483,18 +472,15 @@
 
             if e.id in (*ArrangementID, *TimeMarkerID, *TrackID):
                 return True
 
             if e.id == ArrangementsID.Current:
                 return False  # Yield out last arrangement
 
-        yield from (
-            Arrangement(ed, **self._kw)
-            for ed in self.events.subtrees(select, len(self))
-        )
+        yield from (Arrangement(ed, **self._kw) for ed in self.events.subtrees(select, len(self)))
 
     def __len__(self) -> int:
         """The number of arrangements present in the project.
 
         Raises:
             NoModelsFound: When no arrangements are found.
         """
@@ -529,35 +515,29 @@
 
            :attr:`ArrangementsID.PLSelection` is used by default
            while :attr:`ArrangementsID._LoopPos` is a fallback.
 
         *New in FL Studio v1.3.8*.
         """
         if ArrangementsID.PLSelection in self.events:
-            event = cast(
-                PLSelectionEvent, self.events.first(ArrangementsID.PLSelection)
-            )
+            event = cast(PLSelectionEvent, self.events.first(ArrangementsID.PLSelection))
             return event["start"], event["end"]
 
         if ArrangementsID._LoopPos in self.events:
             return self.events.first(ArrangementsID._LoopPos).value
 
     @loop_pos.setter
     def loop_pos(self, value: tuple[int, int]) -> None:
         if ArrangementsID.PLSelection in self.events:
-            event = cast(
-                PLSelectionEvent, self.events.first(ArrangementsID.PLSelection)
-            )
+            event = cast(PLSelectionEvent, self.events.first(ArrangementsID.PLSelection))
             event["start"], event["end"] = value
         elif ArrangementsID._LoopPos in self.events:
             self.events.first(ArrangementsID._LoopPos).value = value
         else:
-            raise PropertyCannotBeSet(
-                ArrangementsID.PLSelection, ArrangementsID._LoopPos
-            )
+            raise PropertyCannotBeSet(ArrangementsID.PLSelection, ArrangementsID._LoopPos)
 
     @property
     def max_tracks(self) -> Literal[500, 199]:
         return 500 if self._kw["version"] >= FLVersion(12, 9, 1) else 199
 
     time_signature = NestedProp(
         TimeSignature, ArrangementsID.TimeSigNum, ArrangementsID.TimeSigBeat
```

### Comparing `pyflp-2.1.1/pyflp/channel.py` & `pyflp-2.2.0/pyflp/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,39 +13,22 @@
 
 """Contains the types used by channels and the channel rack."""
 
 from __future__ import annotations
 
 import enum
 import pathlib
-import sys
-from typing import Any, Iterator, Tuple, cast
+from typing import Any, Iterator, Literal, Tuple, cast
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
-import colour
 import construct as c
 import construct_typed as ct
 
-from ._descriptors import (
-    EventProp,
-    FlagProp,
-    LinearMusical,
-    List2Tuple,
-    Log2,
-    LogNormal,
-    MusicalTime,
-    NestedProp,
-    StdEnum,
-    StructProp,
-)
-from ._events import (
+from pyflp._adapters import LinearMusical, List2Tuple, Log2, LogNormal, StdEnum
+from pyflp._descriptors import EventProp, FlagProp, NestedProp, StructProp
+from pyflp._events import (
     DATA,
     DWORD,
     TEXT,
     WORD,
     BoolEvent,
     EventEnum,
     F32Event,
@@ -53,23 +36,18 @@
     I32Event,
     StructEventBase,
     U8Event,
     U16Event,
     U16TupleEvent,
     U32Event,
 )
-from ._models import (
-    EventModel,
-    ItemModel,
-    ModelCollection,
-    ModelReprMixin,
-    supports_slice,
-)
-from .exceptions import ModelNotFound, NoModelsFound, PropertyCannotBeSet
-from .plugin import BooBass, FruitKick, Plucked, PluginID, PluginProp, VSTPlugin
+from pyflp._models import EventModel, ItemModel, ModelCollection, ModelReprMixin, supports_slice
+from pyflp.exceptions import ModelNotFound, NoModelsFound, PropertyCannotBeSet
+from pyflp.plugin import BooBass, FruitKick, Plucked, PluginID, PluginProp, VSTPlugin
+from pyflp.types import RGBA, MusicalTime
 
 __all__ = [
     "ArpDirection",
     "Automation",
     "AutomationPoint",
     "Channel",
     "Instrument",
@@ -125,17 +103,15 @@
         / c.PrefixedArray(
             c.Int32ul,  # 21
             c.Struct(
                 "_offset" / c.Float64l * "Change in X-axis w.r.t last point",
                 "position"  # TODO Implement a setter
                 / c.IfThenElse(
                     lambda ctx: ctx._index > 0,
-                    c.Computed(
-                        lambda ctx: AutomationEvent._get_position(ctx._io, ctx._index)
-                    ),
+                    c.Computed(lambda ctx: AutomationEvent._get_position(ctx._io, ctx._index)),
                     c.Computed(lambda ctx: ctx["_offset"]),
                 ),
                 "value" / c.Float64l,
                 "tension" / c.Float32l,
                 "_u1" / c.Bytes(4),  # Linked to tension
             ),  # 24 per struct
         ),
@@ -1078,17 +1054,15 @@
     """Whether to add root note (instead of pitch) to triggered note.
 
     Named as :guilabel:`Add to key`. Defaults to ``False``.
 
     *New in FL Studio v3.4.0*.
     """
 
-    key_region = StructProp[Tuple[int, int]](
-        ChannelID.Parameters, prop="keyboard.key_region"
-    )
+    key_region = StructProp[Tuple[int, int]](ChannelID.Parameters, prop="keyboard.key_region")
     """A `(start_note, end_note)` tuple representing the playable range."""
 
 
 class Playback(EventModel, ModelReprMixin):
     """Used by :class:`Sampler`.
 
     ![](https://bit.ly/3xjSypY)
@@ -1135,17 +1109,15 @@
 
 class Content(EventModel, ModelReprMixin):
     """Used by :class:`Sampler`.
 
     ![](https://bit.ly/3TCXFKI)
     """
 
-    declick_mode = StructProp[DeclickMode](
-        ChannelID.Parameters, prop="content.declick_mode"
-    )
+    declick_mode = StructProp[DeclickMode](ChannelID.Parameters, prop="content.declick_mode")
     """Defaults to ``DeclickMode.OutOnly``.
 
     *New in FL Studio v9.0.0*.
     """
 
     keep_on_disk = FlagProp(_SamplerFlags.KeepOnDisk, ChannelID.SamplerFlags)
     """Whether a sample is streamed from disk or kept in RAM, defaults to ``False``.
@@ -1198,15 +1170,15 @@
 
 class Channel(EventModel):
     """Represents a channel in the channel rack."""
 
     def __repr__(self) -> str:
         return f"{type(self).__name__} (name={self.display_name!r}, iid={self.iid})"
 
-    color = EventProp[colour.Color](PluginID.Color)
+    color = EventProp[RGBA](PluginID.Color)
     """Defaults to #5C656A (granite gray).
 
     ![](https://bit.ly/3SllDsG)
 
     Values below 20 for any color component (R, G or B) are ignored by FL.
     """
 
@@ -1234,17 +1206,15 @@
     icon = EventProp[int](PluginID.Icon)
     """Internal ID of the icon shown beside the ``display_name``.
 
     ![](https://bit.ly/3zjK2sf)
     """
 
     iid = EventProp[int](ChannelID.New)
-    keyboard = NestedProp(
-        Keyboard, ChannelID.FineTune, ChannelID.RootNote, ChannelID.Parameters
-    )
+    keyboard = NestedProp(Keyboard, ChannelID.FineTune, ChannelID.RootNote, ChannelID.Parameters)
     """Located at the bottom of :menuselection:`Miscellaneous functions (page)`."""
 
     locked = EventProp[bool](ChannelID.IsLocked)
     """Whether in a locked state or not; mute / solo acts differently when ``True``.
 
     ![](https://bit.ly/3BOBc7j)
     """
@@ -1417,17 +1387,15 @@
 
     :menuselection:`Miscellaneous functions --> Group`
 
     Hint:
         To cut itself when retriggered, set the same value for both.
     """
 
-    delay = NestedProp(
-        Delay, ChannelID.Delay, ChannelID.DelayModXY, ChannelID.Parameters
-    )
+    delay = NestedProp(Delay, ChannelID.Delay, ChannelID.DelayModXY, ChannelID.Parameters)
     """:menuselection:`Miscellaneous functions -> Echo delay / fat mode`"""
 
     insert = EventProp[int](ChannelID.RoutedTo)
     """The index of the :class:`Insert` the channel is routed to according to FL.
 
     "Current" insert = -1, Master = 0 and so on... till :attr:`Mixer.max_inserts`.
     """
@@ -1595,15 +1563,14 @@
         groups = [DisplayGroup(et) for et in self.events.separate(DisplayGroupID.Name)]
 
         for et in self.events.divide(ChannelID.New, *ChannelID, *PluginID):
             iid = et.first(ChannelID.New).value
             typ = et.first(ChannelID.Type).value
             groupnum = et.first(ChannelID.GroupNum).value
 
-            # pylint: disable=redefined-outer-name
             ct = Channel  # prevent type error and logic failure below
             if typ == ChannelType.Automation:
                 ct = Automation
             elif typ == ChannelType.Layer:
                 ct = Layer
             elif typ == ChannelType.Sampler:
                 ct = Sampler
```

### Comparing `pyflp-2.1.1/pyflp/controller.py` & `pyflp-2.2.0/pyflp/controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from __future__ import annotations
 
 import enum
 from typing import cast
 
 import construct as c
 
-from ._events import DATA, EventEnum, StructEventBase
-from ._models import EventModel, ModelReprMixin
+from pyflp._events import DATA, EventEnum, StructEventBase
+from pyflp._models import EventModel, ModelReprMixin
 
 __all__ = ["RemoteController"]
 
 
 class MIDIControllerEvent(StructEventBase):
     STRUCT = c.Struct("_u1" / c.GreedyBytes)
 
@@ -53,24 +53,24 @@
 
     *New in FL Studio v3.3.0*.
     """
 
     @property
     def parameter(self) -> int | None:
         """The ID of the plugin parameter to which controller is linked to."""
-        value = cast(StructEventBase, self.events.first(ControllerID.Remote))[
-            "parameter_data"
-        ]
-        if value is not None:
+        if (
+            value := cast(StructEventBase, self.events.first(ControllerID.Remote))["parameter_data"]
+            is not None
+        ):
             return value & 0x7FFF
 
     @property
     def controls_vst(self) -> bool | None:
         """Whether `parameter` is linked to a VST plugin.
 
         None when linked to a plugin parameter on an insert slot.
         """
-        value = cast(StructEventBase, self.events.first(ControllerID.Remote))[
-            "parameter_data"
-        ]
-        if value is not None:
+        if (
+            value := cast(StructEventBase, self.events.first(ControllerID.Remote))["parameter_data"]
+            is not None
+        ):
             return (value & 0x8000) > 0
```

### Comparing `pyflp-2.1.1/pyflp/exceptions.py` & `pyflp-2.2.0/pyflp/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,29 +40,25 @@
     Some exceptions derive from standard Python exceptions to ease handling.
     """
 
 
 class EventIDOutOfRange(Error, ValueError):
     """An event is created with an ID out of its allowed range."""
 
-    def __init__(self, id: int, min_i: int, max_e: int) -> None:
-        super().__init__(f"Expected ID in {min_i}-{max_e - 1}; got {id} instead")
+    def __init__(self, id: int, *expected: int) -> None:
+        super().__init__(f"Expected ID in {expected!r}; got {id!r} instead")
 
 
 class InvalidEventChunkSize(Error, BufferError):
     """A fixed size event is created with a wrong amount of bytes."""
 
     def __init__(self, expected: int, got: int) -> None:
         super().__init__(f"Expected a bytes object of length {expected}; got {got}")
 
 
-class ListEventNotParsed(Error, AttributeError, IndexError):
-    """`ListEventBase` could not be parsed due to mismatching struct layouts."""
-
-
 class PropertyCannotBeSet(Error, AttributeError):
     def __init__(self, *ids: enum.Enum | int) -> None:
         super().__init__(f"Event(s) {ids!r} was / were not found")
 
 
 class DataCorrupted(Error):
     """Base class for parsing exceptions."""
```

### Comparing `pyflp-2.1.1/pyflp/mixer.py` & `pyflp-2.2.0/pyflp/mixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,90 +13,57 @@
 
 """Contains the types used by the mixer, inserts and effect slots."""
 
 from __future__ import annotations
 
 import dataclasses
 import enum
-import sys
-import warnings
 from collections import defaultdict
 from typing import Any, DefaultDict, Iterator, NamedTuple, cast
 
-if sys.version_info >= (3, 8):
-    from typing import TypedDict
-else:
-    from typing_extensions import TypedDict
-
-if sys.version_info >= (3, 11):
-    from typing import NotRequired, Unpack
-else:
-    from typing_extensions import NotRequired, Unpack
-
-import colour
 import construct as c
 import construct_typed as ct
+from typing_extensions import NotRequired, TypedDict, Unpack
 
-from ._descriptors import (
-    EventProp,
-    FlagProp,
-    NamedPropMixin,
-    ROProperty,
-    RWProperty,
-    StdEnum,
-)
-from ._events import (
+from pyflp._adapters import StdEnum
+from pyflp._descriptors import EventProp, FlagProp, NamedPropMixin, ROProperty, RWProperty
+from pyflp._events import (
     DATA,
     DWORD,
     TEXT,
     WORD,
     AnyEvent,
     ColorEvent,
-    DataEventBase,
     EventEnum,
     EventTree,
     I16Event,
     I32Event,
     ListEventBase,
     StructEventBase,
-    T,
     U16Event,
 )
-from ._models import (
-    EventModel,
-    FLVersion,
-    ModelBase,
-    ModelCollection,
-    ModelReprMixin,
-    supports_slice,
-)
-from .exceptions import ModelNotFound, NoModelsFound, PropertyCannotBeSet
-from .plugin import (
+from pyflp._models import EventModel, ModelBase, ModelCollection, ModelReprMixin, supports_slice
+from pyflp.exceptions import ModelNotFound, NoModelsFound, PropertyCannotBeSet
+from pyflp.plugin import (
     FruityBalance,
     FruityBloodOverdrive,
     FruityCenter,
     FruityFastDist,
     FruityNotebook2,
     FruitySend,
     FruitySoftClipper,
     FruityStereoEnhancer,
     PluginID,
     PluginProp,
     Soundgoodizer,
     VSTPlugin,
 )
+from pyflp.types import RGBA, FLVersion, T
 
-__all__ = [
-    "Insert",
-    "InsertDock",
-    "InsertEQ",
-    "InsertEQBand",
-    "Mixer",
-    "Slot",
-]
+__all__ = ["Insert", "InsertDock", "InsertEQ", "InsertEQBand", "Mixer", "Slot"]
 
 
 @enum.unique
 class _InsertFlags(enum.IntFlag):
     None_ = 0
     PolarityReversed = 1 << 0
     SwapLeftRight = 1 << 1
@@ -140,59 +107,50 @@
         "_u1" / c.Optional(c.Bytes(4)),  # 4
         "flags" / c.Optional(StdEnum[_InsertFlags](c.Int32ul)),  # 8
         "_u2" / c.Optional(c.Bytes(4)),  # 12
     ).compile()
 
 
 class InsertRoutingEvent(ListEventBase):
-    STRUCT = c.Struct("is_routed" / c.Flag).compile()
+    STRUCT = c.GreedyRange(c.Flag)
 
 
 @dataclasses.dataclass
 class _InsertItems:
     slots: DefaultDict[int, dict[int, dict[str, Any]]] = dataclasses.field(
         default_factory=lambda: defaultdict(dict)
     )
     own: dict[int, dict[str, Any]] = dataclasses.field(default_factory=dict)
 
 
-class MixerParamsEvent(DataEventBase):
-    STRUCT = c.Struct(
-        "_u4" / c.Bytes(4),  # 4
-        "id" / StdEnum[_MixerParamsID](c.Byte),  # 5
-        "_u1" / c.Byte,  # 6
-        "channel_data" / c.Int16ul,  # 8
-        "msg" / c.Int32sl,  # 12
-    ).compile()
-    STRUCT_SIZE = STRUCT.sizeof()
+class MixerParamsEvent(ListEventBase):
+    STRUCT = c.GreedyRange(
+        c.Struct(
+            "_u4" / c.Bytes(4),  # 4
+            "id" / StdEnum[_MixerParamsID](c.Byte),  # 5
+            "_u1" / c.Byte,  # 6
+            "channel_data" / c.Int16ul,  # 8
+            "msg" / c.Int32sl,  # 12
+        )
+    )
 
     def __init__(self, id: Any, data: bytearray) -> None:
         super().__init__(id, data)
-        self.items: DefaultDict[int, _InsertItems] = defaultdict(_InsertItems)
-        self.unparsed = False
+        self.items_: DefaultDict[int, _InsertItems] = defaultdict(_InsertItems)
 
-        if not len(data) % self.STRUCT_SIZE:
-            for i in range(len(data) // self.STRUCT_SIZE):
-                offset = self.STRUCT_SIZE * i
-                item = self.STRUCT.parse(data[offset : offset + self.STRUCT_SIZE])
-                insert_idx = (item["channel_data"] >> 6) & 0x7F
-                slot_idx = item["channel_data"] & 0x3F
-                insert = self.items[insert_idx]
-                id = item["id"]
+        for item in self.data:
+            insert_idx = (item["channel_data"] >> 6) & 0x7F
+            slot_idx = item["channel_data"] & 0x3F
+            insert = self.items_[insert_idx]
+            id = item["id"]
 
-                if id in (_MixerParamsID.SlotEnabled, _MixerParamsID.SlotMix):
-                    insert.slots[slot_idx][id] = item
-                else:
-                    insert.own[id] = item
-        else:
-            self.unparsed = True
-            warnings.warn(
-                f"Cannot parse event {id} as event "
-                "size is not a multiple of struct size"
-            )
+            if id in (_MixerParamsID.SlotEnabled, _MixerParamsID.SlotMix):
+                insert.slots[slot_idx][id] = item
+            else:
+                insert.own[id] = item
 
 
 @enum.unique
 class InsertID(EventEnum):
     Icon = (WORD + 31, I16Event)
     Output = (DWORD + 19, I32Event)
     Color = (DWORD + 21, ColorEvent)  #: 4.0+
@@ -244,15 +202,15 @@
 
 class InsertEQBand(ModelBase, ModelReprMixin):
     def __init__(self, **kw: Unpack[_InsertEQBandKW]) -> None:
         super().__init__(**kw)
 
     @property
     def size(self) -> int:
-        return MixerParamsEvent.STRUCT_SIZE * len(self._kw)
+        return 12 * len(self._kw)  # ! TODO
 
     gain = _InsertEQBandProp()
     """
     | Min   | Max  | Default |
     |-------|------|---------|
     | -1800 | 1800 | 0       |
     """
@@ -311,40 +269,34 @@
     """
 
     def __init__(self, params: _InsertItems) -> None:
         super().__init__(params=params)
 
     @property
     def size(self) -> int:
-        return MixerParamsEvent.STRUCT_SIZE * self._kw["param"]
+        return 12 * self._kw["param"]  # ! TODO
 
     low = _InsertEQProp(
-        _InsertEQPropArgs(
-            _MixerParamsID.LowFreq, _MixerParamsID.LowGain, _MixerParamsID.LowQ
-        )
+        _InsertEQPropArgs(_MixerParamsID.LowFreq, _MixerParamsID.LowGain, _MixerParamsID.LowQ)
     )
     """Low shelf band. Default frequency - 5777 (90 Hz)."""
 
     mid = _InsertEQProp(
-        _InsertEQPropArgs(
-            _MixerParamsID.MidFreq, _MixerParamsID.MidGain, _MixerParamsID.MidQ
-        )
+        _InsertEQPropArgs(_MixerParamsID.MidFreq, _MixerParamsID.MidGain, _MixerParamsID.MidQ)
     )
     """Middle band. Default frequency - 33145 (1500 Hz)."""
 
     high = _InsertEQProp(
-        _InsertEQPropArgs(
-            _MixerParamsID.HighFreq, _MixerParamsID.HighGain, _MixerParamsID.HighQ
-        )
+        _InsertEQPropArgs(_MixerParamsID.HighFreq, _MixerParamsID.HighGain, _MixerParamsID.HighQ)
     )
     """High shelf band. Default frequency - 55825 (8000 Hz)."""
 
 
 class _MixerParamProp(RWProperty[T]):
-    def __init__(self, id: int) -> None:  # pylint: disable=super-init-not-called
+    def __init__(self, id: int) -> None:
         self._id = id
 
     def __get__(self, ins: Insert, owner: object = None) -> T | None:
         if owner is None:
             return NotImplemented
 
         for id, item in cast(_InsertItems, ins._kw["params"]).own.items():
@@ -361,23 +313,21 @@
 
 class Slot(EventModel):
     """Represents an effect slot in an `Insert` / mixer channel.
 
     ![](https://bit.ly/3RUDtTu)
     """
 
-    def __init__(
-        self, events: EventTree, params: list[dict[str, Any]] | None = None
-    ) -> None:
+    def __init__(self, events: EventTree, params: list[dict[str, Any]] | None = None) -> None:
         super().__init__(events, params=params or [])
 
     def __repr__(self) -> str:
         return f"Slot (name={self.name}, iid={self.index}, plugin={self.plugin!r})"
 
-    color = EventProp[colour.Color](PluginID.Color)
+    color = EventProp[RGBA](PluginID.Color)
     # TODO controllers = KWProp[List[RemoteController]]()
     iid = EventProp[int](SlotID.Index)
     """A 0-based internal index."""
 
     internal_name = EventProp[str](PluginID.InternalName)
     """'Fruity Wrapper' for VST/AU plugins or factory name for native plugins."""
 
@@ -470,15 +420,15 @@
 
     bypassed = FlagProp(_InsertFlags.EnableEffects, InsertID.Flags, inverted=True)
     """Whether all slots are bypassed."""
 
     channels_swapped = FlagProp(_InsertFlags.SwapLeftRight, InsertID.Flags)
     """Whether the left and right channels are swapped."""
 
-    color = EventProp[colour.Color](InsertID.Color)
+    color = EventProp[RGBA](InsertID.Color)
     """Defaults to #636C71 (granite gray) in FL Studio.
 
     ![](https://bit.ly/3yVKXPc)
 
     Values below 20 for any color component (R, G, B) are ignored by FL.
 
     *New in FL Studio v4.0*.
@@ -563,15 +513,15 @@
 
         *New in FL Studio v4.0*.
         """
         items = iter(cast(InsertRoutingEvent, self.events.first(InsertID.Routing)))
         for id, item in cast(_InsertItems, self._kw["params"]).own.items():
             if id >= _MixerParamsID.RouteVolStart:
                 try:
-                    cond = next(items)["is_routed"]
+                    cond = next(items)
                 except StopIteration:
                     continue
                 else:
                     if cond:
                         yield item["msg"]
 
     separator_shown = FlagProp(_InsertFlags.SeparatorShown, InsertID.Flags)
@@ -653,15 +603,15 @@
                 return False
 
             if e.id in (*InsertID, *PluginID, *SlotID):
                 return True
 
         params: dict[int, _InsertItems] = {}
         if MixerID.Params in self.events.ids:
-            params = cast(MixerParamsEvent, self.events.first(MixerID.Params)).items
+            params = cast(MixerParamsEvent, self.events.first(MixerID.Params)).items_
 
         for i, ed in enumerate(self.events.subtrees(select, self.max_inserts)):
             if i in params:
                 yield Insert(ed, iid=i - 1, max_slots=self.max_slots, params=params[i])
             else:
                 yield Insert(ed, iid=i - 1, max_slots=self.max_slots)
```

### Comparing `pyflp-2.1.1/pyflp/pattern.py` & `pyflp-2.2.0/pyflp/pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,79 +15,78 @@
 
 from __future__ import annotations
 
 import enum
 from collections import defaultdict
 from typing import DefaultDict, Iterator, cast
 
-import colour
 import construct as c
 
-from ._descriptors import EventProp, FlagProp, StdEnum, StructProp
-from ._events import (
+from pyflp._adapters import StdEnum
+from pyflp._descriptors import EventProp, FlagProp, StructProp
+from pyflp._events import (
     DATA,
     DWORD,
     TEXT,
     WORD,
     BoolEvent,
     ColorEvent,
     EventEnum,
     EventTree,
     I32Event,
     IndexedEvent,
     ListEventBase,
     U16Event,
     U32Event,
 )
-from ._models import (
-    EventModel,
-    ItemModel,
-    ModelCollection,
-    ModelReprMixin,
-    supports_slice,
-)
-from .exceptions import ModelNotFound, NoModelsFound
-from .timemarker import TimeMarker, TimeMarkerID
+from pyflp._models import EventModel, ItemModel, ModelCollection, ModelReprMixin, supports_slice
+from pyflp.exceptions import ModelNotFound, NoModelsFound
+from pyflp.timemarker import TimeMarker, TimeMarkerID
+from pyflp.types import RGBA
 
 __all__ = ["Note", "Controller", "Pattern", "Patterns"]
 
 
 class ControllerEvent(ListEventBase):
-    STRUCT = c.Struct(
-        "position" / c.Int32ul,  # 4, can be delta as well!
-        "_u1" / c.Byte,  # 5
-        "_u2" / c.Byte,  # 6
-        "channel" / c.Int8ul,  # 7
-        "_flags" / c.Int8ul,  # 8
-        "value" / c.Float32l,  # 12
-    ).compile()
+    STRUCT = c.GreedyRange(
+        c.Struct(
+            "position" / c.Int32ul,  # 4, can be delta as well!
+            "_u1" / c.Byte,  # 5
+            "_u2" / c.Byte,  # 6
+            "channel" / c.Int8ul,  # 7
+            "_flags" / c.Int8ul,  # 8
+            "value" / c.Float32l,  # 12
+        )
+    )
 
 
 @enum.unique
 class _NoteFlags(enum.IntFlag):
     Slide = 1 << 3
 
 
 class NotesEvent(ListEventBase):
-    STRUCT = c.Struct(
-        "position" / c.Int32ul,  # 4
-        "flags" / StdEnum[_NoteFlags](c.Int16ul),  # 6
-        "rack_channel" / c.Int16ul,  # 8
-        "length" / c.Int32ul,  # 12
-        "key" / c.Int16ul,  # 14
-        "group" / c.Int16ul,  # 16
-        "fine_pitch" / c.Int8ul,  # 17
-        "_u1" / c.Byte,  # 18
-        "release" / c.Int8ul,  # 19
-        "midi_channel" / c.Int8ul,  # 20
-        "pan" / c.Int8ul,  # 21
-        "velocity" / c.Int8ul,  # 22
-        "mod_x" / c.Int8ul,  # 23
-        "mod_y" / c.Int8ul,  # 24
-    ).compile()
+    STRUCT = c.GreedyRange(
+        c.Struct(
+            "position" / c.Int32ul,  # 4
+            "flags" / StdEnum[_NoteFlags](c.Int16ul),  # 6
+            "rack_channel" / c.Int16ul,  # 8
+            "length" / c.Int32ul,  # 12
+            "key" / c.Int16ul,  # 14
+            "group" / c.Int16ul,  # 16
+            "fine_pitch" / c.Int8ul,  # 17
+            "_u1" / c.Byte,  # 18
+            "release" / c.Int8ul,  # 19
+            "midi_channel" / c.Int8ul,  # 20
+            "pan" / c.Int8ul,  # 21
+            "velocity" / c.Int8ul,  # 22
+            "mod_x" / c.Int8ul,  # 23
+            "mod_y" / c.Int8ul,  # 24
+        )
+    )
 
 
 class PatternsID(EventEnum):
     PlayTruncatedNotes = (30, BoolEvent)
     CurrentlySelected = (WORD + 3, U16Event)
 
 
@@ -143,15 +142,15 @@
 
         Only sharp key names (C#, D#, etc.) are used, flats aren't.
 
         Raises:
             ValueError: A value not in between 0-131 is tried to be set.
             ValueError: Invalid note name (not in the format {note-name}{octave}).
         """
-        return self._NOTE_NAMES[self["key"] % 12] + str(self["key"] // 12)
+        return self._NOTE_NAMES[self["key"] % 12] + str(self["key"] // 12)  # pyright: ignore
 
     @key.setter
     def key(self, value: int | str) -> None:
         if isinstance(value, int):
             if value not in range(132):
                 raise ValueError("Expected a value between 0-131.")
             self["key"] = value
@@ -247,15 +246,15 @@
             num_ctrls = 0
 
         return (
             f"Pattern(iid={self.iid}, name={self.name!r},"
             f"{num_notes} notes, {num_ctrls} controllers)"
         )
 
-    color = EventProp[colour.Color](PatternID.Color)
+    color = EventProp[RGBA](PatternID.Color)
     """Returns a colour if one is set while saving the project file, else ``None``.
 
     ![](https://bit.ly/3eNeSSW)
 
     Defaults to #485156 in FL Studio.
     """
```

### Comparing `pyflp-2.1.1/pyflp/plugin.py` & `pyflp-2.2.0/pyflp/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,42 +12,36 @@
 # <https://www.gnu.org/licenses/>.
 
 """Contains the types used by native and VST plugins to store their preset data."""
 
 from __future__ import annotations
 
 import enum
-import sys
 import warnings
-from typing import Any, ClassVar, Dict, Generic, TypeVar, cast
-
-if sys.version_info >= (3, 8):
-    from typing import Literal, Protocol, runtime_checkable
-else:
-    from typing_extensions import Literal, Protocol, runtime_checkable
+from typing import Any, ClassVar, Dict, Generic, Literal, Protocol, TypeVar, cast, runtime_checkable
 
 import construct as c
 import construct_typed as ct
 
-from ._descriptors import FlagProp, NamedPropMixin, RWProperty, StdEnum, StructProp
-from ._events import (
+from pyflp._adapters import FourByteBool, StdEnum
+from pyflp._descriptors import FlagProp, NamedPropMixin, RWProperty, StructProp
+from pyflp._events import (
     DATA,
     DWORD,
     TEXT,
     AnyEvent,
     ColorEvent,
     EventEnum,
     EventTree,
-    FourByteBool,
     StructEventBase,
-    T,
     U32Event,
     UnknownDataEvent,
 )
-from ._models import EventModel, ModelReprMixin
+from pyflp._models import EventModel, ModelReprMixin
+from pyflp.types import T
 
 __all__ = [
     "BooBass",
     "FruitKick",
     "FruityBalance",
     "FruityBloodOverdrive",
     "FruityFastDist",
@@ -103,31 +97,29 @@
 
 class FruityBalanceEvent(StructEventBase):
     STRUCT = c.Struct("pan" / c.Int32ul, "volume" / c.Int32ul).compile()
 
 
 class FruityBloodOverdriveEvent(StructEventBase):
     STRUCT = c.Struct(
-        "plugin_marker"
-        / c.If(c.this._.len == 36, c.Bytes(4)),  # redesigned native plugin marker
+        "plugin_marker" / c.If(c.this._.len == 36, c.Bytes(4)),  # redesigned native plugin marker
         "pre_band" / c.Int32ul,
         "color" / c.Int32ul,
         "pre_amp" / c.Int32ul,
         "x100" / FourByteBool,
         "post_filter" / c.Int32ul,
         "post_gain" / c.Int32ul,
         "_u1" / c.Bytes(4),
         "_u2" / c.Bytes(4),
     ).compile()
 
 
 class FruityCenterEvent(StructEventBase):
     STRUCT = c.Struct(
-        "_u1" / c.If(c.this._.len == 8, c.Bytes(4)),
-        "enabled" / FourByteBool,
+        "_u1" / c.If(c.this._.len == 8, c.Bytes(4)), "enabled" / FourByteBool
     ).compile()
 
 
 class FruityFastDistEvent(StructEventBase):
     STRUCT = c.Struct(
         "pre" / c.Int32ul,
         "threshold" / c.Int32ul,
@@ -296,15 +288,15 @@
         "type" / c.Int32ul,  # * 8 or 10 for VSTs, but I am not forcing it
         "events"
         / c.GreedyRange(
             c.Struct(
                 "id" / StdEnum[_VSTPluginEventID](c.Int32ul),
                 # ! Using a c.Select or c.IfThenElse doesn't work here
                 # Check https://github.com/construct/construct/issues/993
-                "data"
+                "data"  # pyright: ignore
                 / c.Prefixed(
                     c.Int64ul,
                     c.Switch(
                         c.this["id"],
                         {
                             _VSTPluginEventID.MIDI: _MIDIStruct,
                             _VSTPluginEventID.Flags: _FlagsStruct,
@@ -837,17 +829,15 @@
     |---------|-------|----------------|
     | Min     | 0     | -INFdB / 0.00  |
     | Max     | 320   | 5.6dB / 1.90   |
     | Default | 256   | 0.0dB / 1.00   |
     """
 
 
-class FruityBloodOverdrive(
-    _PluginBase[FruityBloodOverdriveEvent], _IPlugin, ModelReprMixin
-):
+class FruityBloodOverdrive(_PluginBase[FruityBloodOverdriveEvent], _IPlugin, ModelReprMixin):
     """![](https://bit.ly/3LnS1LE)"""
 
     INTERNAL_NAME = "Fruity Blood Overdrive"
 
     pre_band = _NativePluginProp[int]()
     """Linear.
 
@@ -1038,17 +1028,15 @@
     |---------|-------|----------------|
     | Min     | 1     | -INFdB / 0.00  |
     | Max     | 127   | 0.0dB / 1.00   |
     | Default | 100   | -4.4dB / 0.60  |
     """
 
 
-class FruityStereoEnhancer(
-    _PluginBase[FruityStereoEnhancerEvent], _IPlugin, ModelReprMixin
-):
+class FruityStereoEnhancer(_PluginBase[FruityStereoEnhancerEvent], _IPlugin, ModelReprMixin):
     """![](https://bit.ly/3DoHvji)"""
 
     INTERNAL_NAME = "Fruity Stereo Enhancer"
     effect_position = _NativePluginProp[Literal["pre", "post"]]()
     """Defaults to ``post``."""
 
     pan = _NativePluginProp[int]()
```

### Comparing `pyflp-2.1.1/pyflp/project.py` & `pyflp-2.2.0/pyflp/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,32 +15,22 @@
 
 from __future__ import annotations
 
 import datetime
 import enum
 import math
 import pathlib
-import sys
-from typing import cast
-
-if sys.version_info >= (3, 8):
-    from typing import Final, Literal, TypedDict
-else:
-    from typing_extensions import Final, Literal, TypedDict
-
-if sys.version_info >= (3, 11):
-    from typing import Unpack
-else:
-    from typing_extensions import Unpack
+from typing import Final, Literal, cast
 
 import construct as c
 import construct_typed as ct
+from typing_extensions import TypedDict, Unpack
 
-from ._descriptors import EventProp, KWProp
-from ._events import (
+from pyflp._descriptors import EventProp, KWProp
+from pyflp._events import (
     DATA,
     DWORD,
     TEXT,
     WORD,
     AnyEvent,
     AsciiEvent,
     BoolEvent,
@@ -48,22 +38,23 @@
     EventTree,
     I16Event,
     I32Event,
     StructEventBase,
     U8Event,
     U32Event,
 )
-from ._models import EventModel, FLVersion
-from .arrangement import ArrangementID, Arrangements, ArrangementsID, TrackID
-from .channel import ChannelID, ChannelRack, DisplayGroupID, RackID
-from .exceptions import PropertyCannotBeSet
-from .mixer import InsertID, Mixer, MixerID, SlotID
-from .pattern import PatternID, Patterns, PatternsID
-from .plugin import PluginID
-from .timemarker import TimeMarkerID
+from pyflp._models import EventModel
+from pyflp.arrangement import ArrangementID, Arrangements, ArrangementsID, TrackID
+from pyflp.channel import ChannelID, ChannelRack, DisplayGroupID, RackID
+from pyflp.exceptions import PropertyCannotBeSet
+from pyflp.mixer import InsertID, Mixer, MixerID, SlotID
+from pyflp.pattern import PatternID, Patterns, PatternsID
+from pyflp.plugin import PluginID
+from pyflp.timemarker import TimeMarkerID
+from pyflp.types import FLVersion
 
 __all__ = ["PanLaw", "Project", "FileFormat", "VALID_PPQS"]
 
 _DELPHI_EPOCH: Final = datetime.datetime(1899, 12, 30)
 MIN_TEMPO: Final = 10.000
 """Minimum tempo (in BPM) FL Studio supports."""
 
@@ -153,17 +144,15 @@
 class Project(EventModel):
     """Represents an FL Studio project."""
 
     def __init__(self, events: EventTree, **kw: Unpack[_ProjectKW]) -> None:
         super().__init__(events, **kw)
 
     def __repr__(self) -> str:
-        return "Project(format={}, version={}, {} channels)".format(
-            self.format, self.version, self.channel_count
-        )
+        return f"<Project(format={self.format!r}, version={self.version!r}>"
 
     def __str__(self) -> str:
         return f"FL Studio v{self.version!s} {self.format.name}"  # type: ignore
 
     @property
     def arrangements(self) -> Arrangements:
         """Provides an iterator over arrangements and other related properties."""
@@ -467,21 +456,17 @@
         if ProjectID._TempoFine in self.events.ids:
             tempo += self.events.first(ProjectID._TempoFine).value / 1000
         return tempo
 
     @tempo.setter
     def tempo(self, value: int | float) -> None:
         if self.tempo is None:
-            raise PropertyCannotBeSet(
-                ProjectID.Tempo, ProjectID._TempoCoarse, ProjectID._TempoFine
-            )
+            raise PropertyCannotBeSet(ProjectID.Tempo, ProjectID._TempoCoarse, ProjectID._TempoFine)
 
-        max_tempo = (
-            999.0 if FLVersion(1, 4, 2) <= self.version < FLVersion(11) else 522.0
-        )
+        max_tempo = 999.0 if FLVersion(1, 4, 2) <= self.version < FLVersion(11) else 522.0
 
         if isinstance(value, float) and self.version < FLVersion(3, 4, 0):
             raise TypeError("Expected an 'int' object got a 'float' instead")
 
         if float(value) > max_tempo or float(value) < MIN_TEMPO:
             raise ValueError(f"Invalid tempo {value}; expected {MIN_TEMPO}-{max_tempo}")
```

### Comparing `pyflp-2.1.1/pyflp/timemarker.py` & `pyflp-2.2.0/pyflp/timemarker.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 """Contains the types required for pattern and playlist timemarkers."""
 
 from __future__ import annotations
 
 import enum
 
-from ._descriptors import EventProp
-from ._events import DWORD, TEXT, EventEnum, U8Event, U32Event
-from ._models import EventModel, ModelReprMixin
+from pyflp._descriptors import EventProp
+from pyflp._events import DWORD, TEXT, EventEnum, U8Event, U32Event
+from pyflp._models import EventModel, ModelReprMixin
 
 __all__ = ["TimeMarkerID", "TimeMarkerType", "TimeMarker"]
 
 
 @enum.unique
 class TimeMarkerID(EventEnum):
     Numerator = (33, U8Event)
```

### Comparing `pyflp-2.1.1/pyflp.egg-info/PKG-INFO` & `pyflp-2.2.0/pyflp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: pyflp
-Version: 2.1.1
+Version: 2.2.0
 Summary: FL Studio project file parser
 Author-email: demberto <demberto@protonmail.com>
 License: GPL-3.0
 Project-URL: Source, https://github.com/demberto/PyFLP
 Project-URL: Changelog, https://github.com/demberto/PyFLP/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://pyflp.rtfd.io
 Project-URL: Bug Tracker, https://github.com/demberto/PyFLP/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # PyFLP
 
 PyFLP is an unofficial parser for [FL Studio](https://www.image-line.com/fl-studio/)
@@ -40,15 +39,14 @@
     <col style="width: 10%;"/>
     <col style="width: 90%;"/>
   </colgroup>
   <tbody>
     <tr>
       <th>CI</th>
       <td>
-        <img alt="build" src="https://github.com/demberto/PyFLP/actions/workflows/publish.yml/badge.svg"/>
         <a href="https://pyflp.readthedocs.io/en/latest/">
           <img alt="Documentation Build Status" src="https://img.shields.io/readthedocs/pyflp/latest?logo=read-the-docs"/>
         </a>
         <a href="https://results.pre-commit.ci/latest/github/demberto/PyFLP/master">
           <img alt="pre-commit-ci" src="https://results.pre-commit.ci/badge/github/demberto/PyFLP/master.svg"/>
         </a>
       </td>
@@ -337,15 +335,15 @@
     </td>
   </tr>
 </table>
 <!-- markdownlint-restore -->
 
 ## ⏬ Installation
 
-CPython 3.7+ / PyPy 3.8+ required.
+CPython 3.8+ / PyPy 3.8+ required.
 
 ```none
 python -m pip install -U pyflp
 ```
 
 ## ▶ Usage
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1 Name: pyflp Version: 2.1.1 Summary: FL Studio project
+Metadata-Version: 2.1 Name: pyflp Version: 2.2.0 Summary: FL Studio project
 file parser Author-email: demberto
 protonmail.com> License: GPL-3.0 Project-URL: Source, https://github.com/
 demberto/PyFLP Project-URL: Changelog, https://github.com/demberto/PyFLP/blob/
 master/CHANGELOG.md Project-URL: Documentation, https://pyflp.rtfd.io Project-
 URL: Bug Tracker, https://github.com/demberto/PyFLP/issues Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Multimedia
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev License-File: LICENSE # PyFLP PyFLP is an
-unofficial parser for [FL Studio](https://www.image-line.com/fl-studio/
-) project and preset files written in Python.
-CI       [build] [Documentation_Build_Status] [pre-commit-ci]
+:: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Multimedia Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python: >=3.8
+Description-Content-Type: text/markdown Provides-Extra: dev License-File:
+LICENSE # PyFLP PyFLP is an unofficial parser for [FL Studio](https://
+www.image-line.com/fl-studio/) project and preset files written in Python.
+CI       [Documentation_Build_Status] [pre-commit-ci]
 PyPI     [PyPI_-_Package_Version] [PyPI_-_Supported_Python_Versions] [PyPI_-
          Supported_Implementations] [PyPI_-_Wheel]
 Activity [Maintenance] [PyPI_-_Downloads]
 QA       [codecov] [CodeFactor_Grade] [Checked_with_mypy] [pre-commit]
          [Security_Status]
 Other    [License] [GitHub top language] [Code_Style:_Black] [covenant]
  From a very general point-of-view, this is the state of what is currently
@@ -65,15 +64,15 @@
 Plugins                                         issues]
                                                 [plugin-3rdparty_issues]
                           VST_2/3               [closed_plugin-3rdparty
                                                 issues]
                                                 [open_project-general
 Project - Settings and song metadata            issues] [closed_project-
                                                 general_issues]
- ## â¬ Installation CPython 3.7+ / PyPy 3.8+ required. ```none python -m pip
+ ## â¬ Installation CPython 3.8+ / PyPy 3.8+ required. ```none python -m pip
 install -U pyflp ``` ## â¶ Usage [Load](https://pyflp.readthedocs.io/en/
 latest/reference.html#pyflp.parse) a project file: ```py import pyflp project =
 pyflp.parse("/path/to/parse.flp") ``` > If you get any sort of errors or
 warnings while doing this, please open an > [issue](https://github.com/
 demberto/PyFLP/issues). [Save](https://pyflp.readthedocs.io/en/latest/
 reference.html#pyflp.save) the project: ```py pyflp.save(project, "/path/to/
 save.flp") ``` > It is advised to do a backup of your projects before doing any
```

### Comparing `pyflp-2.1.1/pyflp.egg-info/SOURCES.txt` & `pyflp-2.2.0/pyflp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -154,28 +154,30 @@
 docs/reference/patterns/index.rst
 docs/reference/patterns/pattern.rst
 docs/reference/plugins/effects.rst
 docs/reference/plugins/generators.rst
 docs/reference/plugins/index.rst
 docs/reference/plugins/vst.rst
 pyflp/__init__.py
+pyflp/_adapters.py
 pyflp/_descriptors.py
 pyflp/_events.py
 pyflp/_models.py
 pyflp/_version.py
 pyflp/arrangement.py
 pyflp/channel.py
 pyflp/controller.py
 pyflp/exceptions.py
 pyflp/mixer.py
 pyflp/pattern.py
 pyflp/plugin.py
 pyflp/project.py
 pyflp/py.typed
 pyflp/timemarker.py
+pyflp/types.py
 pyflp.egg-info/PKG-INFO
 pyflp.egg-info/SOURCES.txt
 pyflp.egg-info/dependency_links.txt
 pyflp.egg-info/requires.txt
 pyflp.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
```

### Comparing `pyflp-2.1.1/pyproject.toml` & `pyflp-2.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,52 +3,58 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyflp"
 authors = [{ name = "demberto", email = "demberto@protonmail.com" }]
 description = "FL Studio project file parser"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Multimedia",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed",
 ]
 license = { text = "GPL-3.0" }
 dependencies = [
-  "colour>=0.1.5",
   "f-enum>=0.2.0;python_version<='3.10'",
   "construct-typing>=0.5.6",
   "sortedcontainers>=2.4.0",
   "typing_extensions>=4.6.1",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["coverage >=7.2.6", "pre-commit >= 3.3.2", "pytest >=7.3.1", "tox >=4.5.1"]
+dev = [
+  "coverage >=7.2.6",
+  "pre-commit >= 3.3.2",
+  "pytest >=7.3.1",
+  "tox >=4.5.1",
+]
 # for docs dependencies see docs/requirements.txt
 
 [project.urls]
 Source = "https://github.com/demberto/PyFLP"
 Changelog = "https://github.com/demberto/PyFLP/blob/master/CHANGELOG.md"
 Documentation = "https://pyflp.rtfd.io"
 "Bug Tracker" = "https://github.com/demberto/PyFLP/issues"
 
+[tool.black]
+line-length = 100
+
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = ["main.py"]
 
 [tool.coverage.report]
 exclude_lines = [
@@ -58,17 +64,18 @@
   "if owner is None:",        # Descriptor __get__() checks
   "@(abc\\.)?abstractmethod", # "@abc.abstractmethod" or "@abstractmethod"
 ]
 ignore_errors = true
 
 [tool.isort]
 profile = "black"
+line-length = 100
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 check_untyped_defs = true
 enable_incomplete_feature = ["Unpack"]
 ignore_missing_imports = true
 warn_no_return = false
 
 [tool.pyright]
 ignore = ["./venv"]
@@ -79,14 +86,15 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = "tests"
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
+line-length = 100
 
 [tool.setuptools]
 packages = ["pyflp"]
 
 [tool.setuptools_scm]
 write_to = "pyflp/_version.py"
```

### Comparing `pyflp-2.1.1/tests/assets/FL 20.8.4.flp` & `pyflp-2.2.0/tests/assets/FL 20.8.4.flp`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/+4800-cents.fst` & `pyflp-2.2.0/tests/assets/channels/+4800-cents.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/-4800-cents.fst` & `pyflp-2.2.0/tests/assets/channels/-4800-cents.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/100%-left.fst` & `pyflp-2.2.0/tests/assets/channels/100%-left.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/100%-right.fst` & `pyflp-2.2.0/tests/assets/channels/100%-right.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/arp.fst` & `pyflp-2.2.0/tests/assets/channels/arp.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/automation-lfo.fst` & `pyflp-2.2.0/tests/assets/channels/automation-lfo.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/automation-points.fst` & `pyflp-2.2.0/tests/assets/channels/automation-points.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/colored.fst` & `pyflp-2.2.0/tests/assets/channels/colored.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/cut-groups.fst` & `pyflp-2.2.0/tests/assets/channels/cut-groups.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/delay.fst` & `pyflp-2.2.0/tests/assets/channels/delay.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/disabled.fst` & `pyflp-2.2.0/tests/assets/channels/disabled.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/envelope.fst` & `pyflp-2.2.0/tests/assets/channels/envelope.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/full-volume.fst` & `pyflp-2.2.0/tests/assets/channels/full-volume.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/iconified.fst` & `pyflp-2.2.0/tests/assets/channels/iconified.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/keyboard.fst` & `pyflp-2.2.0/tests/assets/channels/keyboard.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/layer-crossfade.fst` & `pyflp-2.2.0/tests/assets/channels/layer-crossfade.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/layer-random.fst` & `pyflp-2.2.0/tests/assets/channels/layer-random.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/level-adjusts.fst` & `pyflp-2.2.0/tests/assets/channels/level-adjusts.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/lfo.fst` & `pyflp-2.2.0/tests/assets/channels/lfo.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/locked.fst` & `pyflp-2.2.0/tests/assets/channels/locked.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/polyphony.fst` & `pyflp-2.2.0/tests/assets/channels/polyphony.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/routed.fst` & `pyflp-2.2.0/tests/assets/channels/routed.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/sampler-content.fst` & `pyflp-2.2.0/tests/assets/channels/sampler-content.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/sampler-filter.fst` & `pyflp-2.2.0/tests/assets/channels/sampler-filter.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/sampler-fx.fst` & `pyflp-2.2.0/tests/assets/channels/sampler-fx.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/sampler-path.fst` & `pyflp-2.2.0/tests/assets/channels/sampler-path.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/sampler-playback.fst` & `pyflp-2.2.0/tests/assets/channels/sampler-playback.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/sampler-stretching.fst` & `pyflp-2.2.0/tests/assets/channels/sampler-stretching.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/time.fst` & `pyflp-2.2.0/tests/assets/channels/time.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/tracking.fst` & `pyflp-2.2.0/tests/assets/channels/tracking.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/channels/zero-volume.fst` & `pyflp-2.2.0/tests/assets/channels/zero-volume.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/inserts/50ms-input-latency.fst` & `pyflp-2.2.0/tests/assets/inserts/50ms-input-latency.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/inserts/50ms-track-latency.fst` & `pyflp-2.2.0/tests/assets/inserts/50ms-track-latency.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/inserts/effects-bypassed.fst` & `pyflp-2.2.0/tests/assets/inserts/effects-bypassed.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/patterns/multi-channel.flp` & `pyflp-2.2.0/tests/assets/patterns/multi-channel.flp`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/plugins/fruit-kick.fst` & `pyflp-2.2.0/tests/assets/plugins/fruit-kick.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/plugins/fruity-wrapper.fst` & `pyflp-2.2.0/tests/assets/plugins/fruity-wrapper.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/plugins/plucked.fst` & `pyflp-2.2.0/tests/assets/plugins/plucked.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/assets/plugins/xfer-djmfilter.fst` & `pyflp-2.2.0/tests/assets/plugins/xfer-djmfilter.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/conftest.py` & `pyflp-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/test_arrangement.py` & `pyflp-2.2.0/tests/test_arrangement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Callable
 
-import colour
 import pytest
 
+from pyflp._events import RGBA
 from pyflp.arrangement import (
     Arrangement,
     Arrangements,
     ChannelPLItem,
     PatternPLItem,
     Track,
     TrackMotion,
@@ -38,26 +38,24 @@
 def tracks(arrangement: Callable[[int], Arrangement]):
     return tuple(arrangement(0).tracks)[:22]
 
 
 def test_track_color(tracks: tuple[Track, ...]):
     for track in tracks:
         assert (
-            track.color == colour.Color("red")
+            track.color == RGBA(1.0, 0.0, 0.0, 0.0)
             if track.name == "Red"
-            else track.color == colour.Color("#485156")
+            else track.color == RGBA.from_bytes(bytes((72, 81, 86, 0)))
         )
 
 
 def test_track_content_locked(tracks: tuple[Track, ...]):
     for track in tracks:
         assert (
-            track.content_locked
-            if track.name == "Locked to content"
-            else not track.content_locked
+            track.content_locked if track.name == "Locked to content" else not track.content_locked
         )
 
 
 def test_track_enabled(tracks: tuple[Track, ...]):
     for track in tracks:
         assert not track.enabled if track.name == "Disabled" else track.enabled
 
@@ -83,20 +81,20 @@
 
 
 def test_track_items(tracks: tuple[Track, ...]):
     for track in tracks:
         num_items = 0
         if track.name == "Audio track":
             num_items = 16
-            assert set(type(i) for i in track) == set((ChannelPLItem,))
-            assert set(i.channel.iid for i in track) == set((11,))  # type: ignore
+            assert {type(i) for i in track} == {ChannelPLItem}
+            assert {i.channel.iid for i in track} == {11}  # type: ignore
         elif track.name == "MIDI":
             num_items = 4
-            assert set(type(i) for i in track) == set((PatternPLItem,))
-            assert set(i.pattern.iid for i in track) == set((3,))  # type: ignore
+            assert {type(i) for i in track} == {PatternPLItem}
+            assert {i.pattern.iid for i in track} == {3}  # type: ignore
             assert [i.position for i in track] == [p * 384 for p in range(num_items)]
         elif track.name in ("Cut pattern", "Automation"):
             num_items = 1
 
         assert len(track) == num_items
         assert [i.group for i in track] == [0] * num_items
```

### Comparing `pyflp-2.1.1/tests/test_channel.py` & `pyflp-2.2.0/tests/test_channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import pathlib
 from typing import TypeVar
 
-import colour
-
+from pyflp._events import RGBA
 from pyflp.channel import (
     Automation,
     Channel,
     ChannelRack,
     DeclickMode,
     FilterType,
     Instrument,
@@ -66,15 +65,15 @@
 
 def test_automation_points():
     points = [point for point in load_automation("automation-points.fst")]
     assert [int(p.position or 0) for p in points] == [0, 8, 8, 16, 24, 32]
 
 
 def test_channel_color():
-    assert load_channel("colored.fst").color == colour.Color("#1414FF")
+    assert load_channel("colored.fst").color == RGBA.from_bytes(bytes((20, 20, 255, 0)))
 
 
 def test_channel_enabled():
     assert not load_channel("disabled.fst").enabled
 
 
 def test_channel_group(rack: ChannelRack):
```

### Comparing `pyflp-2.1.1/tests/test_corrupted.py` & `pyflp-2.2.0/tests/test_corrupted.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.1.1/tests/test_mixer.py` & `pyflp-2.2.0/tests/test_mixer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from typing import cast
 
-import colour
-
+from pyflp._events import RGBA
 from pyflp.mixer import Insert, InsertDock, Mixer, MixerID, MixerParamsEvent
 
 from .conftest import get_model
 
 
 def get_insert(preset: str):
     # Parse as Mixer to get events, because an Insert cannot parse
@@ -15,28 +14,28 @@
     mixer = get_model(f"inserts/{preset}", Mixer)
 
     # A preset stores items only for a single insert, currently thats 32 per
     # insert. Pass these to Insert's constructor. This mimics Mixer's normal
     # behaviour, however that depends on InsertID.Output as a marker to indicate
     # the end of an Insert, which surprisingly isn't a part of presets.
     params = cast(MixerParamsEvent, mixer.events.first(MixerID.Params))
-    items = tuple(params.items.values())[0]
+    items = tuple(params.items_.values())[0]
     return Insert(mixer.events, iid=0, max_slots=10, params=items)
 
 
 def test_insert_bypassed():
     assert get_insert("effects-bypassed.fst").bypassed
 
 
 def test_insert_channels_swapped():
     assert get_insert("channels-swapped.fst").channels_swapped
 
 
 def test_insert_color():
-    assert get_insert("colored.fst").color == colour.Color("#FF1414")
+    assert get_insert("colored.fst").color == RGBA.from_bytes(bytes((255, 20, 20, 0)))
 
 
 def test_insert_dock(inserts: tuple[Insert, ...]):
     sends = (101, 102, 103, 104)
     for insert in inserts:
         if insert.name in ("Docked left", "Master"):
             assert insert.dock == InsertDock.Left
```

### Comparing `pyflp-2.1.1/tests/test_pattern.py` & `pyflp-2.2.0/tests/test_pattern.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
-import colour
-
+from pyflp._events import RGBA
 from pyflp.pattern import Pattern, PatternID, Patterns
 
 from .conftest import get_model
 
 
 def get_notes(score: str):
     return tuple(get_model(f"patterns/{score}", Pattern, *PatternID).notes)
@@ -14,21 +13,25 @@
 def test_patterns(patterns: Patterns):
     assert len(patterns) == 5
     assert patterns.current == patterns[4]
     assert patterns.play_cut_notes
 
 
 def test_pattern_color(patterns: Patterns):
-    assert patterns[2].color == colour.Color("#00FF00")
+    assert patterns[2].color == RGBA(0.0, 1.0, 0.0, 0.0)
 
 
 def test_pattern_names(patterns: Patterns):
-    assert set(pattern.name for pattern in patterns) == set(
-        ("Default", "Colored", "MIDI", "Timemarkers", "Selected")
-    )
+    assert {pattern.name for pattern in patterns} == {
+        "Default",
+        "Colored",
+        "MIDI",
+        "Timemarkers",
+        "Selected",
+    }
 
 
 def test_pattern_timemarkers(patterns: Patterns):
     assert len(tuple(patterns["Timemarkers"].timemarkers)) == 5
 
 
 def test_empty_pattern():
@@ -70,15 +73,15 @@
 
 def test_note_position():
     notes = get_notes("c-major-scale.fsc")
     assert [n.position for n in notes] == [x * 384 for x in range(8)]
 
 
 def test_note_rack_channel():
-    assert set(n.rack_channel for n in get_notes("multi-channel.flp")) == set((0, 1))
+    assert {n.rack_channel for n in get_notes("multi-channel.flp")} == {0, 1}
 
 
 def test_note_release():
     assert [n.release for n in get_notes("release-min-max.fsc")] == [0, 128]
 
 
 def test_note_slide():
```

### Comparing `pyflp-2.1.1/tests/test_plugin.py` & `pyflp-2.2.0/tests/test_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,17 +47,15 @@
 def test_fruity_balance():
     fruity_balance = get_plugin("fruity-balance.fst", FruityBalance)
     assert fruity_balance.volume == 256
     assert fruity_balance.pan == 0
 
 
 def test_fruity_blood_overdrive():
-    fruity_blood_overdrive = get_plugin(
-        "fruity-blood-overdrive.fst", FruityBloodOverdrive
-    )
+    fruity_blood_overdrive = get_plugin("fruity-blood-overdrive.fst", FruityBloodOverdrive)
     assert fruity_blood_overdrive.pre_band == 0
     assert fruity_blood_overdrive.color == 5000
     assert fruity_blood_overdrive.pre_amp == 0
     assert fruity_blood_overdrive.x100 == 0
     assert fruity_blood_overdrive.post_filter == 0
 
 
@@ -86,17 +84,15 @@
 def test_fruity_soft_clipper():
     fruity_soft_clipper = get_plugin("fruity-soft-clipper.fst", FruitySoftClipper)
     assert fruity_soft_clipper.threshold == 100
     assert fruity_soft_clipper.post == 128
 
 
 def test_fruity_stereo_enhancer():
-    fruity_stereo_enhancer = get_plugin(
-        "fruity-stereo-enhancer.fst", FruityStereoEnhancer
-    )
+    fruity_stereo_enhancer = get_plugin("fruity-stereo-enhancer.fst", FruityStereoEnhancer)
     assert fruity_stereo_enhancer.stereo_separation == 0
     assert fruity_stereo_enhancer.effect_position == "post"
     assert fruity_stereo_enhancer.phase_offset == 0
     assert fruity_stereo_enhancer.phase_inversion == "none"
     assert fruity_stereo_enhancer.pan == 0
     assert fruity_stereo_enhancer.volume == 256
```

### Comparing `pyflp-2.1.1/tests/test_project.py` & `pyflp-2.2.0/tests/test_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,9 +59,9 @@
         project.version = "2.2"  # type: ignore
 
 
 def test_null_check(project: Project, tmp_path: pathlib.Path):
     pyflp.save(project, tmp_path / "null_check.flp")
     b1 = open(pathlib.Path(__file__).parent / "assets" / "FL 20.8.4.flp", "rb").read()
     b2 = open(tmp_path / "null_check.flp", "rb").read()
-    result = b1 == b2  # ! Don't compare 2 big bytes objects in pytest EVER
-    assert result
+    # result = b1 == b2  # ! Don't compare 2 big bytes objects in pytest EVER
+    assert b1 == b2
```

### Comparing `pyflp-2.1.1/tox.ini` & `pyflp-2.2.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = precommit,py{37,38,39,310,311},pypy{38,39},docs
+envlist = precommit,py{38,39,310,311},pypy{38,39},docs
 minversion = 4.0
 parallel = auto
 
 [testenv]
 deps =
   -rrequirements.txt
   coverage
@@ -26,14 +26,13 @@
   -rdocs/requirements.txt
   -rrequirements.txt
 commands =
   sphinx-build -b linkcheck docs docs/_build/linkcheck
 
 [gh]
 python =
-  3.7: py37, mypy
   3.8: py38
   3.9: py39
   3.10: py310, docs
   3.11: py311, precommit
   pypy-3.8: pypy38
   pypy-3.9: pypy39
```

