# Comparing `tmp/apysc-2.7.9.tar.gz` & `tmp/apysc-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apysc-2.7.9.tar", last modified: Sat Apr  1 12:12:41 2023, max compression
+gzip compressed data, was "apysc-2.8.0.tar", last modified: Sun May 28 09:12:13 2023, max compression
```

## Comparing `apysc-2.7.9.tar` & `apysc-2.8.0.tar`

### file list

```diff
@@ -1,588 +1,669 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.578360 apysc-2.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-01 12:12:18.000000 apysc-2.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-01 12:12:18.000000 apysc-2.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-01 12:12:41.578360 apysc-2.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-01 12:12:18.000000 apysc-2.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.526360 apysc-2.7.9/apysc/
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.534360 apysc-2.7.9/apysc/_animation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_cx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_cy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_finish_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_height.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_height_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_height_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_parallel_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_pause_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_play_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_reset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_reverse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_scale_x_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_scale_x_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_scale_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_scale_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_time_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_width.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_width_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_width_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/animation_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_animation/easing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.534360 apysc-2.7.9/apysc/_branch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_branch/_elif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_branch/_else.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_branch/_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_branch/if_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.534360 apysc-2.7.9/apysc/_callable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_callable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_callable/callable_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.534360 apysc-2.7.9/apysc/_color/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_color/color_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.534360 apysc-2.7.9/apysc/_console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_console/_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    31060 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_console/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_console/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.534360 apysc-2.7.9/apysc/_converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_converter/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_converter/to_apysc_val_from_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_converter/to_builtin_val_from_apysc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.542360 apysc-2.7.9/apysc/_display/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/any_display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_fill_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_fill_color_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_line_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_line_cap_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_line_color_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_line_joints_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_line_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_line_thickness_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_x_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/append_y_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/begin_fill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/ellipse_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/ellipse_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/flip_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/flip_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/flip_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    47129 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/graphics_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/graphics_clear_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/graphics_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_cap_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_caps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_dash_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_dash_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_joints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_joints_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_round_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    27089 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_style_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/points_2d_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/points_var_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14323 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polygon_append_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polygon_apply_current_points_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polygon_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polygon_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polygon_x3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polygon_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polygon_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polygon_y3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/rotation_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/scale_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/set_lower_scale_limit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/skew_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/skew_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_set_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_set_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_set_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_set_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_set_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_set_font_size_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_set_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_set_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_set_text_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_singleton_for_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15985 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/svg_text_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/visible_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/width_and_height_mixin_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/x_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/y_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_display/y_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.546360 apysc-2.7.9/apysc/_event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/custom_event_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/custom_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/document_mouse_wheel_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/double_click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/enter_frame_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/enter_frame_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/handler_circular_calling_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_down_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_event_binding_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_event_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_event_unbinding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_out_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_over_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/mouse_up_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/prevent_default_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/set_handler_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/stop_propagation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_event/wheel_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.546360 apysc-2.7.9/apysc/_expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_expression/event_handler_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_expression/expression_data_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_expression/expression_variables_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_expression/indent_num.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_expression/js_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_expression/last_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_expression/var_names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.546360 apysc-2.7.9/apysc/_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_file/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_file/module_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.550360 apysc-2.7.9/apysc/_geom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_control_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_control_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_control_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_control_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_control_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_control_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_data_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_data_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_dest_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_dest_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/path_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_geom/relative_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.550360 apysc-2.7.9/apysc/_html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_html/debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_html/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_html/html_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_html/html_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.550360 apysc-2.7.9/apysc/_jslib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_jslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_jslib/jquery-3.6.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_jslib/jslib_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    78572 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_jslib/svg-3.1.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_jslib/underscore-1.12.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.550360 apysc-2.7.9/apysc/_jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_jupyter/jupyter_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.550360 apysc-2.7.9/apysc/_lint_and_doc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/conf_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/docs_keyword_link_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/docs_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/docs_toctree_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/docs_translation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/docstring_to_markdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51969 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/docstring_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/document_text_split_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/document_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.550360 apysc-2.7.9/apysc/_lint_and_doc/fixed_translation_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   202620 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/lint_and_doc_hash_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_lint_and_doc/translation_mapping_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.554360 apysc-2.7.9/apysc/_loop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_loop/_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_loop/_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_loop/loop_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.554360 apysc-2.7.9/apysc/_math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_math/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_math/max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_math/min_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_math/trunc_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.554360 apysc-2.7.9/apysc/_string/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_string/indent_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_string/string_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.554360 apysc-2.7.9/apysc/_testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_testing/e2e_testing_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_testing/testing_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.554360 apysc-2.7.9/apysc/_time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/datetime_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/day_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/days_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/fps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/hour_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/left_and_right_datetimes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/millisecond_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/minute_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/month_end_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/month_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/now_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/second_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/timedelta_.py
--rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/total_seconds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/weekday_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_time/year_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.554360 apysc-2.7.9/apysc/_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.574360 apysc-2.7.9/apysc/_translation/jp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/about_handler_options_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/add_child_and_remove_child.py
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/add_debug_info_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_base_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_base_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_finish.py
--rw-r--r--   0 runner    (1001) docker     (123)   143972 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_method_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_pause_and_play.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_return_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    22568 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_width_and_height.py
--rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/append_js_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_append_and_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_extend_and_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_index_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_insert_and_insert_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_remove_and_remove_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/array_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/assert_defined_and_undefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/assert_equal_and_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/assert_greater_and_greater_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/assert_less_and_less_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/assert_true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/assertion_basic_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    25457 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/bind_and_trigger_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    47227 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/contains.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/continue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_day.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_hour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_millisecond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_minute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_month.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_second.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_set_month_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/datetime_year.py
--rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/dblclick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/dictionary_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/dictionary_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/dictionary_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/display_object_get_and_set_css.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/display_object_mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/display_object_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/display_object_visible.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/display_object_x_and_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/display_on_colaboratory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/display_on_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/draw_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    84469 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/easing_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/elif.py
--rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/else.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/enter_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/for.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/fps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/fundamental_data_classes_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/get_child_at.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_flip_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_scale_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_scale_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_base_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_begin_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_dashed_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_round_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_round_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_draw_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    62521 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_line_style.py
--rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/graphics_move_to_and_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/if.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/import_conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/int_and_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/int_and_number_arithmetic_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/int_and_number_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/math_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/math_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/math_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/mouse_event_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/mouse_event_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    27457 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/mousedown_and_mouseup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/mousemove.py
--rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/mouseover_and_mouseout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/num_children.py
--rw-r--r--   0 runner    (1001) docker     (123)    60597 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    49410 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    51647 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/quick_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/recommended_type_checker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/remove_children.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/return.py
--rw-r--r--   0 runner    (1001) docker     (123)    17192 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/save_overall_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/sequential_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/set_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)    30948 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/string_addition_and_multiplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/string_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/string_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    48345 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    44916 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timedelta_days.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timedelta_total_seconds.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timer_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timer_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timer_repeat_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timer_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/timer_start_and_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    64293 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/unset_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/variable_name_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/what_apysc_can_do.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.578360 apysc-2.7.9/apysc/_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/_return.py
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    45376 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/attr_linking_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/blank_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/deleted_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/dictionary_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/expression_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/initial_substitution_exp_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/number.py
--rw-r--r--   0 runner    (1001) docker     (123)    33927 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/number_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/py_builtin_iter_disabling_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/revert_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/revert_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    25560 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/string_split_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/type_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/type_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/value_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/variable_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/variable_name_suffix_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_type/variable_name_suffix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.578360 apysc-2.7.9/apysc/_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92425 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/arg_validation_decos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/bool_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/color_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/display_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/event_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/geom_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/number_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/parent_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/path_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/string_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-01 12:12:18.000000 apysc-2.7.9/apysc/_validation/variable_name_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 12:12:41.526360 apysc-2.7.9/apysc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-01 12:12:41.000000 apysc-2.7.9/apysc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-04-01 12:12:41.000000 apysc-2.7.9/apysc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 12:12:41.000000 apysc-2.7.9/apysc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-01 12:12:41.000000 apysc-2.7.9/apysc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-01 12:12:41.000000 apysc-2.7.9/apysc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 12:12:41.578360 apysc-2.7.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:13.008486 apysc-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-28 09:11:47.000000 apysc-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 09:11:47.000000 apysc-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-28 09:12:13.008486 apysc-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-28 09:11:47.000000 apysc-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.912486 apysc-2.8.0/apysc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.924486 apysc-2.8.0/apysc/_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_cx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_cy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_finish_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_height_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_height_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_parallel_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_pause_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_play_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_reset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_reverse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_scale_x_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_scale_x_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_scale_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_scale_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_time_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_width_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_width_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/animation_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_animation/easing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.924486 apysc-2.8.0/apysc/_auto_reloading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_auto_reloading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_auto_reloading/auto_reloading_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.924486 apysc-2.8.0/apysc/_branch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_branch/_elif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_branch/_else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_branch/_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_branch/if_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.924486 apysc-2.8.0/apysc/_callable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_callable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_callable/callable_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.932486 apysc-2.8.0/apysc/_chart/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/add_background_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/add_border_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/axis_label_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/axis_label_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/axis_label_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/axis_label_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/axis_label_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/axis_label_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/axis_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/axis_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/axis_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/background_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/border_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/chart_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/chart_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18520 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/create_single_column_y_axis_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/initialize_each_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/is_display_axis_label_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/overall_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_background_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_background_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_border_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_border_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_border_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_horizontal_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_matrix_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_vertical_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/set_initial_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/tick_max_num_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/tick_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/tick_text_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/tick_text_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/tick_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/tick_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/tick_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/vertical_bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/x_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/x_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/x_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/x_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/x_axis_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/y_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/y_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/y_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/y_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/y_axis_single_column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/y_max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_chart/y_min_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.932486 apysc-2.8.0/apysc/_color/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_color/color_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.932486 apysc-2.8.0/apysc/_console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_console/_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31060 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_console/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_console/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.932486 apysc-2.8.0/apysc/_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_converter/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_converter/to_apysc_val_from_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_converter/to_builtin_val_from_apysc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.952486 apysc-2.8.0/apysc/_display/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/any_display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_fill_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_fill_color_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_line_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_line_cap_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_line_color_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_line_joints_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_line_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_line_thickness_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_x_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/append_y_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/begin_fill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/css_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/ellipse_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/ellipse_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/flip_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/flip_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/flip_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/get_bounds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47941 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/graphics_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/graphics_clear_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/graphics_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_cap_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_caps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_dash_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_dash_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_joints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_joints_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_round_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_style_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/points_2d_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/points_var_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polygon_append_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polygon_apply_current_points_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polygon_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polygon_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polygon_x3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polygon_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polygon_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polygon_y3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16471 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18581 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/rotation_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/scale_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/set_lower_scale_limit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/set_overflow_visible_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/skew_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/skew_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_set_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_set_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_set_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_set_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_set_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_set_font_size_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_set_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_set_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_set_text_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_singleton_for_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/svg_text_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/visible_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/width_and_height_mixin_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/x_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/y_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_display/y_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.956486 apysc-2.8.0/apysc/_event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/custom_event_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/custom_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/document_mouse_wheel_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/double_click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/enter_frame_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/enter_frame_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/handler_circular_calling_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_down_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_event_binding_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_event_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_event_unbinding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_out_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_over_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/mouse_up_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/prevent_default_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/set_handler_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/stop_propagation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_event/wheel_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.956486 apysc-2.8.0/apysc/_expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_expression/event_handler_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_expression/expression_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_expression/expression_variables_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_expression/indent_num.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_expression/js_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_expression/last_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_expression/var_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.956486 apysc-2.8.0/apysc/_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_file/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_file/module_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.960486 apysc-2.8.0/apysc/_geom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_control_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_control_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_control_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_control_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_control_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_control_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_dest_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_dest_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/path_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/rectangle_geom_bottom_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/rectangle_geom_center_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/rectangle_geom_center_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/rectangle_geom_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/rectangle_geom_left_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/rectangle_geom_right_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/rectangle_geom_top_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/rectangle_geom_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_geom/relative_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.960486 apysc-2.8.0/apysc/_html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_html/debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_html/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_html/html_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_html/html_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.964486 apysc-2.8.0/apysc/_jslib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_jslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_jslib/jquery-3.6.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_jslib/jslib_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78572 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_jslib/svg-3.1.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_jslib/underscore-1.12.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.964486 apysc-2.8.0/apysc/_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_jupyter/jupyter_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.964486 apysc-2.8.0/apysc/_lint_and_doc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/conf_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/docs_keyword_link_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/docs_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/docs_toctree_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/docs_translation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/docstring_to_markdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51969 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/docstring_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/document_text_split_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/document_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.964486 apysc-2.8.0/apysc/_lint_and_doc/fixed_translation_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209108 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/lint_and_doc_hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_lint_and_doc/translation_mapping_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.968486 apysc-2.8.0/apysc/_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_loop/_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_loop/_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_loop/_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_loop/loop_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.968486 apysc-2.8.0/apysc/_math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_math/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_math/max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_math/min_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_math/trunc_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.968486 apysc-2.8.0/apysc/_string/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_string/indent_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_string/string_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.968486 apysc-2.8.0/apysc/_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_testing/e2e_testing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_testing/testing_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.972486 apysc-2.8.0/apysc/_time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/datetime_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/day_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/days_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/hour_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/left_and_right_datetimes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/millisecond_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/minute_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/month_end_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/month_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/now_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/second_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/timedelta_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/total_seconds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/weekday_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_time/year_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.972486 apysc-2.8.0/apysc/_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:13.000486 apysc-2.8.0/apysc/_translation/jp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/about_handler_options_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/add_child_and_remove_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/add_debug_info_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_base_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_base_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143972 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_method_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_pause_and_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22568 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_width_and_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/append_js_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_append_and_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_extend_and_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_index_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_insert_and_insert_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_remove_and_remove_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/array_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/assert_defined_and_undefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/assert_equal_and_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/assert_greater_and_greater_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/assert_less_and_less_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/assert_true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/assertion_basic_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25457 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/bind_and_trigger_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47227 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/contains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_hour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_millisecond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_minute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_second.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_set_month_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/datetime_year.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/dblclick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/dictionary_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/dictionary_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/dictionary_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/display_object_get_and_set_css.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/display_object_mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/display_object_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/display_object_visible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/display_object_x_and_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/display_on_colaboratory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/display_on_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/draw_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84469 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/easing_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/elif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/enter_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/fundamental_data_classes_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/get_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/get_child_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_flip_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_scale_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_scale_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_base_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_begin_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_dashed_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_round_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_round_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_draw_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62521 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_line_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/graphics_move_to_and_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/import_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18963 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/int_and_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/int_and_number_arithmetic_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/int_and_number_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/int_and_number_to_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/math_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/math_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/math_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/mouse_event_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/mouse_event_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27457 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/mousedown_and_mouseup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/mousemove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/mouseover_and_mouseout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/num_children.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60597 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49410 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51647 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/quick_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/recommended_type_checker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/remove_children.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17192 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/save_overall_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/sequential_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/set_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30948 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/string_addition_and_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/string_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/string_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47748 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44504 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timedelta_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timedelta_total_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timer_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timer_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timer_repeat_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timer_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/timer_start_and_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64293 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/unset_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/variable_name_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/what_apysc_can_do.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:13.008486 apysc-2.8.0/apysc/_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45467 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/attr_linking_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/blank_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/deleted_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/dictionary_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/expression_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/initial_substitution_exp_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34119 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/number_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/py_builtin_iter_disabling_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/repr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/revert_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/revert_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26454 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/string_lstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/string_split_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/to_fixed_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/to_string_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/type_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/value_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/variable_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/variable_name_suffix_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_type/variable_name_suffix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:13.008486 apysc-2.8.0/apysc/_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104542 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/arg_validation_decos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/bool_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/color_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/display_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/event_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/geom_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/matrix_data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/number_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/parent_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/path_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/string_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/validation_common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-28 09:11:47.000000 apysc-2.8.0/apysc/_validation/variable_name_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:12:12.916486 apysc-2.8.0/apysc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-28 09:12:12.000000 apysc-2.8.0/apysc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25016 2023-05-28 09:12:12.000000 apysc-2.8.0/apysc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:12:12.000000 apysc-2.8.0/apysc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 09:12:12.000000 apysc-2.8.0/apysc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 09:12:12.000000 apysc-2.8.0/apysc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 09:12:13.008486 apysc-2.8.0/setup.cfg
```

### Comparing `apysc-2.7.9/LICENSE` & `apysc-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/PKG-INFO` & `apysc-2.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 2.7.9
+Version: 2.8.0
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-2.7.9/README.md` & `apysc-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/__init__.py` & `apysc-2.8.0/apysc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from apysc._type.dictionary import Dictionary
 from apysc._type.any_value import AnyValue
 from apysc._branch._if import If
 from apysc._branch._elif import Elif
 from apysc._branch._else import Else
 from apysc._loop._for import For
 from apysc._loop._continue import Continue
+from apysc._loop._range import range
 from apysc._display.display_object import DisplayObject
 from apysc._display._document import document
 from apysc._display.sprite import Sprite
 from apysc._display.graphics import Graphics
 from apysc._display.stage import Stage
 from apysc._display.stage import get_stage
 from apysc._display.triangle import Triangle
@@ -49,14 +50,15 @@
 from apysc._geom.path_vertical import PathVertical
 from apysc._geom.path_close import PathClose
 from apysc._geom.path_bezier_2d import PathBezier2D
 from apysc._geom.path_bezier_2d_continual import PathBezier2DContinual
 from apysc._geom.path_bezier_3d import PathBezier3D
 from apysc._geom.path_bezier_3d_continual import PathBezier3DContinual
 from apysc._geom.path_data import PathData
+from apysc._geom.rectangle_geom import RectangleGeom
 from apysc._event.event import Event
 from apysc._event.mouse_event import MouseEvent
 from apysc._event.wheel_event import WheelEvent
 from apysc._event.timer_event import TimerEvent
 from apysc._event.animation_event import AnimationEvent
 from apysc._event.enter_frame_event import EnterFrameEvent
 from apysc._event.mouse_event_type import MouseEventType
@@ -114,9 +116,14 @@
 from apysc._animation.animation_rotation_around_point import AnimationRotationAroundPoint
 from apysc._animation.animation_scale_x_from_center import AnimationScaleXFromCenter
 from apysc._animation.animation_scale_y_from_center import AnimationScaleYFromCenter
 from apysc._animation.animation_scale_x_from_point import AnimationScaleXFromPoint
 from apysc._animation.animation_scale_y_from_point import AnimationScaleYFromPoint
 from apysc._animation.animation_parallel import AnimationParallel
 from apysc._math.math import Math
+from apysc._auto_reloading.auto_reloading_decorator import set_auto_reloading
+from apysc._chart.x_axis_settings import XAxisSettings
+from apysc._chart.y_axis_single_column_settings import YAxisSingleColumnSettings
+from apysc._chart.x_axis_label_position import XAxisLabelPosition
+from apysc._chart.y_axis_label_position import YAxisLabelPosition
 
-__version__: str = "2.7.9"
+__version__: str = "2.8.0"
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_base.py` & `apysc-2.8.0/apysc/_animation/animation_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_cx.py` & `apysc-2.8.0/apysc/_animation/animation_cx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Class implementation for the center-x animation value.
+"""Class implementation for the center x animation value.
 """
 
 from typing import Generic
 from typing import TypeVar
 from typing import Union
 
 from typing_extensions import final
@@ -15,15 +15,15 @@
 from apysc._type.variable_name_mixin import VariableNameMixIn
 
 _Target = TypeVar("_Target", bound=VariableNameMixIn)
 
 
 class AnimationCx(AnimationBase[_Target], Generic[_Target]):
     """
-    The animation class for a center-x coordinate.
+    The animation class for a center x coordinate.
 
     References
     ----------
     - animation_x interface
         - https://simon-ritchie.github.io/apysc/en/animation_x.html
     - Animation interfaces duration setting
         - https://simon-ritchie.github.io/apysc/en/animation_duration.html
@@ -63,15 +63,15 @@
         target: _Target,
         x: Union[float, Number],
         duration: Union[int, Int] = 3000,
         delay: Union[int, Int] = 0,
         easing: Easing = Easing.LINEAR,
     ) -> None:
         """
-        The animation class for a center-x coordinate.
+        The animation class for a center x coordinate.
 
         Parameters
         ----------
         target : VariableNameMixIn
             A target instance of the animation target
             (e.g., `Circle` instance).
         x : float or Number
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_cx_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_cx_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Class implementation for the animation_x mix-in
-(using center-x coordinate internally).
+(using center x coordinate internally).
 """
 
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._animation.animation_cx import AnimationCx
@@ -12,39 +12,39 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationCxMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=4)
     def animation_x(
         self,
         *,
         x: Union[float, Number],
         duration: Union[int, Int] = 3000,
         delay: Union[int, Int] = 0,
         easing: Easing = Easing.LINEAR
     ) -> AnimationCx:
         """
-        Set the center-x coordinate animation setting.
+        Set the center x coordinate animation setting.
 
         Notes
         -----
         To start this animation, you need to call the `start` method of
         the returned instance.
 
         Parameters
         ----------
         x : float or Number
-            Destination of the center-x coordinate.
+            Destination of the center x coordinate.
         duration : Int or int, default 3000
             Milliseconds before an animation ends.
         delay : Int or int, default 0
             Milliseconds before an animation starts.
         easing : Easing, default Easing.LINEAR
             Easing setting.
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_cy.py` & `apysc-2.8.0/apysc/_animation/animation_cy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Class implementation for the center-y animation value.
+"""Class implementation for the center y animation value.
 """
 
 from typing import Generic
 from typing import TypeVar
 from typing import Union
 
 from typing_extensions import final
@@ -15,15 +15,15 @@
 from apysc._type.variable_name_mixin import VariableNameMixIn
 
 _Target = TypeVar("_Target", bound=VariableNameMixIn)
 
 
 class AnimationCy(AnimationBase[_Target], Generic[_Target]):
     """
-    The animation class for a center-y coordinate.
+    The animation class for a center y coordinate.
 
     References
     ----------
     - animation_y interface
         - https://simon-ritchie.github.io/apysc/en/animation_y.html
     - Animation interfaces duration setting
         - https://simon-ritchie.github.io/apysc/en/animation_duration.html
@@ -63,15 +63,15 @@
         target: _Target,
         y: Union[float, Number],
         duration: Union[int, Int] = 3000,
         delay: Union[int, Int] = 0,
         easing: Easing = Easing.LINEAR,
     ) -> None:
         """
-        The animation class for a center-y coordinate.
+        The animation class for a center y coordinate.
 
         Parameters
         ----------
         target : VariableNameMixIn
             A target instance of the animation target
             (e.g., `Circle` instance).
         y : float or Number
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_cy_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_cy_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Class implementation for the animation_y interface
-(using center-y coordinate internally).
+(using center y coordinate internally).
 """
 
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._animation.animation_cy import AnimationCy
@@ -12,39 +12,39 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationCyMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=4)
     def animation_y(
         self,
         *,
         y: Union[float, Number],
         duration: Union[int, Int] = 3000,
         delay: Union[int, Int] = 0,
         easing: Easing = Easing.LINEAR
     ) -> AnimationCy:
         """
-        Set the center-y coordinate animation setting.
+        Set the center y coordinate animation setting.
 
         Notes
         -----
         To start this animation, you need to call the `start` method of
         the returned instance.
 
         Parameters
         ----------
         y : float or Number
-            Destination of the center-y coordinate.
+            Destination of the center y coordinate.
         duration : Int or int, default 3000
             Milliseconds before an animation ends.
         delay : Int or int, default 0
             Milliseconds before an animation starts.
         easing : Easing, default Easing.LINEAR
             Easing setting.
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_fill_alpha.py` & `apysc-2.8.0/apysc/_animation/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_fill_alpha_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_fill_alpha_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationFillAlphaMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=1, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=4)
     def animation_fill_alpha(
         self,
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_fill_color.py` & `apysc-2.8.0/apysc/_animation/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_fill_color_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_finish_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_finish_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_height.py` & `apysc-2.8.0/apysc/_animation/animation_height.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_height_for_ellipse.py` & `apysc-2.8.0/apysc/_animation/animation_height_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_height_for_ellipse_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_height_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_height_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_line_alpha.py` & `apysc-2.8.0/apysc/_animation/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_line_alpha_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_line_alpha_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationLineAlphaMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=1, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=4)
     def animation_line_alpha(
         self,
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_line_color.py` & `apysc-2.8.0/apysc/_animation/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_line_color_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_line_thickness.py` & `apysc-2.8.0/apysc/_animation/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_line_thickness_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_mixins.py` & `apysc-2.8.0/apysc/_animation/animation_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_move.py` & `apysc-2.8.0/apysc/_animation/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_move_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_move_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationMoveMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=3, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=5)
     def animation_move(
         self,
         *,
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_parallel.py` & `apysc-2.8.0/apysc/_animation/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_parallel_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_parallel_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_pause_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_pause_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_play_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_play_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_radius.py` & `apysc-2.8.0/apysc/_animation/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_radius_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_reset_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_reset_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_reverse_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_reverse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_rotation_around_center.py` & `apysc-2.8.0/apysc/_animation/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_rotation_around_center_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_rotation_around_point.py` & `apysc-2.8.0/apysc/_animation/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_rotation_around_point_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_rotation_around_point_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationRotationAroundPointMixIn(AnimationMixIns):
     @final
     @arg_validation_decos.is_integer(arg_position_index=1, optional=False)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=4, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=5, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=6)
     def animation_rotation_around_point(
         self,
         *,
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_scale_x_from_center.py` & `apysc-2.8.0/apysc/_animation/animation_scale_x_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_scale_x_from_center_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_scale_x_from_center_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationScaleXFromCenterMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=4)
     def animation_scale_x_from_center(
         self,
         *,
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_scale_x_from_point.py` & `apysc-2.8.0/apysc/_animation/animation_scale_x_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_scale_x_from_point_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_scale_x_from_point_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationScaleXFromPointMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=3, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=5)
     def animation_scale_x_from_point(
         self,
         *,
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_scale_y_from_center.py` & `apysc-2.8.0/apysc/_animation/animation_scale_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_scale_y_from_center_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_scale_y_from_center_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationScaleYFromCenterMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=4)
     def animation_scale_y_from_center(
         self,
         *,
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_scale_y_from_point.py` & `apysc-2.8.0/apysc/_animation/animation_scale_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_scale_y_from_point_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_scale_y_from_point_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationScaleYFromPointMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=3, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=5)
     def animation_scale_y_from_point(
         self,
         *,
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_time_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_time_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_width.py` & `apysc-2.8.0/apysc/_animation/animation_width.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_width_for_ellipse.py` & `apysc-2.8.0/apysc/_animation/animation_width_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_width_for_ellipse_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_width_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_width_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_x.py` & `apysc-2.8.0/apysc/_animation/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_x_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_x_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationXMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=4)
     def animation_x(
         self,
         *,
```

### Comparing `apysc-2.7.9/apysc/_animation/animation_y.py` & `apysc-2.8.0/apysc/_animation/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_animation/animation_y_mixin.py` & `apysc-2.8.0/apysc/_animation/animation_y_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class AnimationYMixIn(AnimationMixIns):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     @arg_validation_decos.num_is_gt_zero(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.is_easing(arg_position_index=4)
     def animation_y(
         self,
         *,
```

### Comparing `apysc-2.7.9/apysc/_animation/easing.py` & `apysc-2.8.0/apysc/_animation/easing.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_branch/_elif.py` & `apysc-2.8.0/apysc/_branch/_elif.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_branch/_else.py` & `apysc-2.8.0/apysc/_branch/_else.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_branch/_if.py` & `apysc-2.8.0/apysc/_branch/_if.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_branch/if_base.py` & `apysc-2.8.0/apysc/_branch/if_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_callable/callable_util.py` & `apysc-2.8.0/apysc/_callable/callable_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_color/color_util.py` & `apysc-2.8.0/apysc/_color/color_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_console/_trace.py` & `apysc-2.8.0/apysc/_console/_trace.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_console/assertion.py` & `apysc-2.8.0/apysc/_console/assertion.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_console/loggers.py` & `apysc-2.8.0/apysc/_console/loggers.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_converter/cast.py` & `apysc-2.8.0/apysc/_converter/cast.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_converter/to_apysc_val_from_builtin.py` & `apysc-2.8.0/apysc/_converter/to_apysc_val_from_builtin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_converter/to_builtin_val_from_apysc.py` & `apysc-2.8.0/apysc/_converter/to_builtin_val_from_apysc.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/_document.py` & `apysc-2.8.0/apysc/_display/_document.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/append_fill_alpha_attr_expression_mixin.py` & `apysc-2.8.0/apysc/_display/append_fill_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/append_fill_color_expression_mixin.py` & `apysc-2.8.0/apysc/_display/append_fill_color_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/append_line_alpha_attr_expression_mixin.py` & `apysc-2.8.0/apysc/_display/append_line_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/append_line_cap_attr_expression_mixin.py` & `apysc-2.8.0/apysc/_display/append_line_cap_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/append_line_color_attr_expression_mixin.py` & `apysc-2.8.0/apysc/_display/append_line_color_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/append_line_joints_attr_expression_mixin.py` & `apysc-2.8.0/apysc/_display/append_line_joints_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/append_line_point_mixin.py` & `apysc-2.8.0/apysc/_display/append_line_point_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 class AppendLinePointMixIn(
     PolygonApplyCurrentPointsMixIn,
     Points2DMixIn,
     VariableNameSuffixMixIn,
     PointsVarNameMixIn,
 ):
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def append_line_point(
         self,
         *,
         x: Union[float, Number],
         y: Union[float, Number],
     ) -> None:
```

### Comparing `apysc-2.7.9/apysc/_display/append_line_thickness_attr_expression_mixin.py` & `apysc-2.8.0/apysc/_display/append_line_thickness_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/append_x_attr_expression_mixin.py` & `apysc-2.8.0/apysc/_display/append_x_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/append_y_attr_expression_mixin.py` & `apysc-2.8.0/apysc/_display/append_y_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/begin_fill_mixin.py` & `apysc-2.8.0/apysc/_display/begin_fill_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class BeginFillMixIn(VariableNameSuffixAttrOrVarMixIn, RevertMixIn):
 
     _fill_color: String
     _fill_alpha: Number
 
     @final
     @arg_validation_decos.is_hex_color_code_format(arg_position_index=1, optional=False)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def begin_fill(
         self, *, color: StrOrString, alpha: Union[float, Number] = 1.0
     ) -> None:
         """
         Set single color value for fill.
```

### Comparing `apysc-2.7.9/apysc/_display/child_mixin.py` & `apysc-2.8.0/apysc/_display/child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/circle.py` & `apysc-2.8.0/apysc/_display/circle.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 )
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
 from apysc._display.append_x_attr_expression_mixin import AppendXAttrExpressionMixIn
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.cx_mixin import CxMixIn
 from apysc._display.cy_mixin import CyMixIn
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
 from apysc._display.flip_x_mixin import FlipXMixIn
 from apysc._display.flip_y_mixin import FlipYMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_caps import LineCaps
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_dash_dot_setting import LineDashDotSetting
 from apysc._display.line_dash_dot_setting_mixin import LineDashDotSettingMixIn
 from apysc._display.line_dash_setting import LineDashSetting
@@ -49,32 +51,39 @@
 from apysc._display.radius_mixin import RadiusMixIn
 from apysc._display.rotation_around_center_mixin import RotationAroundCenterMixIn
 from apysc._display.rotation_around_point_mixin import RotationAroundPointMixIn
 from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
 from apysc._display.scale_x_from_point_mixin import ScaleXFromPointMixIn
 from apysc._display.scale_y_from_center_mixin import ScaleYFromCenterMixIn
 from apysc._display.scale_y_from_point_mixin import ScaleYFromPointMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.attr_to_apysc_val_from_builtin_mixin import (
     AttrToApyscValFromBuiltinMixIn,
 )
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Circle(
+    ReprInterface,
     CxMixIn,
     AppendXAttrExpressionMixIn,
     CyMixIn,
     AppendYAttrExpressionMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     RotationAroundCenterMixIn,
     RotationAroundPointMixIn,
     ScaleXFromCenterMixIn,
     ScaleYFromCenterMixIn,
     ScaleXFromPointMixIn,
     ScaleYFromPointMixIn,
@@ -93,14 +102,15 @@
     AppendLineAlphaAttrExpressionMixIn,
     AppendLineThicknessAttrExpressionMixIn,
     AppendLineCapAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
     AttrToApyscValFromBuiltinMixIn,
 ):
     """
     The circle vector graphics class.
 
     References
@@ -129,17 +139,17 @@
     >>> circle.fill_color
     String("#00aaff")
     """
 
     # self
     @arg_validation_decos.multiple_line_settings_are_not_set(arg_position_index=0)
     # x
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     # y
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     # radius
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=3, optional=False)
     # fill_color
     @arg_validation_decos.is_hex_color_code_format(arg_position_index=4, optional=False)
     # fill_alpha
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=5, optional=False)
```

### Comparing `apysc-2.7.9/apysc/_display/css_mixin.py` & `apysc-2.8.0/apysc/_display/css_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         initialize it yet.
         """
         if hasattr(self, "_css"):
             return
         self._css = {}
 
     @final
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def get_css(self, *, name: Union[str, String]) -> String:
         """
         Get a CSS value string.
 
         Parameters
         ----------
@@ -99,16 +99,16 @@
         css_value_str: str = value_util.get_value_str_for_expression(value=css)
         expression: str = (
             f"{css_value_str} = {self.variable_name}." f"css({name_value_str});"
         )
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_string(arg_position_index=1)
-    @arg_validation_decos.is_string(arg_position_index=2)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_string(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def set_css(self, *, name: Union[str, String], value: Union[str, String]) -> None:
         """
         Set a specified value string to the CSS.
 
         Parameters
         ----------
```

### Comparing `apysc-2.7.9/apysc/_display/cx_mixin.py` & `apysc-2.8.0/apysc/_display/cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/cy_mixin.py` & `apysc-2.8.0/apysc/_display/cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/display_object.py` & `apysc-2.8.0/apysc/_display/display_object.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Implementations for DisplayObject class.
 """
 
 from typing import TYPE_CHECKING
 
-from typing_extensions import final
-
 from apysc._animation.animation_parallel_mixin import AnimationParallelMixIn
-from apysc._display.css_mixin import CssMixIn
+from apysc._display.css_interface import CssInterface
 from apysc._display.parent_mixin import ParentMixIn
 from apysc._display.visible_mixin import VisibleMixIn
 from apysc._event.custom_event_mixin import CustomEventMixIn
 from apysc._event.mouse_event_mixins import MouseEventMixIns
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._validation import arg_validation_decos
 
@@ -19,15 +17,15 @@
 
 
 class DisplayObject(
     ParentMixIn,
     MouseEventMixIns,
     VisibleMixIn,
     CustomEventMixIn,
-    CssMixIn,
+    CssInterface,
     AnimationParallelMixIn,
 ):
     """
     Display object (base) class for the common interfaces.
 
     References
     ----------
@@ -49,15 +47,7 @@
 
         References
         ----------
         - DisplayObject
             - https://simon-ritchie.github.io/apysc/en/display_object.html
         """
         self._variable_name = variable_name
-
-    @final
-    @add_debug_info_setting(module_name=__name__)
-    def _set_overflow_visible_setting(self) -> None:
-        """
-        Set the `visible` value to the `overflow` CSS property.
-        """
-        self.set_css(name="overflow", value="visible")
```

### Comparing `apysc-2.7.9/apysc/_display/ellipse.py` & `apysc-2.8.0/apysc/_display/ellipse.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 )
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
 from apysc._display.append_x_attr_expression_mixin import AppendXAttrExpressionMixIn
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.cx_mixin import CxMixIn
 from apysc._display.cy_mixin import CyMixIn
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
 from apysc._display.flip_x_mixin import FlipXMixIn
 from apysc._display.flip_y_mixin import FlipYMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_caps import LineCaps
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_dash_dot_setting import LineDashDotSetting
 from apysc._display.line_dash_dot_setting_mixin import LineDashDotSettingMixIn
 from apysc._display.line_dash_setting import LineDashSetting
@@ -48,35 +50,42 @@
 from apysc._display.line_round_dot_setting_mixin import LineRoundDotSettingMixIn
 from apysc._display.rotation_around_center_mixin import RotationAroundCenterMixIn
 from apysc._display.rotation_around_point_mixin import RotationAroundPointMixIn
 from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
 from apysc._display.scale_x_from_point_mixin import ScaleXFromPointMixIn
 from apysc._display.scale_y_from_center_mixin import ScaleYFromCenterMixIn
 from apysc._display.scale_y_from_point_mixin import ScaleYFromPointMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.width_and_height_mixin_for_ellipse import (
     WidthAndHeightMixInForEllipse,
 )
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.attr_to_apysc_val_from_builtin_mixin import (
     AttrToApyscValFromBuiltinMixIn,
 )
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Ellipse(
+    ReprInterface,
     CxMixIn,
     AppendXAttrExpressionMixIn,
     CyMixIn,
     AppendYAttrExpressionMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     RotationAroundCenterMixIn,
     RotationAroundPointMixIn,
     ScaleXFromCenterMixIn,
     ScaleYFromCenterMixIn,
     ScaleXFromPointMixIn,
     ScaleYFromPointMixIn,
@@ -95,14 +104,15 @@
     AppendLineAlphaAttrExpressionMixIn,
     AppendLineThicknessAttrExpressionMixIn,
     AppendLineCapAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
     AttrToApyscValFromBuiltinMixIn,
 ):
     """
     The ellipse vector graphics class.
 
     References
@@ -136,17 +146,17 @@
     >>> ellipse.fill_color
     String("#00aaff")
     """
 
     # self
     @arg_validation_decos.multiple_line_settings_are_not_set(arg_position_index=0)
     # x
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     # y
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     # width
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=3, optional=False)
     # height
     @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=4, optional=False)
     # fill_color
```

### Comparing `apysc-2.7.9/apysc/_display/ellipse_height_mixin.py` & `apysc-2.8.0/apysc/_display/ellipse_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/ellipse_width_mixin.py` & `apysc-2.8.0/apysc/_display/ellipse_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/fill_alpha_mixin.py` & `apysc-2.8.0/apysc/_display/fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/fill_color_mixin.py` & `apysc-2.8.0/apysc/_display/fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/flip_interface_helper.py` & `apysc-2.8.0/apysc/_display/flip_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/flip_x_mixin.py` & `apysc-2.8.0/apysc/_display/flip_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/flip_y_mixin.py` & `apysc-2.8.0/apysc/_display/flip_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/graphics.py` & `apysc-2.8.0/apysc/_display/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,32 +13,38 @@
 from apysc._display import path as _path
 from apysc._display import polygon as _polyg
 from apysc._display import polyline as _polyline
 from apysc._display import sprite
 from apysc._display import triangle as _triangle
 from apysc._display.begin_fill_mixin import BeginFillMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.display_object import DisplayObject
 from apysc._display.graphics_clear_mixin import GraphicsClearMixIn
 from apysc._display.line_style_mixin import LineStyleMixIn
 from apysc._display.rectangle import Rectangle
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.path_data_base import PathDataBase
 from apysc._geom.point2d import Point2D
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.array import Array
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class Graphics(
     XMixIn,
     YMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     DisplayObject,
     BeginFillMixIn,
     LineStyleMixIn,
     GraphicsClearMixIn,
     ChildMixIn,
 ):
     """
@@ -157,16 +163,16 @@
         import apysc as ap
 
         stage: ap.Stage = ap.get_stage()
         expression: str = f"var {self.variable_name} = {stage.variable_name}.nested();"
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=3, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=4, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=5, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def draw_rect(
@@ -230,16 +236,16 @@
             width=width,
             height=height,
             variable_name_suffix=variable_name_suffix,
         )
         return rectangle
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=3, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=4, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=5, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=5, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=6, optional=False)
@@ -322,16 +328,16 @@
                 ellipse_height, variable_name_suffix=variable_name_suffix
             )
         rectangle.ellipse_width = ellipse_width
         rectangle.ellipse_height = ellipse_height
         return rectangle
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=3, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=4, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def draw_circle(
         self,
         *,
@@ -390,16 +396,16 @@
             y=y,
             radius=radius,
             variable_name_suffix=variable_name_suffix,
         )
         return circle
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=3, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=4, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=5, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def draw_ellipse(
@@ -469,16 +475,16 @@
             width=width,
             height=height,
             variable_name_suffix=variable_name_suffix,
         )
         return ellipse
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=3, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def line_to(
         self,
         *,
         x: Union[float, Number],
         y: Union[float, Number],
@@ -541,16 +547,16 @@
         else:
             self._current_line.append_line_point(x=x, y=y)
             if variable_name_suffix != "":
                 self._current_line._variable_name_suffix = variable_name_suffix
         return self._current_line
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=3, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def move_to(
         self,
         *,
         x: Union[float, Number],
         y: Union[float, Number],
@@ -615,18 +621,18 @@
         """
         self._line_dot_setting = None
         self._line_dash_setting = None
         self._line_round_dot_setting = None
         self._line_dash_dot_setting = None
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=5, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def draw_line(
         self,
         *,
         x_start: Union[float, Number],
         y_start: Union[float, Number],
@@ -694,18 +700,18 @@
             ),
             variable_name_suffix=variable_name_suffix,
         )
         self._run_all_revert_methods(snapshot_name=snapshot_name)
         return line
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=5, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=5, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=6, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def draw_dotted_line(
         self,
         *,
@@ -786,18 +792,18 @@
             ),
             variable_name_suffix=variable_name_suffix,
         )
         self._run_all_revert_methods(snapshot_name=snapshot_name)
         return line
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=5, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=5, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=6, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=6, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=7, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def draw_dashed_line(
@@ -885,18 +891,18 @@
             ),
             variable_name_suffix=variable_name_suffix,
         )
         self._run_all_revert_methods(snapshot_name=snapshot_name)
         return line
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=5, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=5, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=6, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=6, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=7, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def draw_round_dotted_line(
@@ -984,18 +990,18 @@
             ),
             variable_name_suffix=variable_name_suffix,
         )
         self._run_all_revert_methods(snapshot_name=snapshot_name)
         return line
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=5, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=5, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=6, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=6, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=7, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=7, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=8, optional=False)
@@ -1148,20 +1154,20 @@
         """
         polygon: _polyg.Polygon = _polyg.Polygon._create_with_graphics(
             graphics=self, points=points, variable_name_suffix=variable_name_suffix
         )
         return polygon
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
-    @arg_validation_decos.is_num(arg_position_index=5)
-    @arg_validation_decos.is_num(arg_position_index=6)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=5, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=6, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=7, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def draw_triangle(
         self,
         *,
         x1: Union[float, Number],
         y1: Union[float, Number],
```

### Comparing `apysc-2.7.9/apysc/_display/graphics_base.py` & `apysc-2.8.0/apysc/_display/graphics_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Class implementation for graphic's base class.
 """
 
-from abc import ABC
-from abc import abstractmethod
 from typing import Optional
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._display.child_mixin import ChildMixIn
 from apysc._display.display_object import DisplayObject
@@ -22,15 +20,14 @@
 from apysc._type.number import Number
 from apysc._type.string import String
 from apysc._validation import arg_validation_decos
 
 
 class GraphicsBase(
     DisplayObject,
-    ABC,
 ):
 
     _variable_name: str
 
     @arg_validation_decos.not_empty_string(arg_position_index=1)
     @add_debug_info_setting(module_name=__name__)
     def __init__(self, *, variable_name: str) -> None:
@@ -190,14 +187,7 @@
             return
         if line_round_dot_setting is not None:
             self.line_round_dot_setting = line_round_dot_setting
             return
         if line_dash_dot_setting is not None:
             self.line_dash_dot_setting = line_dash_dot_setting
             return
-
-    @abstractmethod
-    def __repr__(self) -> str:
-        """
-        Get a string representation of this instance (for the sake of
-        debugging).
-        """
```

### Comparing `apysc-2.7.9/apysc/_display/graphics_clear_mixin.py` & `apysc-2.8.0/apysc/_display/graphics_clear_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/graphics_expression.py` & `apysc-2.8.0/apysc/_display/graphics_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/height_mixin.py` & `apysc-2.8.0/apysc/_display/height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line.py` & `apysc-2.8.0/apysc/_display/line.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 )
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
 from apysc._display.append_x_attr_expression_mixin import AppendXAttrExpressionMixIn
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.flip_x_mixin import FlipXMixIn
 from apysc._display.flip_y_mixin import FlipYMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_caps import LineCaps
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_dash_dot_setting import LineDashDotSetting
 from apysc._display.line_dash_dot_setting_mixin import LineDashDotSettingMixIn
 from apysc._display.line_dash_setting import LineDashSetting
@@ -38,32 +40,39 @@
 from apysc._display.line_round_dot_setting_mixin import LineRoundDotSettingMixIn
 from apysc._display.rotation_around_center_mixin import RotationAroundCenterMixIn
 from apysc._display.rotation_around_point_mixin import RotationAroundPointMixIn
 from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
 from apysc._display.scale_x_from_point_mixin import ScaleXFromPointMixIn
 from apysc._display.scale_y_from_center_mixin import ScaleYFromCenterMixIn
 from apysc._display.scale_y_from_point_mixin import ScaleYFromPointMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom import point2d
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Line(
+    ReprInterface,
     XMixIn,
     AppendXAttrExpressionMixIn,
     YMixIn,
     AppendYAttrExpressionMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     RotationAroundCenterMixIn,
     RotationAroundPointMixIn,
     ScaleXFromCenterMixIn,
     ScaleYFromCenterMixIn,
     ScaleXFromPointMixIn,
     ScaleYFromPointMixIn,
@@ -77,14 +86,15 @@
     AppendLineAlphaAttrExpressionMixIn,
     AppendLineThicknessAttrExpressionMixIn,
     AppendLineCapAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
 ):
     """
     The line vector graphics class.
 
     References
     ----------
```

### Comparing `apysc-2.7.9/apysc/_display/line_alpha_mixin.py` & `apysc-2.8.0/apysc/_display/line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_cap_mixin.py` & `apysc-2.8.0/apysc/_display/line_cap_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_caps.py` & `apysc-2.8.0/apysc/_display/line_caps.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_color_mixin.py` & `apysc-2.8.0/apysc/_display/line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_dash_dot_setting.py` & `apysc-2.8.0/apysc/_display/line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_dash_dot_setting_mixin.py` & `apysc-2.8.0/apysc/_display/line_dash_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_dash_setting.py` & `apysc-2.8.0/apysc/_display/line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_dash_setting_mixin.py` & `apysc-2.8.0/apysc/_display/line_dash_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_dot_setting.py` & `apysc-2.8.0/apysc/_display/line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_dot_setting_mixin.py` & `apysc-2.8.0/apysc/_display/line_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_joints.py` & `apysc-2.8.0/apysc/_display/line_joints.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_joints_mixin.py` & `apysc-2.8.0/apysc/_display/line_joints_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_round_dot_setting.py` & `apysc-2.8.0/apysc/_display/line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_round_dot_setting_mixin.py` & `apysc-2.8.0/apysc/_display/line_round_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/line_style_mixin.py` & `apysc-2.8.0/apysc/_display/line_style_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     _line_round_dot_setting: Optional[LineRoundDotSetting]
     _line_dash_dot_setting: Optional[LineDashDotSetting]
 
     @final
     @arg_validation_decos.multiple_line_settings_are_not_set(arg_position_index=0)
     @arg_validation_decos.is_hex_color_code_format(arg_position_index=1, optional=False)
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
-    @arg_validation_decos.is_num(arg_position_index=3)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=3, optional=False)
     @arg_validation_decos.is_line_cap(arg_position_index=4, optional=True)
     @arg_validation_decos.are_line_joints(arg_position_index=5, optional=True)
     @arg_validation_decos.is_line_dot_setting(arg_position_index=6)
     @arg_validation_decos.is_line_dash_setting(arg_position_index=7)
     @arg_validation_decos.is_line_round_dot_setting(arg_position_index=8)
     @arg_validation_decos.is_line_dash_dot_setting(arg_position_index=9)
```

### Comparing `apysc-2.7.9/apysc/_display/line_thickness_mixin.py` & `apysc-2.8.0/apysc/_display/line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/parent_mixin.py` & `apysc-2.8.0/apysc/_display/parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/path.py` & `apysc-2.8.0/apysc/_display/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 )
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
 from apysc._display.append_x_attr_expression_mixin import AppendXAttrExpressionMixIn
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
 from apysc._display.flip_x_mixin import FlipXMixIn
 from apysc._display.flip_y_mixin import FlipYMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_caps import LineCaps
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_dash_dot_setting import LineDashDotSetting
 from apysc._display.line_dash_dot_setting_mixin import LineDashDotSettingMixIn
 from apysc._display.line_dash_setting import LineDashSetting
@@ -52,32 +54,39 @@
 from apysc._display.line_round_dot_setting_mixin import LineRoundDotSettingMixIn
 from apysc._display.rotation_around_center_mixin import RotationAroundCenterMixIn
 from apysc._display.rotation_around_point_mixin import RotationAroundPointMixIn
 from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
 from apysc._display.scale_x_from_point_mixin import ScaleXFromPointMixIn
 from apysc._display.scale_y_from_center_mixin import ScaleYFromCenterMixIn
 from apysc._display.scale_y_from_point_mixin import ScaleYFromPointMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.path_data_base import PathDataBase
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Path(
+    ReprInterface,
     XMixIn,
     AppendXAttrExpressionMixIn,
     YMixIn,
     AppendYAttrExpressionMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     RotationAroundCenterMixIn,
     RotationAroundPointMixIn,
     ScaleXFromCenterMixIn,
     ScaleYFromCenterMixIn,
     ScaleXFromPointMixIn,
     ScaleYFromPointMixIn,
@@ -97,14 +106,15 @@
     AppendLineCapAttrExpressionMixIn,
     LineJointsMixIn,
     AppendLineJointsAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
 ):
     """
     The path vector graphics class.
 
     References
     ----------
```

### Comparing `apysc-2.7.9/apysc/_display/points_2d_mixin.py` & `apysc-2.8.0/apysc/_display/points_2d_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/polygon.py` & `apysc-2.8.0/apysc/_display/polygon.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,18 +29,20 @@
 from apysc._display.append_line_point_mixin import AppendLinePointMixIn
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
 from apysc._display.append_x_attr_expression_mixin import AppendXAttrExpressionMixIn
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
 from apysc._display.flip_x_mixin import FlipXMixIn
 from apysc._display.flip_y_mixin import FlipYMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_caps import LineCaps
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_dash_dot_setting import LineDashDotSetting
 from apysc._display.line_dash_dot_setting_mixin import LineDashDotSettingMixIn
 from apysc._display.line_dash_setting import LineDashSetting
@@ -56,36 +58,43 @@
 )
 from apysc._display.rotation_around_center_mixin import RotationAroundCenterMixIn
 from apysc._display.rotation_around_point_mixin import RotationAroundPointMixIn
 from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
 from apysc._display.scale_x_from_point_mixin import ScaleXFromPointMixIn
 from apysc._display.scale_y_from_center_mixin import ScaleYFromCenterMixIn
 from apysc._display.scale_y_from_point_mixin import ScaleYFromPointMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.set_x_and_y_with_minimum_point_interface_base import (
     SetXAndYWithMinimumPointInterfaceBase,
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.point2d import Point2D
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.array import Array
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Polygon(
+    ReprInterface,
     XMixIn,
     AppendXAttrExpressionMixIn,
     YMixIn,
     AppendYAttrExpressionMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     RotationAroundCenterMixIn,
     RotationAroundPointMixIn,
     ScaleXFromCenterMixIn,
     ScaleYFromCenterMixIn,
     ScaleXFromPointMixIn,
     ScaleYFromPointMixIn,
@@ -108,14 +117,15 @@
     LineJointsMixIn,
     AppendLineJointsAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     PolygonAppendConstructorExpressionMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
 ):
     """
     The polygon vector graphics class.
 
     References
     ----------
```

### Comparing `apysc-2.7.9/apysc/_display/polygon_append_constructor_expression_mixin.py` & `apysc-2.8.0/apysc/_display/polygon_append_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/polygon_apply_current_points_mixin.py` & `apysc-2.8.0/apysc/_display/polygon_apply_current_points_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/polygon_x1_mixin.py` & `apysc-2.8.0/apysc/_display/polygon_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/polygon_x2_mixin.py` & `apysc-2.8.0/apysc/_display/polygon_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/polygon_x3_mixin.py` & `apysc-2.8.0/apysc/_display/polygon_x3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/polygon_y1_mixin.py` & `apysc-2.8.0/apysc/_display/polygon_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/polygon_y2_mixin.py` & `apysc-2.8.0/apysc/_display/polygon_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/polygon_y3_mixin.py` & `apysc-2.8.0/apysc/_display/polygon_y3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/polyline.py` & `apysc-2.8.0/apysc/_display/polyline.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,20 @@
 from apysc._display.append_line_point_mixin import AppendLinePointMixIn
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
 from apysc._display.append_x_attr_expression_mixin import AppendXAttrExpressionMixIn
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
 from apysc._display.flip_x_mixin import FlipXMixIn
 from apysc._display.flip_y_mixin import FlipYMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_caps import LineCaps
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_dash_dot_setting import LineDashDotSetting
 from apysc._display.line_dash_dot_setting_mixin import LineDashDotSettingMixIn
 from apysc._display.line_dash_setting import LineDashSetting
@@ -54,36 +56,43 @@
 from apysc._display.line_round_dot_setting_mixin import LineRoundDotSettingMixIn
 from apysc._display.rotation_around_center_mixin import RotationAroundCenterMixIn
 from apysc._display.rotation_around_point_mixin import RotationAroundPointMixIn
 from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
 from apysc._display.scale_x_from_point_mixin import ScaleXFromPointMixIn
 from apysc._display.scale_y_from_center_mixin import ScaleYFromCenterMixIn
 from apysc._display.scale_y_from_point_mixin import ScaleYFromPointMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.set_x_and_y_with_minimum_point_interface_base import (
     SetXAndYWithMinimumPointInterfaceBase,
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.point2d import Point2D
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.array import Array
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Polyline(
+    ReprInterface,
     XMixIn,
     AppendXAttrExpressionMixIn,
     YMixIn,
     AppendYAttrExpressionMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     RotationAroundCenterMixIn,
     RotationAroundPointMixIn,
     ScaleXFromCenterMixIn,
     ScaleYFromCenterMixIn,
     ScaleXFromPointMixIn,
     ScaleYFromPointMixIn,
@@ -105,14 +114,15 @@
     AppendLineCapAttrExpressionMixIn,
     LineJointsMixIn,
     AppendLineJointsAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
 ):
     """
     The polyline vector graphics class.
 
     References
     ----------
```

### Comparing `apysc-2.7.9/apysc/_display/radius_mixin.py` & `apysc-2.8.0/apysc/_display/radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/rectangle.py` & `apysc-2.8.0/apysc/_display/rectangle.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,22 @@
 )
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
 from apysc._display.append_x_attr_expression_mixin import AppendXAttrExpressionMixIn
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.ellipse_height_mixin import EllipseHeightMixIn
 from apysc._display.ellipse_width_mixin import EllipseWidthMixIn
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
 from apysc._display.flip_x_mixin import FlipXMixIn
 from apysc._display.flip_y_mixin import FlipYMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.height_mixin import HeightMixIn
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_caps import LineCaps
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_dash_dot_setting import LineDashDotSetting
 from apysc._display.line_dash_dot_setting_mixin import LineDashDotSettingMixIn
@@ -54,32 +56,39 @@
 from apysc._display.line_round_dot_setting_mixin import LineRoundDotSettingMixIn
 from apysc._display.rotation_around_center_mixin import RotationAroundCenterMixIn
 from apysc._display.rotation_around_point_mixin import RotationAroundPointMixIn
 from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
 from apysc._display.scale_x_from_point_mixin import ScaleXFromPointMixIn
 from apysc._display.scale_y_from_center_mixin import ScaleYFromCenterMixIn
 from apysc._display.scale_y_from_point_mixin import ScaleYFromPointMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.width_mixin import WidthMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Rectangle(
+    ReprInterface,
     XMixIn,
     AppendXAttrExpressionMixIn,
     YMixIn,
     AppendYAttrExpressionMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     RotationAroundCenterMixIn,
     RotationAroundPointMixIn,
     ScaleXFromCenterMixIn,
     ScaleYFromCenterMixIn,
     ScaleXFromPointMixIn,
     ScaleYFromPointMixIn,
@@ -103,14 +112,15 @@
     AppendLineCapAttrExpressionMixIn,
     LineJointsMixIn,
     AppendLineJointsAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
 ):
     """
     The rectangle vector graphics class.
 
     References
     ----------
@@ -143,17 +153,17 @@
     >>> rectangle.fill_color
     String("#00aaff")
     """
 
     # self
     @arg_validation_decos.multiple_line_settings_are_not_set(arg_position_index=0)
     # x
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     # y
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     # width
     @arg_validation_decos.is_integer(arg_position_index=3, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=3, optional=False)
     # height
     @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=4, optional=False)
     # ellipse_width
```

### Comparing `apysc-2.7.9/apysc/_display/rotation_around_center_mixin.py` & `apysc-2.8.0/apysc/_display/rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/rotation_around_point_mixin.py` & `apysc-2.8.0/apysc/_display/rotation_around_point_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         self._rotation_around_point = Dictionary(
             {},
             variable_name_suffix=suffix,
             skip_init_substitution_expression_appending=True,
         )
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def get_rotation_around_point(self, *, x: Number, y: Number) -> Int:
         """
         Get a rotation value around the given coordinates.
 
         Parameters
         ----------
@@ -100,16 +100,16 @@
         rotation: ap.Int = self._rotation_around_point.get(
             key=key_exp_str, default=default_val
         )
         return rotation
 
     @final
     @arg_validation_decos.is_integer(arg_position_index=1, optional=False)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def set_rotation_around_point(self, *, rotation: Int, x: Number, y: Number) -> None:
         """
         Update a rotation value around the given coordinates.
 
         Parameters
         ----------
```

### Comparing `apysc-2.7.9/apysc/_display/rotation_interface_helper.py` & `apysc-2.8.0/apysc/_display/rotation_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/scale_interface_helper.py` & `apysc-2.8.0/apysc/_display/scale_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/scale_x_from_center_mixin.py` & `apysc-2.8.0/apysc/_display/scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/scale_x_from_point_mixin.py` & `apysc-2.8.0/apysc/_display/scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/scale_y_from_center_mixin.py` & `apysc-2.8.0/apysc/_display/scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/scale_y_from_point_mixin.py` & `apysc-2.8.0/apysc/_display/scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/set_lower_scale_limit_mixin.py` & `apysc-2.8.0/apysc/_display/set_lower_scale_limit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/skew_x_mixin.py` & `apysc-2.8.0/apysc/_display/skew_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/skew_y_mixin.py` & `apysc-2.8.0/apysc/_display/skew_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/sprite.py` & `apysc-2.8.0/apysc/_display/sprite.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """Implementations for Sprite class.
 """
 
 from typing_extensions import final
 
 from apysc._display import graphics
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.display_object import DisplayObject
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._event.enter_frame_mixin import EnterFrameMixIn
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.revert_mixin import RevertMixIn
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
@@ -17,14 +22,17 @@
 _Graphics = graphics.Graphics
 
 
 class Sprite(
     XMixIn,
     YMixIn,
     EnterFrameMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
+    GetBoundsMixIn,
     DisplayObject,
     ChildMixIn,
     RevertMixIn,
     VariableNameSuffixMixIn,
 ):
     """
     This class is for the basic display object that
```

### Comparing `apysc-2.7.9/apysc/_display/stage.py` & `apysc-2.8.0/apysc/_display/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text.py` & `apysc-2.8.0/apysc/_display/svg_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,31 @@
 )
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
 from apysc._display.append_x_attr_expression_mixin import AppendXAttrExpressionMixIn
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
 from apysc._display.flip_x_mixin import FlipXMixIn
 from apysc._display.flip_y_mixin import FlipYMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_thickness_mixin import LineThicknessMixIn
 from apysc._display.rotation_around_center_mixin import RotationAroundCenterMixIn
 from apysc._display.rotation_around_point_mixin import RotationAroundPointMixIn
 from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
 from apysc._display.scale_x_from_point_mixin import ScaleXFromPointMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.svg_text_align_mixin import SVGTextAlign
 from apysc._display.svg_text_align_mixin import SVGTextAlignMixIn
 from apysc._display.svg_text_bold_mixin import SVGTextBoldMixIn
 from apysc._display.svg_text_font_family_mixin import SVGTextFontFamilyMixIn
 from apysc._display.svg_text_font_size_mixin import SVGTextFontSizeMixIn
@@ -60,24 +65,28 @@
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.array import Array
 from apysc._type.boolean import Boolean
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class SVGText(
+    ReprInterface,
     XMixIn,
     AppendXAttrExpressionMixIn,
     YMixIn,
     AppendYAttrExpressionMixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     RotationAroundCenterMixIn,
     RotationAroundPointMixIn,
     ScaleXFromCenterMixIn,
     ScaleXFromPointMixIn,
     FlipXMixIn,
     FlipYMixIn,
@@ -103,14 +112,15 @@
     SVGTextSetLeadingMixIn,
     SVGTextAlignMixIn,
     SVGTextSetAlignMixIn,
     SVGTextItalicMixIn,
     SVGTextSetItalicMixIn,
     SVGTextBoldMixIn,
     SVGTextSetBoldMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
 ):
     """
     The class for an SVG text.
 
     Notes
     -----
@@ -140,38 +150,38 @@
     >>> svg_text.font_size
     Int(20)
     >>> svg_text.fill_color
     String("#00aaff")
     """
 
     # text
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     # font_size
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     # font_family
     @arg_validation_decos.is_builtin_str_list_or_apysc_str_arr(
         arg_position_index=3, optional=True
     )
     # x
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     # y
-    @arg_validation_decos.is_num(arg_position_index=5)
+    @arg_validation_decos.is_num(arg_position_index=5, optional=False)
     # fill_color
     @arg_validation_decos.is_hex_color_code_format(arg_position_index=6, optional=False)
     # fill_alpha
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=7, optional=False)
     # line_color
     @arg_validation_decos.is_hex_color_code_format(arg_position_index=8, optional=False)
     # line_alpha
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=9, optional=False)
     # line_thickness
     @arg_validation_decos.is_integer(arg_position_index=10, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=10, optional=False)
     # leading
-    @arg_validation_decos.is_num(arg_position_index=11)
+    @arg_validation_decos.is_num(arg_position_index=11, optional=False)
     # align
     @arg_validation_decos.is_svg_text_align(arg_position_index=12)
     # bold
     @arg_validation_decos.is_boolean(arg_position_index=13, optional=False)
     # italic
     @arg_validation_decos.is_boolean(arg_position_index=14, optional=False)
     # parent
@@ -238,15 +248,15 @@
         line_thickness : int or Int, optional
             A line-thickness (line-width) setting.
         leading : float or Number, optional
             A text-leading size.
         align : SVGTextAlign, default SVGTextAlign.LEFT
             A text-align setting.
         bold : Union[bool, Boolean], optional
-            A boolean, whether this text is bold style or not.
+            A boolean, whether this text is a bold style or not.
         italic : Union[bool, Boolean], optional
             A boolean, whether a text is an italic style or not (normal).
         parent : ChildMixIn or None, optional
             A parent instance to add this instance.
             If a specified value is None, this interface uses
             a stage instance.
         variable_name_suffix : str, optional
@@ -353,30 +363,30 @@
     # font_size
     @arg_validation_decos.is_integer(arg_position_index=2, optional=False)
     # font_family
     @arg_validation_decos.is_builtin_str_list_or_apysc_str_arr(
         arg_position_index=3, optional=True
     )
     # x
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     # y
-    @arg_validation_decos.is_num(arg_position_index=5)
+    @arg_validation_decos.is_num(arg_position_index=5, optional=False)
     # fill_color
     @arg_validation_decos.is_hex_color_code_format(arg_position_index=6, optional=False)
     # fill_alpha
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=7, optional=False)
     # line_color
     @arg_validation_decos.is_hex_color_code_format(arg_position_index=8, optional=False)
     # line_alpha
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=9, optional=False)
     # line_thickness
     @arg_validation_decos.is_integer(arg_position_index=10, optional=False)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=10, optional=False)
     # leading
-    @arg_validation_decos.is_num(arg_position_index=11)
+    @arg_validation_decos.is_num(arg_position_index=11, optional=False)
     # align
     @arg_validation_decos.is_svg_text_align(arg_position_index=12)
     # bold
     @arg_validation_decos.is_boolean(arg_position_index=13, optional=False)
     # italic
     @arg_validation_decos.is_boolean(arg_position_index=14, optional=False)
     # parent
@@ -444,15 +454,15 @@
         line_thickness : int or Int, optional
             A line-thickness (line-width) setting for an overall text.
         leading : float or Number, optional
             A text-leading size for an overall text.
         align : SVGTextAlign, optional
             A text-align setting for an overall text.
         bold : Union[bool, Boolean], optional
-            A boolean, whether this text is bold style or not.
+            A boolean, whether this text is a bold style or not.
         italic : Union[bool, Boolean], optional
             A boolean, whether a text is an italic style or not (normal).
         parent : Optional[ChildMixIn], optional
             A parent instance to add this instance.
             If a specified value is None, this interface uses
             a stage instance.
         variable_name_suffix : str, optional
@@ -553,9 +563,10 @@
 
         Returns
         -------
         repr_str : str
             This interface returns a type name and variable name
             (e.g., `SVGText("<variable_name>")`).
         """
-        repr_str: str = f'{SVGText.__name__}("{self._variable_name}")'
+
+        repr_str: str = f'{SVGText.__name__}("{self.variable_name}")'
         return repr_str
```

### Comparing `apysc-2.7.9/apysc/_display/svg_text_align_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_bold_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_bold_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def bold(self) -> Boolean:
         """
         Get a boolean whether this text is a bold style or not.
 
         Returns
         -------
         bold_ : Boolean
-            A boolean, whether this text is bold style or not.
+            A boolean, whether this text is a bold style or not.
         """
         import apysc as ap
         from apysc._type.variable_name_suffix_utils import (
             get_attr_or_variable_name_suffix,
         )
 
         suffix: str = get_attr_or_variable_name_suffix(
@@ -48,15 +48,15 @@
     def bold(self, value: Boolean) -> None:
         """
         Set a boolean whether this text is a bold style or not.
 
         Parameters
         ----------
         value : Boolean
-            A boolean, whether this text is bold style or not.
+            A boolean, whether this text is a bold style or not.
         """
         import apysc as ap
 
         self._bold = value._value
         expression: str = (
             f"if ({value.variable_name}) {{"
             f'\n  {self.variable_name}.font("weight", "bold");'
```

### Comparing `apysc-2.7.9/apysc/_display/svg_text_delta_x_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_delta_y_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_font_family_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_font_size_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_italic_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_leading_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_set_align_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_set_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_set_bold_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_set_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_set_delta_x_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_set_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_set_delta_y_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_set_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_set_font_family_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_set_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_set_font_size_value_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_set_font_size_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_set_italic_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_set_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_set_leading_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_set_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_set_text_value_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_set_text_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_singleton_for_text_span.py` & `apysc-2.8.0/apysc/_display/svg_text_singleton_for_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/svg_text_span.py` & `apysc-2.8.0/apysc/_display/svg_text_span.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,25 @@
 )
 from apysc._display.append_line_color_attr_expression_mixin import (
     AppendLineColorAttrExpressionMixIn,
 )
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_thickness_mixin import LineThicknessMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.svg_text_bold_mixin import SVGTextBoldMixIn
 from apysc._display.svg_text_delta_x_mixin import SVGTextDeltaXMixIn
 from apysc._display.svg_text_delta_y_mixin import SVGTextDeltaYMixIn
 from apysc._display.svg_text_font_family_mixin import SVGTextFontFamilyMixIn
 from apysc._display.svg_text_font_size_mixin import SVGTextFontSizeMixIn
 from apysc._display.svg_text_italic_mixin import SVGTextItalicMixIn
 from apysc._display.svg_text_set_bold_mixin import SVGTextSetBoldMixIn
@@ -60,20 +65,24 @@
 )
 from apysc._display.svg_text_text_mixin import SVGTextTextMixIn
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.array import Array
 from apysc._type.boolean import Boolean
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class SVGTextSpan(
+    ReprInterface,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     FillColorMixIn,
     AppendFillColorAttrExpressionMixIn,
     SVGTextSkipFillColorExpAppendingMixIn,
     FillAlphaMixIn,
     AppendFillAlphaAttrExpressionMixIn,
     SVGTextSkipFillAlphaExpAppendingMixIn,
@@ -96,14 +105,15 @@
     SVGTextSetItalicMixIn,
     SVGTextBoldMixIn,
     SVGTextSetBoldMixIn,
     SVGTextDeltaXMixIn,
     SVGTextSetDeltaXMixIn,
     SVGTextDeltaYMixIn,
     SVGTextSetDeltaYMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
 ):
     """
     The class for an SVG text-span (the child class of `SVGText`).
 
     Notes
     -----
@@ -115,15 +125,15 @@
     - SVGText class
         - https://simon-ritchie.github.io/apysc/en/svg_text.html
     - SVGTextSpan class
         - https://simon-ritchie.github.io/apysc/en/svg_text_span.html
     """
 
     # text
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     # font_size
     @arg_validation_decos.is_integer(arg_position_index=2, optional=True)
     # font_family
     @arg_validation_decos.is_builtin_str_list_or_apysc_str_arr(
         arg_position_index=3, optional=True
     )
     # fill_color
@@ -138,17 +148,17 @@
     @arg_validation_decos.is_integer(arg_position_index=8, optional=True)
     @arg_validation_decos.num_is_gte_zero(arg_position_index=8, optional=True)
     # bold
     @arg_validation_decos.is_boolean(arg_position_index=9, optional=True)
     # italic
     @arg_validation_decos.is_boolean(arg_position_index=10, optional=True)
     # delta_x
-    @arg_validation_decos.is_num(arg_position_index=11)
+    @arg_validation_decos.is_num(arg_position_index=11, optional=False)
     # delta_y
-    @arg_validation_decos.is_num(arg_position_index=12)
+    @arg_validation_decos.is_num(arg_position_index=12, optional=False)
     # variable_name_suffix
     @arg_validation_decos.is_builtin_string(arg_position_index=13, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         *,
         text: Union[str, String],
@@ -196,15 +206,15 @@
         line_color : Optional[Union[str, String]], optional
             A line-color setting.
         line_alpha : Optional[Union[float, Number]], optional
             A line-alpha setting.
         line_thickness : Optional[Union[int, Int]], optional
             A line-thickness (line-width) to set.
         bold : Optional[Union[bool, Boolean]], optional
-            A boolean, whether this text is bold style or not.
+            A boolean, whether this text is a bold style or not.
         italic : Optional[Union[bool, Boolean]], optional
             A boolean, whether a text is an italic style or not (normal).
         delta_x : Union[float, Number], optional
             A coordinate delta-x setting.
             Notes: This setting also changes a coordinate of subsequent
             `SVGTextSpan`'s instance.
         delta_y : Union[float, Number], optional
```

### Comparing `apysc-2.7.9/apysc/_display/svg_text_text_mixin.py` & `apysc-2.8.0/apysc/_display/svg_text_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/triangle.py` & `apysc-2.8.0/apysc/_display/triangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 )
 from apysc._display.append_line_thickness_attr_expression_mixin import (
     AppendLineThicknessAttrExpressionMixIn,
 )
 from apysc._display.append_x_attr_expression_mixin import AppendXAttrExpressionMixIn
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
+from apysc._display.css_mixin import CssMixIn
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
 from apysc._display.flip_x_mixin import FlipXMixIn
 from apysc._display.flip_y_mixin import FlipYMixIn
+from apysc._display.get_bounds_mixin import GetBoundsMixIn
 from apysc._display.graphics_base import GraphicsBase
 from apysc._display.line_alpha_mixin import LineAlphaMixIn
 from apysc._display.line_caps import LineCaps
 from apysc._display.line_color_mixin import LineColorMixIn
 from apysc._display.line_dash_dot_setting import LineDashDotSetting
 from apysc._display.line_dash_dot_setting_mixin import LineDashDotSettingMixIn
 from apysc._display.line_dash_setting import LineDashSetting
@@ -60,39 +62,46 @@
 from apysc._display.polygon_y3_mixin import PolygonY3MixIn
 from apysc._display.rotation_around_center_mixin import RotationAroundCenterMixIn
 from apysc._display.rotation_around_point_mixin import RotationAroundPointMixIn
 from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
 from apysc._display.scale_x_from_point_mixin import ScaleXFromPointMixIn
 from apysc._display.scale_y_from_center_mixin import ScaleYFromCenterMixIn
 from apysc._display.scale_y_from_point_mixin import ScaleYFromPointMixIn
+from apysc._display.set_overflow_visible_setting_mixin import (
+    SetOverflowVisibleSettingMixIn,
+)
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.point2d import Point2D
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.array import Array
 from apysc._type.int import Int
 from apysc._type.number import Number
+from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Triangle(
+    ReprInterface,
     XMixIn,
     AppendXAttrExpressionMixIn,
     YMixIn,
     AppendYAttrExpressionMixIn,
     PolygonX1MixIn,
     PolygonY1MixIn,
     PolygonX2MixIn,
     PolygonY2MixIn,
     PolygonX3MixIn,
     PolygonY3MixIn,
+    SetOverflowVisibleSettingMixIn,
+    CssMixIn,
     GraphicsBase,
     RotationAroundCenterMixIn,
     RotationAroundPointMixIn,
     ScaleXFromCenterMixIn,
     ScaleYFromCenterMixIn,
     ScaleXFromPointMixIn,
     ScaleYFromPointMixIn,
@@ -113,14 +122,15 @@
     LineJointsMixIn,
     AppendLineJointsAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     PolygonAppendConstructorExpressionMixIn,
+    GetBoundsMixIn,
     VariableNameSuffixMixIn,
 ):
     """
     The triangle vector graphics class.
 
     References
     ----------
@@ -148,25 +158,25 @@
     >>> triangle.y1
     Number(30.0)
     """
 
     # self
     @arg_validation_decos.multiple_line_settings_are_not_set(arg_position_index=0)
     # x1
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     # y1
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     # x2
-    @arg_validation_decos.is_num(arg_position_index=3)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
     # y2
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     # x3
-    @arg_validation_decos.is_num(arg_position_index=5)
+    @arg_validation_decos.is_num(arg_position_index=5, optional=False)
     # y3
-    @arg_validation_decos.is_num(arg_position_index=6)
+    @arg_validation_decos.is_num(arg_position_index=6, optional=False)
     # fill_color
     @arg_validation_decos.is_hex_color_code_format(arg_position_index=7, optional=False)
     # fill_alpha
     @arg_validation_decos.num_is_0_to_1_range(arg_position_index=8, optional=False)
     # line_color
     @arg_validation_decos.is_hex_color_code_format(arg_position_index=9, optional=False)
     # line_alpha
```

### Comparing `apysc-2.7.9/apysc/_display/visible_mixin.py` & `apysc-2.8.0/apysc/_display/visible_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/width_and_height_mixin_for_ellipse.py` & `apysc-2.8.0/apysc/_display/width_and_height_mixin_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/width_mixin.py` & `apysc-2.8.0/apysc/_display/width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/x_interface.py` & `apysc-2.8.0/apysc/_display/x_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/x_mixin.py` & `apysc-2.8.0/apysc/_display/x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/y_interface.py` & `apysc-2.8.0/apysc/_display/y_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_display/y_mixin.py` & `apysc-2.8.0/apysc/_display/y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/animation_event.py` & `apysc-2.8.0/apysc/_event/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/click_mixin.py` & `apysc-2.8.0/apysc/_event/click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/custom_event_mixin.py` & `apysc-2.8.0/apysc/_event/custom_event_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/document_mouse_wheel_func.py` & `apysc-2.8.0/apysc/_event/document_mouse_wheel_func.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/double_click_mixin.py` & `apysc-2.8.0/apysc/_event/double_click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/enter_frame_event.py` & `apysc-2.8.0/apysc/_event/enter_frame_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/enter_frame_mixin.py` & `apysc-2.8.0/apysc/_event/enter_frame_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/event.py` & `apysc-2.8.0/apysc/_event/event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/handler.py` & `apysc-2.8.0/apysc/_event/handler.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/handler_circular_calling_util.py` & `apysc-2.8.0/apysc/_event/handler_circular_calling_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/mouse_down_mixin.py` & `apysc-2.8.0/apysc/_event/mouse_down_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/mouse_event.py` & `apysc-2.8.0/apysc/_event/mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/mouse_event_binding_expression_mixin.py` & `apysc-2.8.0/apysc/_event/mouse_event_binding_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/mouse_event_mixins.py` & `apysc-2.8.0/apysc/_event/mouse_event_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/mouse_event_unbinding_mixin.py` & `apysc-2.8.0/apysc/_event/mouse_event_unbinding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/mouse_move_mixin.py` & `apysc-2.8.0/apysc/_event/mouse_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/mouse_out_mixin.py` & `apysc-2.8.0/apysc/_event/mouse_out_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/mouse_over_mixin.py` & `apysc-2.8.0/apysc/_event/mouse_over_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/mouse_up_mixin.py` & `apysc-2.8.0/apysc/_event/mouse_up_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/prevent_default_mixin.py` & `apysc-2.8.0/apysc/_event/prevent_default_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/set_handler_data_mixin.py` & `apysc-2.8.0/apysc/_event/set_handler_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/stop_propagation_mixin.py` & `apysc-2.8.0/apysc/_event/stop_propagation_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/timer_event.py` & `apysc-2.8.0/apysc/_event/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_event/wheel_event.py` & `apysc-2.8.0/apysc/_event/wheel_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_expression/event_handler_scope.py` & `apysc-2.8.0/apysc/_expression/event_handler_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_expression/expression_data_util.py` & `apysc-2.8.0/apysc/_expression/expression_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_expression/expression_variables_util.py` & `apysc-2.8.0/apysc/_expression/expression_variables_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_expression/indent_num.py` & `apysc-2.8.0/apysc/_expression/indent_num.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_expression/js_functions.py` & `apysc-2.8.0/apysc/_expression/js_functions.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_expression/last_scope.py` & `apysc-2.8.0/apysc/_expression/last_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_expression/var_names.py` & `apysc-2.8.0/apysc/_expression/var_names.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_file/file_util.py` & `apysc-2.8.0/apysc/_file/file_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_file/module_util.py` & `apysc-2.8.0/apysc/_file/module_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_bezier_2d.py` & `apysc-2.8.0/apysc/_geom/path_bezier_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,18 +50,18 @@
     ...         ap.PathMoveTo(x=0, y=50),
     ...         ap.PathBezier2D(control_x=50, control_y=0, dest_x=100, dest_y=50),
     ...     ]
     ... )
     """
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=5, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=6, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         control_x: Union[float, Number],
         control_y: Union[float, Number],
@@ -162,18 +162,18 @@
             f'+ String({control_y_str}) + " " '
             f'+ String({dest_x_str}) + " " '
             f"+ String({dest_y_str})"
         )
         return svg_str
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=5, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def update_path_data(
         self,
         control_x: Union[float, Number],
         control_y: Union[float, Number],
         dest_x: Union[float, Number],
```

### Comparing `apysc-2.7.9/apysc/_geom/path_bezier_2d_continual.py` & `apysc-2.8.0/apysc/_geom/path_bezier_2d_continual.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     ...         ap.PathBezier2D(control_x=50, control_y=0, dest_x=100, dest_y=50),
     ...         ap.PathBezier2DContinual(x=150, y=50),
     ...     ]
     ... )
     """
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=3, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=4, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         x: Union[float, Number],
         y: Union[float, Number],
@@ -133,16 +133,16 @@
         svg_char_str: str = value_util.get_value_str_for_expression(value=svg_char)
         x_str: str = value_util.get_value_str_for_expression(value=self._x)
         y_str: str = value_util.get_value_str_for_expression(value=self._y)
         svg_str: str = f'{svg_char_str} + String({x_str}) + " " + String({y_str})'
         return svg_str
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=3, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def update_path_data(
         self,
         x: Union[float, Number],
         y: Union[float, Number],
         *,
```

### Comparing `apysc-2.7.9/apysc/_geom/path_bezier_3d.py` & `apysc-2.8.0/apysc/_geom/path_bezier_3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,20 +65,20 @@
     ...             control_x=100, control_y=100, dest_x=100, dest_y=50
     ...         ),
     ...     ]
     ... )
     """
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
-    @arg_validation_decos.is_num(arg_position_index=5)
-    @arg_validation_decos.is_num(arg_position_index=6)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=5, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=6, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=7, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=8, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         control_x1: Union[float, Number],
         control_y1: Union[float, Number],
@@ -201,20 +201,20 @@
             f'+ " " + String({control_y2_str}) '
             f'+ " " + String({dest_x_str}) '
             f'+ " " + String({dest_y_str})'
         )
         return svg_str
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
-    @arg_validation_decos.is_num(arg_position_index=5)
-    @arg_validation_decos.is_num(arg_position_index=6)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=5, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=6, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=7, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def update_path_data(
         self,
         control_x1: Union[float, Number],
         control_y1: Union[float, Number],
         control_x2: Union[float, Number],
```

### Comparing `apysc-2.7.9/apysc/_geom/path_bezier_3d_continual.py` & `apysc-2.8.0/apysc/_geom/path_bezier_3d_continual.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,18 +61,18 @@
     ...             control_x=100, control_y=100, dest_x=100, dest_y=50
     ...         ),
     ...     ]
     ... )
     """
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=5, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=6, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         control_x: Union[float, Number],
         control_y: Union[float, Number],
@@ -180,18 +180,18 @@
             f'+ " " + String({control_y_str}) '
             f'+ " " + String({dest_x_str}) '
             f'+ " " + String({dest_y_str})'
         )
         return svg_str
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
-    @arg_validation_decos.is_num(arg_position_index=3)
-    @arg_validation_decos.is_num(arg_position_index=4)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=4, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=5, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def update_path_data(
         self,
         control_x: Union[float, Number],
         control_y: Union[float, Number],
         dest_x: Union[float, Number],
```

### Comparing `apysc-2.7.9/apysc/_geom/path_close.py` & `apysc-2.8.0/apysc/_geom/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_control_x1_mixin.py` & `apysc-2.8.0/apysc/_geom/path_control_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_control_x2_mixin.py` & `apysc-2.8.0/apysc/_geom/path_control_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_control_x_mixin.py` & `apysc-2.8.0/apysc/_geom/path_control_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_control_y1_mixin.py` & `apysc-2.8.0/apysc/_geom/path_control_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_control_y2_mixin.py` & `apysc-2.8.0/apysc/_geom/path_control_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_control_y_mixin.py` & `apysc-2.8.0/apysc/_geom/path_control_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_data.py` & `apysc-2.8.0/apysc/_geom/path_data.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_data_base.py` & `apysc-2.8.0/apysc/_geom/path_data_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_data_util.py` & `apysc-2.8.0/apysc/_geom/path_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_dest_x_mixin.py` & `apysc-2.8.0/apysc/_geom/path_dest_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_dest_y_mixin.py` & `apysc-2.8.0/apysc/_geom/path_dest_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_horizontal.py` & `apysc-2.8.0/apysc/_geom/path_horizontal.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ...         ap.PathMoveTo(x=0, y=50),
     ...         ap.PathHorizontal(x=50),
     ...     ]
     ... )
     """
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=2, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=3, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         x: Union[float, Number],
         *,
@@ -117,15 +117,15 @@
         svg_char: String = self._get_svg_char()
         svg_char_str: str = value_util.get_value_str_for_expression(value=svg_char)
         x_str: str = value_util.get_value_str_for_expression(value=self._x)
         svg_str: str = f"{svg_char_str} + String({x_str})"
         return svg_str
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def update_path_data(
         self, x: Union[float, Number], *, relative: Union[bool, Boolean] = False
     ) -> None:
         """
         Update the path's data settings.
```

### Comparing `apysc-2.7.9/apysc/_geom/path_line_to.py` & `apysc-2.8.0/apysc/_geom/path_line_to.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     ...         ap.PathMoveTo(x=0, y=50),
     ...         ap.PathLineTo(x=50, y=50),
     ...     ]
     ... )
     """
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=3, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=4, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         x: Union[float, Number],
         y: Union[float, Number],
@@ -127,16 +127,16 @@
         svg_char_str: str = value_util.get_value_str_for_expression(value=svg_char)
         x_str: str = value_util.get_value_str_for_expression(value=self._x)
         y_str: str = value_util.get_value_str_for_expression(value=self._y)
         svg_str: str = f'{svg_char_str} + String({x_str}) + " " ' f"+ String({y_str})"
         return svg_str
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=3, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def update_path_data(
         self,
         x: Union[float, Number],
         y: Union[float, Number],
         *,
```

### Comparing `apysc-2.7.9/apysc/_geom/path_move_to.py` & `apysc-2.8.0/apysc/_geom/path_move_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     ...         ap.PathMoveTo(x=0, y=50),
     ...         ap.PathLineTo(x=50, y=50),
     ...     ]
     ... )
     """
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=3, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=4, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         x: Union[float, Number],
         y: Union[float, Number],
```

### Comparing `apysc-2.7.9/apysc/_geom/path_vertical.py` & `apysc-2.8.0/apysc/_geom/path_vertical.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ...         ap.PathMoveTo(x=0, y=50),
     ...         ap.PathVertical(y=100),
     ...     ]
     ... )
     """
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=2, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=3, optional=True)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         y: Union[float, Number],
         *,
@@ -117,15 +117,15 @@
         svg_char: String = self._get_svg_char()
         svg_char_str: str = value_util.get_value_str_for_expression(value=svg_char)
         y_str: str = value_util.get_value_str_for_expression(value=self._y)
         svg_str: str = f"{svg_char_str} + String({y_str})"
         return svg_str
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_boolean(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def update_path_data(
         self, y: Union[float, Number], *, relative: Union[bool, Boolean] = False
     ) -> None:
         """
         Update the path's data settings.
```

### Comparing `apysc-2.7.9/apysc/_geom/path_x_mixin.py` & `apysc-2.8.0/apysc/_geom/path_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/path_y_mixin.py` & `apysc-2.8.0/apysc/_geom/path_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_geom/point2d.py` & `apysc-2.8.0/apysc/_geom/point2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
     Number(0.0)
     """
 
     _x: Number
     _y: Number
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
-    @arg_validation_decos.is_num(arg_position_index=2)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=3, optional=True)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         x: Union[float, Number],
         y: Union[float, Number],
         *,
@@ -160,15 +160,15 @@
 
         suffix: str = self._get_attr_or_variable_name_suffix(value_identifier="x")
         x: ap.Number = ap.Number(self._x._value, variable_name_suffix=suffix)
         self._append_x_getter_expression(x=x)
         return x
 
     @x.setter
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def x(self, value: Number) -> None:
         """
         Update x-coordinate property.
 
         Parameters
         ----------
@@ -239,15 +239,15 @@
 
         suffix: str = self._get_attr_or_variable_name_suffix(value_identifier="y")
         y: ap.Number = ap.Number(self._y._value, variable_name_suffix=suffix)
         self._append_y_getter_expression(y=y)
         return y
 
     @y.setter
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def y(self, value: Number) -> None:
         """
         Update y-coordinate property.
 
         Parameters
         ----------
```

### Comparing `apysc-2.7.9/apysc/_geom/relative_mixin.py` & `apysc-2.8.0/apysc/_geom/relative_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_html/debug_mode.py` & `apysc-2.8.0/apysc/_html/debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_html/exporter.py` & `apysc-2.8.0/apysc/_html/exporter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_html/html_util.py` & `apysc-2.8.0/apysc/_html/html_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_jslib/jquery-3.6.3.min.js` & `apysc-2.8.0/apysc/_jslib/jquery-3.6.3.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_jslib/jquery.mousewheel-3.1.13.min.js` & `apysc-2.8.0/apysc/_jslib/jquery.mousewheel-3.1.13.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_jslib/jslib_util.py` & `apysc-2.8.0/apysc/_jslib/jslib_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_jslib/svg-3.1.2.min.js` & `apysc-2.8.0/apysc/_jslib/svg-3.1.2.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_jslib/underscore-1.12.0.min.js` & `apysc-2.8.0/apysc/_jslib/underscore-1.12.0.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_jupyter/jupyter_util.py` & `apysc-2.8.0/apysc/_jupyter/jupyter_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py` & `apysc-2.8.0/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/conf_common.py` & `apysc-2.8.0/apysc/_lint_and_doc/conf_common.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/docs_keyword_link_mapping.py` & `apysc-2.8.0/apysc/_lint_and_doc/docs_keyword_link_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,8 +188,15 @@
     "Math.max": "math_max",
     "Math.trunc": "math_trunc",
     "delete_line_dot_setting": "graphics_base_line_dot_setting",
     "delete_line_dash_setting": "graphics_base_line_dash_setting",
     "delete_line_round_dot_setting": "graphics_base_line_round_dot_setting",
     "delete_line_dash_dot_setting": "graphics_base_line_dash_dot_setting",
     "draw_triangle": "graphics_draw_triangle",
+    "SVGText": "svg_text",
+    "SVGTextSpan": "svg_text_span",
+    "create_with_svg_text_spans": "svg_text_span",
+    "get_bounds": "get_bounds",
+    "RectangleGeom": "rectangle_geom",
+    "to_string": "to_string",
+    "range": "range",
 }
```

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/docs_lang.py` & `apysc-2.8.0/apysc/_lint_and_doc/docs_lang.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/docs_toctree_util.py` & `apysc-2.8.0/apysc/_lint_and_doc/docs_toctree_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/docs_translation_converter.py` & `apysc-2.8.0/apysc/_lint_and_doc/docs_translation_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/docstring_to_markdown_converter.py` & `apysc-2.8.0/apysc/_lint_and_doc/docstring_to_markdown_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/docstring_util.py` & `apysc-2.8.0/apysc/_lint_and_doc/docstring_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/document_text_split_util.py` & `apysc-2.8.0/apysc/_lint_and_doc/document_text_split_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/document_util.py` & `apysc-2.8.0/apysc/_lint_and_doc/document_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py` & `apysc-2.8.0/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/fixed_translation_mapping/jp.py` & `apysc-2.8.0/apysc/_lint_and_doc/fixed_translation_mapping/jp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3595,15 +3595,15 @@
             val="  - テキストの行間のサイズ。",
         ),
         Mapping(
             key="  - A text-align setting.",
             val="  - テキストの行揃えの設定。",
         ),
         Mapping(
-            key="  - A boolean, whether this text is bold style or not.",
+            key="  - A boolean, whether this text is a bold style or not.",
             val="  - テキストに太字のスタイル設定を行うかどうかの真偽値。",
         ),
         Mapping(
             key="  - A boolean, whether a text is an italic style or not (normal).",
             val="  - テキストを斜体表示のスタイル設定を行うかどうかの真偽値。",
         ),
         Mapping(
@@ -3735,9 +3735,181 @@
             key="SVGTextSpan class",
             val="SVGTextSpan クラス",
         ),
         Mapping(
             key=" ・SVGText's y-coordinate zero-position starts at the bottom of a text. So if you set y=0, a text becomes almost invisible.<hr>",
             val=" ・SVGTextクラスの座標の0の位置はテキストの下部からスタートします。そのためもしもy=0を指定した場合、テキストはほとんど見えない状態になります。<hr>",
         ),
+        Mapping(
+            key="## RectangleGeom constructor API",
+            val="## RectangleGeom クラスのコンストラクタのAPI",
+        ),
+        Mapping(
+            key="The rectangle's geometry class.<hr>",
+            val="四角の幾何学情報を扱うためのクラスです。<hr>",
+        ),
+        Mapping(
+            key="  - The rectangle left x coordinate.",
+            val="  - 四角の左端のX座標。",
+        ),
+        Mapping(
+            key="  - The rectangle center x coordinate.",
+            val="  - 四角の中央のX座標。",
+        ),
+        Mapping(
+            key="  - The rectangle right x coordinate.",
+            val="  - 四角の右端のX座標。",
+        ),
+        Mapping(
+            key="  - The rectangle top y coordinate.",
+            val="  - 四角の上端のY座標。",
+        ),
+        Mapping(
+            key="  - The rectangle center y coordinate.",
+            val="  - 四角の中央のY座標。",
+        ),
+        Mapping(
+            key="  - The rectangle bottom y coordinate.",
+            val="  - 四角の下端のY座標。",
+        ),
+        Mapping(
+            key="  - The rectangle width.",
+            val="  - 四角の幅。",
+        ),
+        Mapping(
+            key="  - The Rectangle height.",
+            val="  - 四角の高さ。",
+        ),
+        Mapping(
+            key="## RectangleGeom left_x property API",
+            val="## RectangleGeom クラスの left_x 属性のAPI",
+        ),
+        Mapping(
+            key="Get the rectangle left x coordinate.<hr>",
+            val="四角の左端のX座標を取得します。<hr>",
+        ),
+        Mapping(
+            key="## RectangleGeom center_x property API",
+            val="## RectangleGeom クラスの center_x 属性のAPI",
+        ),
+        Mapping(
+            key="Get the rectangle center x coordinate.<hr>",
+            val="四角の中央のX座標を取得します。<hr>",
+        ),
+        Mapping(
+            key="## RectangleGeom right_x property API",
+            val="## RectangleGeom クラスの right_x 属性のAPI",
+        ),
+        Mapping(
+            key="Get the rectangle right x coordinate.<hr>",
+            val="四角の右端のX座標を取得します。<hr>",
+        ),
+        Mapping(
+            key="## RectangleGeom top_y property API",
+            val="## RectangleGeom クラスの top_y 属性のAPI",
+        ),
+        Mapping(
+            key="Get the rectangle top y coordinate.<hr>",
+            val="四角の上端のY座標を取得します。<hr>",
+        ),
+        Mapping(
+            key="## RectangleGeom center_y property API",
+            val="## RectangleGeom クラスの center_y 属性のAPI",
+        ),
+        Mapping(
+            key="Get the rectangle center y coordinate.<hr>",
+            val="四角の中央のY座標を取得します。<hr>",
+        ),
+        Mapping(
+            key="## RectangleGeom bottom_y property API",
+            val="## RectangleGeom クラスの bottom_y 属性のAPI",
+        ),
+        Mapping(
+            key="Get the rectangle bottom y coordinate.<hr>",
+            val="四角の下端のY座標を取得します。<hr>",
+        ),
+        Mapping(
+            key="## RectangleGeom width property API",
+            val="## RectangleGeom クラスの width 属性のAPI",
+        ),
+        Mapping(
+            key="Get the rectangle geometry width.<hr>",
+            val="四角の幅の値を取得します。<hr>",
+        ),
+        Mapping(
+            key="  - The rectangle geometry width.",
+            val="  - 四角の幅の値。",
+        ),
+        Mapping(
+            key="## RectangleGeom height property API",
+            val="## RectangleGeom の height 属性のAPI",
+        ),
+        Mapping(
+            key="Get the rectangle geometry height.<hr>",
+            val="四角の高さの値を取得します。<hr>",
+        ),
+        Mapping(
+            key="  - The rectangle geometry height.",
+            val="  - 四角の高さの値。",
+        ),
+        Mapping(
+            key="## get_bounds method API",
+            val="## get_bounds メソッドのAPI",
+        ),
+        Mapping(
+            key="Get an instance's bounding-box geometry data.<hr>",
+            val="インスタンスのバウンディングボックスの幾何データを取得します。<hr>",
+        ),
+        Mapping(
+            key="  - An instance's bounding-box geometry data.",
+            val="  - インスタンスのバウンディングボックスの幾何データ。",
+        ),
+        Mapping(
+            key="RectangleGeom class",
+            val="RectangleGeom クラス",
+        ),
+        Mapping(
+            key="get_bounds interface",
+            val="get_bounds インターフェイス",
+        ),
+        Mapping(
+            key="## to_string method API",
+            val="## to_string メソッドのAPI",
+        ),
+        Mapping(
+            key="Convert this instance to a string.<hr>",
+            val="このインスタンスを文字列へと変換します。<hr>",
+        ),
+        Mapping(
+            key="  - A converted string.",
+            val="  - 変換された文字列。",
+        ),
+        Mapping(
+            key="## What function is this?",
+            val="## 関数概要",
+        ),
+        Mapping(
+            key="## range function API",
+            val="## range 関数のAPI",
+        ),
+        Mapping(
+            key="Create a range array of integers.<hr>",
+            val="整数の指定範囲の配列を生成します。<hr>",
+        ),
+        Mapping(
+            key="  - A created array.",
+            val="  - 生成された配列。",
+        ),
+        Mapping(
+            key="## to_fixed API",
+            val="## to_fixed API",
+        ),
+        Mapping(
+            key="Convert value to fixed floating point string notation.<hr>",
+            val="値を固定の小数点以下の桁数の文字列へと変換します。<hr>",
+        ),
+        Mapping(
+            key="  - A floating point digit number (0 to 100 value is acceptable).",
+            val="  - 浮動小数点数の桁数（0～100の範囲の値を受け付けることができます）。",
+        ),
     ]
 )
```

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/lint_and_doc_hash_util.py` & `apysc-2.8.0/apysc/_lint_and_doc/lint_and_doc_hash_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_lint_and_doc/translation_mapping_utils.py` & `apysc-2.8.0/apysc/_lint_and_doc/translation_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_loop/_continue.py` & `apysc-2.8.0/apysc/_loop/_continue.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_loop/_for.py` & `apysc-2.8.0/apysc/_loop/_for.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_loop/loop_count.py` & `apysc-2.8.0/apysc/_loop/loop_count.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_math/max_mixin.py` & `apysc-2.8.0/apysc/_math/max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_math/min_mixin.py` & `apysc-2.8.0/apysc/_math/min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_math/trunc_mixin.py` & `apysc-2.8.0/apysc/_math/trunc_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_string/indent_util.py` & `apysc-2.8.0/apysc/_string/indent_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_string/string_util.py` & `apysc-2.8.0/apysc/_string/string_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_testing/e2e_testing_helper.py` & `apysc-2.8.0/apysc/_testing/e2e_testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_testing/testing_helper.py` & `apysc-2.8.0/apysc/_testing/testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/datetime_.py` & `apysc-2.8.0/apysc/_time/datetime_.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/day_mixin.py` & `apysc-2.8.0/apysc/_time/day_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/days_mixin.py` & `apysc-2.8.0/apysc/_time/days_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/fps.py` & `apysc-2.8.0/apysc/_time/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/hour_mixin.py` & `apysc-2.8.0/apysc/_time/hour_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/left_and_right_datetimes_mixin.py` & `apysc-2.8.0/apysc/_time/left_and_right_datetimes_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/millisecond_mixin.py` & `apysc-2.8.0/apysc/_time/millisecond_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/minute_mixin.py` & `apysc-2.8.0/apysc/_time/minute_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/month_end_mixin.py` & `apysc-2.8.0/apysc/_time/month_end_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/month_mixin.py` & `apysc-2.8.0/apysc/_time/month_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/now_mixin.py` & `apysc-2.8.0/apysc/_time/now_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/second_mixin.py` & `apysc-2.8.0/apysc/_time/second_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/timedelta_.py` & `apysc-2.8.0/apysc/_time/timedelta_.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/timer.py` & `apysc-2.8.0/apysc/_time/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/total_seconds_mixin.py` & `apysc-2.8.0/apysc/_time/total_seconds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/weekday_mixin.py` & `apysc-2.8.0/apysc/_time/weekday_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_time/year_mixin.py` & `apysc-2.8.0/apysc/_time/year_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/about_handler_options_type.py` & `apysc-2.8.0/apysc/_translation/jp/about_handler_options_type.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/add_child_and_remove_child.py` & `apysc-2.8.0/apysc/_translation/jp/add_child_and_remove_child.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/add_debug_info_setting.py` & `apysc-2.8.0/apysc/_translation/jp/add_debug_info_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_base_start.py` & `apysc-2.8.0/apysc/_translation/jp/animation_base_start.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_base_target.py` & `apysc-2.8.0/apysc/_translation/jp/animation_base_target.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_complete.py` & `apysc-2.8.0/apysc/_translation/jp/animation_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_delay.py` & `apysc-2.8.0/apysc/_translation/jp/animation_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_duration.py` & `apysc-2.8.0/apysc/_translation/jp/animation_duration.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_event.py` & `apysc-2.8.0/apysc/_translation/jp/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_fill_alpha.py` & `apysc-2.8.0/apysc/_translation/jp/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_fill_color.py` & `apysc-2.8.0/apysc/_translation/jp/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_finish.py` & `apysc-2.8.0/apysc/_translation/jp/animation_finish.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_interfaces_abstract.py` & `apysc-2.8.0/apysc/_translation/jp/animation_interfaces_abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ##################################################
     "## Examples of each attribute animation": "## 各属性のアニメーション設定例",
     ##################################################
     "This section will show each attribute animation example:": "この節では各属性のアニメーション設定例を表示します。",  # noqa
     ##################################################
     "<details>\n<summary>Display the code block:</summary>": "<details>\n<summary>コードブロックを表示:</summary>",  # noqa
     ##################################################
-    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=550, stage_height=550, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\nsprite.graphics.line_style(color="#fff", thickness=1)\n\nDURATION: int = 1000\nDELAY: int = 500\nEASING: ap.Easing = ap.Easing.EASE_OUT_QUINT\n\n\ndef on_x_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the x-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_x_animation_complete_2).start()\n\n\ndef on_x_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the x-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_x_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=50, width=50, height=50,).animation_x(\n    x=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_x_animation_complete_1).start()\n\n\ndef on_y_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the y-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_y_animation_complete_2).start()\n\n\ndef on_y_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the y-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_y_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=150, y=50, width=50, height=50,).animation_y(\n    y=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_y_animation_complete_1).start()\n\n\ndef on_cx_animation_complete_1(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center-x animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=275,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cx_animation_complete_2).start()\n\n\ndef on_cx_animation_complete_2(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center-x animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=325,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cx_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=275, y=75, radius=25,).animation_x(\n    x=325,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_cx_animation_complete_1).start()\n\n\ndef on_cy_animation_complete_1(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center-y animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=75,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cy_animation_complete_2).start()\n\n\ndef on_cy_animation_complete_2(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center-y animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=25,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cy_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=375, y=75, radius=25,).animation_y(\n    y=25,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_cy_animation_complete_1).start()\n\n\ndef on_move_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that move-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_move(\n        x=450,\n        y=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_move_animation_complete_2).start()\n\n\ndef on_move_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that move-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_move(\n        x=500,\n        y=0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_move_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=450, y=50, width=50, height=50,).animation_move(\n    x=500,\n    y=0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_move_animation_complete_1).start()\n\n\ndef on_width_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_width_animation_complete_2).start()\n\n\ndef on_width_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_width_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=150, width=50, height=50,).animation_width(\n    width=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_width_animation_complete_1).start()\n\n\ndef on_height_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_height_animation_complete_2).start()\n\n\ndef on_height_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_height_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=150, y=150, width=50, height=50,).animation_height(\n    height=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_height_animation_complete_1).start()\n\n\ndef on_ellipse_width_animation_complete_1(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_width_animation_complete_2).start()\n\n\ndef on_ellipse_width_animation_complete_2(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_width_animation_complete_1).start()\n\n\nsprite.graphics.draw_ellipse(x=275, y=175, width=50, height=50,).animation_width(\n    width=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_ellipse_width_animation_complete_1).start()\n\n\ndef on_ellipse_height_animation_complete_1(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_height_animation_complete_2).start()\n\n\ndef on_ellipse_height_animation_complete_2(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_height_animation_complete_1).start()\n\n\nsprite.graphics.draw_ellipse(x=375, y=175, width=50, height=50,).animation_height(\n    height=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_ellipse_height_animation_complete_1).start()\n\n\ndef on_fill_color_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_color(\n        fill_color="#0af",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_color_animation_complete_2).start()\n\n\ndef on_fill_color_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_color(\n        fill_color="#f0a",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_color_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=450, y=150, width=50, height=50,).animation_fill_color(\n    fill_color="#f0a",\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_fill_color_animation_complete_1).start()\n\n\ndef on_fill_alpha_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_alpha(\n        alpha=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_alpha_animation_complete_2).start()\n\n\ndef on_fill_alpha_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_alpha(\n        alpha=0.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_alpha_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=250, width=50, height=50,).animation_fill_alpha(\n    alpha=0.0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_fill_alpha_animation_complete_1).start()\n\n\ndef on_line_color_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_color(\n        line_color="#fff",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_color_animation_complete_2).start()\n\n\ndef on_line_color_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_color(\n        line_color="#666",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_color_animation_complete_1).start()\n\n\nsprite.graphics.line_style(color="#fff", thickness=5)\nsprite.graphics.draw_rect(x=150, y=250, width=50, height=50,).animation_line_color(\n    line_color="#666",\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_color_animation_complete_1).start()\n\n\ndef on_line_alpha_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_alpha(\n        alpha=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_alpha_animation_complete_2).start()\n\n\ndef on_line_alpha_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_alpha(\n        alpha=0.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_alpha_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=250, y=250, width=50, height=50,).animation_line_alpha(\n    alpha=0.0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_alpha_animation_complete_1).start()\nsprite.graphics.line_style(color="#fff", thickness=1)\n\n\ndef on_line_thickness_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-thickness animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_thickness(\n        thickness=1,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_thickness_animation_complete_2).start()\n\n\ndef on_line_thickness_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-thickness animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_thickness(\n        thickness=5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_thickness_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=350, y=250, width=50, height=50,).animation_line_thickness(\n    thickness=5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_thickness_animation_complete_1).start()\n\n\ndef on_radius_animation_complete_1(\n    e: ap.AnimationEvent[ap.Circle], options: dict\n) -> None:\n    """\n    The handler that the radius-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_radius(\n        radius=25,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_radius_animation_complete_2).start()\n\n\ndef on_radius_animation_complete_2(\n    e: ap.AnimationEvent[ap.Circle], options: dict\n) -> None:\n    """\n    The handler that the radius-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_radius(\n        radius=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_radius_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=475, y=275, radius=25,).animation_radius(\n    radius=50,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_radius_animation_complete_1).start()\n\n\ndef on_rotation_around_center_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_center(\n        rotation_around_center=0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_center_animation_complete_2,\n    ).start()\n\n\ndef on_rotation_around_center_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_center(\n        rotation_around_center=90,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_center_animation_complete_1,\n    ).start()\n\n\nsprite.graphics.draw_rect(\n    x=50,\n    y=350,\n    width=50,\n    height=50,\n).animation_rotation_around_center(\n    rotation_around_center=90,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_rotation_around_center_animation_complete_1\n).start()\n\n\ndef on_rotation_around_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_point(\n        rotation_around_point=0,\n        x=200,\n        y=400,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_point_animation_complete_2,\n    ).start()\n\n\ndef on_rotation_around_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_point(\n        rotation_around_point=90,\n        x=200,\n        y=400,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_point_animation_complete_1,\n    ).start()\n\n\nsprite.graphics.draw_rect(\n    x=150,\n    y=350,\n    width=50,\n    height=50,\n).animation_rotation_around_point(\n    rotation_around_point=90,\n    x=200,\n    y=400,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_rotation_around_point_animation_complete_1\n).start()\n\n\ndef on_scale_x_from_center_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_center(\n        scale_x_from_center=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_center_animation_complete_2).start()\n\n\ndef on_scale_x_from_center_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_center(\n        scale_x_from_center=0.5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_center_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=250,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_x_from_center(\n    scale_x_from_center=0.5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_x_from_center_animation_complete_1\n).start()\n\n\ndef on_scale_y_from_center_animation_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the center point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_center(\n        scale_y_from_center=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_center_animation_2).start()\n\n\ndef on_scale_y_from_center_animation_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the center point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_center(\n        scale_y_from_center=0.5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_center_animation_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=350,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_y_from_center(\n    scale_y_from_center=0.5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_y_from_center_animation_1\n).start()\n\n\ndef on_scale_x_from_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_point(\n        scale_x_from_point=1.0,\n        x=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_point_animation_complete_2).start()\n\n\ndef on_scale_x_from_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_point(\n        scale_x_from_point=0.5,\n        x=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_point_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=450,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_x_from_point(\n    scale_x_from_point=0.5,\n    x=500,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_x_from_point_animation_complete_1\n).start()\n\n\ndef on_scale_y_from_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_point(\n        scale_y_from_point=1.0,\n        y=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_point_animation_complete_2).start()\n\n\ndef on_scale_y_from_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_point(\n        scale_y_from_point=0.5,\n        y=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_point_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=50,\n    y=450,\n    width=50,\n    height=50,\n).animation_scale_y_from_point(\n    scale_y_from_point=0.5,\n    y=500,\n    duration=DURATION,\n    delay=DELAY,\n).animation_complete(\n    on_scale_y_from_point_animation_complete_1\n).start()\n\n\nap.save_overall_html(dest_dir_path="animation_interfaces_abstract_each_attr/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=550, stage_height=550, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\nsprite.graphics.line_style(color="#fff", thickness=1)\n\nDURATION: int = 1000\nDELAY: int = 500\nEASING: ap.Easing = ap.Easing.EASE_OUT_QUINT\n\n\ndef on_x_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the x-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_x_animation_complete_2).start()\n\n\ndef on_x_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the x-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_x_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=50, width=50, height=50,).animation_x(\n    x=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_x_animation_complete_1).start()\n\n\ndef on_y_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the y-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_y_animation_complete_2).start()\n\n\ndef on_y_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the y-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_y_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=150, y=50, width=50, height=50,).animation_y(\n    y=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_y_animation_complete_1).start()\n\n\ndef on_cx_animation_complete_1(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center-x animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=275,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cx_animation_complete_2).start()\n\n\ndef on_cx_animation_complete_2(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center-x animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=325,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cx_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=275, y=75, radius=25,).animation_x(\n    x=325,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_cx_animation_complete_1).start()\n\n\ndef on_cy_animation_complete_1(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center-y animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=75,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cy_animation_complete_2).start()\n\n\ndef on_cy_animation_complete_2(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center-y animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=25,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cy_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=375, y=75, radius=25,).animation_y(\n    y=25,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_cy_animation_complete_1).start()\n\n\ndef on_move_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that move-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_move(\n        x=450,\n        y=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_move_animation_complete_2).start()\n\n\ndef on_move_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that move-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_move(\n        x=500,\n        y=0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_move_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=450, y=50, width=50, height=50,).animation_move(\n    x=500,\n    y=0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_move_animation_complete_1).start()\n\n\ndef on_width_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_width_animation_complete_2).start()\n\n\ndef on_width_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_width_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=150, width=50, height=50,).animation_width(\n    width=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_width_animation_complete_1).start()\n\n\ndef on_height_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_height_animation_complete_2).start()\n\n\ndef on_height_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_height_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=150, y=150, width=50, height=50,).animation_height(\n    height=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_height_animation_complete_1).start()\n\n\ndef on_ellipse_width_animation_complete_1(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_width_animation_complete_2).start()\n\n\ndef on_ellipse_width_animation_complete_2(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_width_animation_complete_1).start()\n\n\nsprite.graphics.draw_ellipse(x=275, y=175, width=50, height=50,).animation_width(\n    width=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_ellipse_width_animation_complete_1).start()\n\n\ndef on_ellipse_height_animation_complete_1(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_height_animation_complete_2).start()\n\n\ndef on_ellipse_height_animation_complete_2(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_height_animation_complete_1).start()\n\n\nsprite.graphics.draw_ellipse(x=375, y=175, width=50, height=50,).animation_height(\n    height=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_ellipse_height_animation_complete_1).start()\n\n\ndef on_fill_color_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_color(\n        fill_color="#0af",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_color_animation_complete_2).start()\n\n\ndef on_fill_color_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_color(\n        fill_color="#f0a",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_color_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=450, y=150, width=50, height=50,).animation_fill_color(\n    fill_color="#f0a",\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_fill_color_animation_complete_1).start()\n\n\ndef on_fill_alpha_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_alpha(\n        alpha=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_alpha_animation_complete_2).start()\n\n\ndef on_fill_alpha_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_alpha(\n        alpha=0.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_alpha_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=250, width=50, height=50,).animation_fill_alpha(\n    alpha=0.0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_fill_alpha_animation_complete_1).start()\n\n\ndef on_line_color_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_color(\n        line_color="#fff",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_color_animation_complete_2).start()\n\n\ndef on_line_color_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_color(\n        line_color="#666",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_color_animation_complete_1).start()\n\n\nsprite.graphics.line_style(color="#fff", thickness=5)\nsprite.graphics.draw_rect(x=150, y=250, width=50, height=50,).animation_line_color(\n    line_color="#666",\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_color_animation_complete_1).start()\n\n\ndef on_line_alpha_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_alpha(\n        alpha=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_alpha_animation_complete_2).start()\n\n\ndef on_line_alpha_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_alpha(\n        alpha=0.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_alpha_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=250, y=250, width=50, height=50,).animation_line_alpha(\n    alpha=0.0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_alpha_animation_complete_1).start()\nsprite.graphics.line_style(color="#fff", thickness=1)\n\n\ndef on_line_thickness_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-thickness animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_thickness(\n        thickness=1,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_thickness_animation_complete_2).start()\n\n\ndef on_line_thickness_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-thickness animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_thickness(\n        thickness=5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_thickness_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=350, y=250, width=50, height=50,).animation_line_thickness(\n    thickness=5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_thickness_animation_complete_1).start()\n\n\ndef on_radius_animation_complete_1(\n    e: ap.AnimationEvent[ap.Circle], options: dict\n) -> None:\n    """\n    The handler that the radius-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_radius(\n        radius=25,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_radius_animation_complete_2).start()\n\n\ndef on_radius_animation_complete_2(\n    e: ap.AnimationEvent[ap.Circle], options: dict\n) -> None:\n    """\n    The handler that the radius-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_radius(\n        radius=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_radius_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=475, y=275, radius=25,).animation_radius(\n    radius=50,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_radius_animation_complete_1).start()\n\n\ndef on_rotation_around_center_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_center(\n        rotation_around_center=0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_center_animation_complete_2,\n    ).start()\n\n\ndef on_rotation_around_center_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_center(\n        rotation_around_center=90,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_center_animation_complete_1,\n    ).start()\n\n\nsprite.graphics.draw_rect(\n    x=50,\n    y=350,\n    width=50,\n    height=50,\n).animation_rotation_around_center(\n    rotation_around_center=90,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_rotation_around_center_animation_complete_1\n).start()\n\n\ndef on_rotation_around_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_point(\n        rotation_around_point=0,\n        x=200,\n        y=400,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_point_animation_complete_2,\n    ).start()\n\n\ndef on_rotation_around_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_point(\n        rotation_around_point=90,\n        x=200,\n        y=400,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_point_animation_complete_1,\n    ).start()\n\n\nsprite.graphics.draw_rect(\n    x=150,\n    y=350,\n    width=50,\n    height=50,\n).animation_rotation_around_point(\n    rotation_around_point=90,\n    x=200,\n    y=400,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_rotation_around_point_animation_complete_1\n).start()\n\n\ndef on_scale_x_from_center_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_center(\n        scale_x_from_center=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_center_animation_complete_2).start()\n\n\ndef on_scale_x_from_center_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_center(\n        scale_x_from_center=0.5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_center_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=250,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_x_from_center(\n    scale_x_from_center=0.5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_x_from_center_animation_complete_1\n).start()\n\n\ndef on_scale_y_from_center_animation_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the center point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_center(\n        scale_y_from_center=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_center_animation_2).start()\n\n\ndef on_scale_y_from_center_animation_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the center point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_center(\n        scale_y_from_center=0.5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_center_animation_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=350,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_y_from_center(\n    scale_y_from_center=0.5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_y_from_center_animation_1\n).start()\n\n\ndef on_scale_x_from_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_point(\n        scale_x_from_point=1.0,\n        x=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_point_animation_complete_2).start()\n\n\ndef on_scale_x_from_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_point(\n        scale_x_from_point=0.5,\n        x=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_point_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=450,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_x_from_point(\n    scale_x_from_point=0.5,\n    x=500,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_x_from_point_animation_complete_1\n).start()\n\n\ndef on_scale_y_from_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_point(\n        scale_y_from_point=1.0,\n        y=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_point_animation_complete_2).start()\n\n\ndef on_scale_y_from_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_point(\n        scale_y_from_point=0.5,\n        y=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_point_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=50,\n    y=450,\n    width=50,\n    height=50,\n).animation_scale_y_from_point(\n    scale_y_from_point=0.5,\n    y=500,\n    duration=DURATION,\n    delay=DELAY,\n).animation_complete(\n    on_scale_y_from_point_animation_complete_1\n).start()\n\n\nap.save_overall_html(dest_dir_path="animation_interfaces_abstract_each_attr/")\n```',  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=550, stage_height=550, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\nsprite.graphics.line_style(color="#fff", thickness=1)\n\nDURATION: int = 1000\nDELAY: int = 500\nEASING: ap.Easing = ap.Easing.EASE_OUT_QUINT\n\n\ndef on_x_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the x-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_x_animation_complete_2).start()\n\n\ndef on_x_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the x-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_x_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=50, width=50, height=50,).animation_x(\n    x=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_x_animation_complete_1).start()\n\n\ndef on_y_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the y-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_y_animation_complete_2).start()\n\n\ndef on_y_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the y-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_y_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=150, y=50, width=50, height=50,).animation_y(\n    y=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_y_animation_complete_1).start()\n\n\ndef on_cx_animation_complete_1(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center x animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=275,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cx_animation_complete_2).start()\n\n\ndef on_cx_animation_complete_2(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center x animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=325,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cx_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=275, y=75, radius=25,).animation_x(\n    x=325,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_cx_animation_complete_1).start()\n\n\ndef on_cy_animation_complete_1(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center y animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=75,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cy_animation_complete_2).start()\n\n\ndef on_cy_animation_complete_2(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center y animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=25,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cy_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=375, y=75, radius=25,).animation_y(\n    y=25,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_cy_animation_complete_1).start()\n\n\ndef on_move_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that move-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_move(\n        x=450,\n        y=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_move_animation_complete_2).start()\n\n\ndef on_move_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that move-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_move(\n        x=500,\n        y=0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_move_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=450, y=50, width=50, height=50,).animation_move(\n    x=500,\n    y=0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_move_animation_complete_1).start()\n\n\ndef on_width_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_width_animation_complete_2).start()\n\n\ndef on_width_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_width_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=150, width=50, height=50,).animation_width(\n    width=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_width_animation_complete_1).start()\n\n\ndef on_height_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_height_animation_complete_2).start()\n\n\ndef on_height_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_height_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=150, y=150, width=50, height=50,).animation_height(\n    height=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_height_animation_complete_1).start()\n\n\ndef on_ellipse_width_animation_complete_1(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_width_animation_complete_2).start()\n\n\ndef on_ellipse_width_animation_complete_2(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_width_animation_complete_1).start()\n\n\nsprite.graphics.draw_ellipse(x=275, y=175, width=50, height=50,).animation_width(\n    width=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_ellipse_width_animation_complete_1).start()\n\n\ndef on_ellipse_height_animation_complete_1(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_height_animation_complete_2).start()\n\n\ndef on_ellipse_height_animation_complete_2(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_height_animation_complete_1).start()\n\n\nsprite.graphics.draw_ellipse(x=375, y=175, width=50, height=50,).animation_height(\n    height=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_ellipse_height_animation_complete_1).start()\n\n\ndef on_fill_color_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_color(\n        fill_color="#0af",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_color_animation_complete_2).start()\n\n\ndef on_fill_color_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_color(\n        fill_color="#f0a",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_color_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=450, y=150, width=50, height=50,).animation_fill_color(\n    fill_color="#f0a",\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_fill_color_animation_complete_1).start()\n\n\ndef on_fill_alpha_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_alpha(\n        alpha=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_alpha_animation_complete_2).start()\n\n\ndef on_fill_alpha_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_alpha(\n        alpha=0.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_alpha_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=250, width=50, height=50,).animation_fill_alpha(\n    alpha=0.0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_fill_alpha_animation_complete_1).start()\n\n\ndef on_line_color_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_color(\n        line_color="#fff",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_color_animation_complete_2).start()\n\n\ndef on_line_color_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_color(\n        line_color="#666",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_color_animation_complete_1).start()\n\n\nsprite.graphics.line_style(color="#fff", thickness=5)\nsprite.graphics.draw_rect(x=150, y=250, width=50, height=50,).animation_line_color(\n    line_color="#666",\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_color_animation_complete_1).start()\n\n\ndef on_line_alpha_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_alpha(\n        alpha=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_alpha_animation_complete_2).start()\n\n\ndef on_line_alpha_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_alpha(\n        alpha=0.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_alpha_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=250, y=250, width=50, height=50,).animation_line_alpha(\n    alpha=0.0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_alpha_animation_complete_1).start()\nsprite.graphics.line_style(color="#fff", thickness=1)\n\n\ndef on_line_thickness_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-thickness animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_thickness(\n        thickness=1,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_thickness_animation_complete_2).start()\n\n\ndef on_line_thickness_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-thickness animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_thickness(\n        thickness=5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_thickness_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=350, y=250, width=50, height=50,).animation_line_thickness(\n    thickness=5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_thickness_animation_complete_1).start()\n\n\ndef on_radius_animation_complete_1(\n    e: ap.AnimationEvent[ap.Circle], options: dict\n) -> None:\n    """\n    The handler that the radius-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_radius(\n        radius=25,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_radius_animation_complete_2).start()\n\n\ndef on_radius_animation_complete_2(\n    e: ap.AnimationEvent[ap.Circle], options: dict\n) -> None:\n    """\n    The handler that the radius-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_radius(\n        radius=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_radius_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=475, y=275, radius=25,).animation_radius(\n    radius=50,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_radius_animation_complete_1).start()\n\n\ndef on_rotation_around_center_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_center(\n        rotation_around_center=0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_center_animation_complete_2,\n    ).start()\n\n\ndef on_rotation_around_center_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_center(\n        rotation_around_center=90,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_center_animation_complete_1,\n    ).start()\n\n\nsprite.graphics.draw_rect(\n    x=50,\n    y=350,\n    width=50,\n    height=50,\n).animation_rotation_around_center(\n    rotation_around_center=90,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_rotation_around_center_animation_complete_1\n).start()\n\n\ndef on_rotation_around_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_point(\n        rotation_around_point=0,\n        x=200,\n        y=400,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_point_animation_complete_2,\n    ).start()\n\n\ndef on_rotation_around_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_point(\n        rotation_around_point=90,\n        x=200,\n        y=400,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_point_animation_complete_1,\n    ).start()\n\n\nsprite.graphics.draw_rect(\n    x=150,\n    y=350,\n    width=50,\n    height=50,\n).animation_rotation_around_point(\n    rotation_around_point=90,\n    x=200,\n    y=400,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_rotation_around_point_animation_complete_1\n).start()\n\n\ndef on_scale_x_from_center_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_center(\n        scale_x_from_center=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_center_animation_complete_2).start()\n\n\ndef on_scale_x_from_center_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_center(\n        scale_x_from_center=0.5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_center_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=250,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_x_from_center(\n    scale_x_from_center=0.5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_x_from_center_animation_complete_1\n).start()\n\n\ndef on_scale_y_from_center_animation_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the center point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_center(\n        scale_y_from_center=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_center_animation_2).start()\n\n\ndef on_scale_y_from_center_animation_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the center point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_center(\n        scale_y_from_center=0.5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_center_animation_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=350,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_y_from_center(\n    scale_y_from_center=0.5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_y_from_center_animation_1\n).start()\n\n\ndef on_scale_x_from_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_point(\n        scale_x_from_point=1.0,\n        x=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_point_animation_complete_2).start()\n\n\ndef on_scale_x_from_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_point(\n        scale_x_from_point=0.5,\n        x=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_point_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=450,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_x_from_point(\n    scale_x_from_point=0.5,\n    x=500,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_x_from_point_animation_complete_1\n).start()\n\n\ndef on_scale_y_from_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_point(\n        scale_y_from_point=1.0,\n        y=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_point_animation_complete_2).start()\n\n\ndef on_scale_y_from_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_point(\n        scale_y_from_point=0.5,\n        y=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_point_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=50,\n    y=450,\n    width=50,\n    height=50,\n).animation_scale_y_from_point(\n    scale_y_from_point=0.5,\n    y=500,\n    duration=DURATION,\n    delay=DELAY,\n).animation_complete(\n    on_scale_y_from_point_animation_complete_1\n).start()\n\n\nap.save_overall_html(dest_dir_path="animation_interfaces_abstract_each_attr/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=550, stage_height=550, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\nsprite.graphics.line_style(color="#fff", thickness=1)\n\nDURATION: int = 1000\nDELAY: int = 500\nEASING: ap.Easing = ap.Easing.EASE_OUT_QUINT\n\n\ndef on_x_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the x-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_x_animation_complete_2).start()\n\n\ndef on_x_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the x-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_x_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=50, width=50, height=50,).animation_x(\n    x=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_x_animation_complete_1).start()\n\n\ndef on_y_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the y-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_y_animation_complete_2).start()\n\n\ndef on_y_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the y-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_y_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=150, y=50, width=50, height=50,).animation_y(\n    y=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_y_animation_complete_1).start()\n\n\ndef on_cx_animation_complete_1(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center x animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=275,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cx_animation_complete_2).start()\n\n\ndef on_cx_animation_complete_2(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center x animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_x(\n        x=325,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cx_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=275, y=75, radius=25,).animation_x(\n    x=325,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_cx_animation_complete_1).start()\n\n\ndef on_cy_animation_complete_1(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center y animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=75,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cy_animation_complete_2).start()\n\n\ndef on_cy_animation_complete_2(e: ap.AnimationEvent[ap.Circle], options: dict) -> None:\n    """\n    The handler that the center y animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_y(\n        y=25,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_cy_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=375, y=75, radius=25,).animation_y(\n    y=25,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_cy_animation_complete_1).start()\n\n\ndef on_move_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that move-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_move(\n        x=450,\n        y=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_move_animation_complete_2).start()\n\n\ndef on_move_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that move-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_move(\n        x=500,\n        y=0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_move_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=450, y=50, width=50, height=50,).animation_move(\n    x=500,\n    y=0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_move_animation_complete_1).start()\n\n\ndef on_width_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_width_animation_complete_2).start()\n\n\ndef on_width_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_width_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=150, width=50, height=50,).animation_width(\n    width=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_width_animation_complete_1).start()\n\n\ndef on_height_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_height_animation_complete_2).start()\n\n\ndef on_height_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_height_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=150, y=150, width=50, height=50,).animation_height(\n    height=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_height_animation_complete_1).start()\n\n\ndef on_ellipse_width_animation_complete_1(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_width_animation_complete_2).start()\n\n\ndef on_ellipse_width_animation_complete_2(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-width animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_width(\n        width=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_width_animation_complete_1).start()\n\n\nsprite.graphics.draw_ellipse(x=275, y=175, width=50, height=50,).animation_width(\n    width=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_ellipse_width_animation_complete_1).start()\n\n\ndef on_ellipse_height_animation_complete_1(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_height_animation_complete_2).start()\n\n\ndef on_ellipse_height_animation_complete_2(\n    e: ap.AnimationEvent[ap.Ellipse], options: dict\n) -> None:\n    """\n    The handler that the ellipse-height animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_height(\n        height=100,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_ellipse_height_animation_complete_1).start()\n\n\nsprite.graphics.draw_ellipse(x=375, y=175, width=50, height=50,).animation_height(\n    height=100,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_ellipse_height_animation_complete_1).start()\n\n\ndef on_fill_color_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_color(\n        fill_color="#0af",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_color_animation_complete_2).start()\n\n\ndef on_fill_color_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_color(\n        fill_color="#f0a",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_color_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=450, y=150, width=50, height=50,).animation_fill_color(\n    fill_color="#f0a",\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_fill_color_animation_complete_1).start()\n\n\ndef on_fill_alpha_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_alpha(\n        alpha=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_alpha_animation_complete_2).start()\n\n\ndef on_fill_alpha_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the fill-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_fill_alpha(\n        alpha=0.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_fill_alpha_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=50, y=250, width=50, height=50,).animation_fill_alpha(\n    alpha=0.0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_fill_alpha_animation_complete_1).start()\n\n\ndef on_line_color_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_color(\n        line_color="#fff",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_color_animation_complete_2).start()\n\n\ndef on_line_color_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-color animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_color(\n        line_color="#666",\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_color_animation_complete_1).start()\n\n\nsprite.graphics.line_style(color="#fff", thickness=5)\nsprite.graphics.draw_rect(x=150, y=250, width=50, height=50,).animation_line_color(\n    line_color="#666",\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_color_animation_complete_1).start()\n\n\ndef on_line_alpha_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_alpha(\n        alpha=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_alpha_animation_complete_2).start()\n\n\ndef on_line_alpha_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-alpha animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_alpha(\n        alpha=0.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_alpha_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=250, y=250, width=50, height=50,).animation_line_alpha(\n    alpha=0.0,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_alpha_animation_complete_1).start()\nsprite.graphics.line_style(color="#fff", thickness=1)\n\n\ndef on_line_thickness_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-thickness animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_thickness(\n        thickness=1,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_thickness_animation_complete_2).start()\n\n\ndef on_line_thickness_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the line-thickness animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_line_thickness(\n        thickness=5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_line_thickness_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(x=350, y=250, width=50, height=50,).animation_line_thickness(\n    thickness=5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_line_thickness_animation_complete_1).start()\n\n\ndef on_radius_animation_complete_1(\n    e: ap.AnimationEvent[ap.Circle], options: dict\n) -> None:\n    """\n    The handler that the radius-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_radius(\n        radius=25,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_radius_animation_complete_2).start()\n\n\ndef on_radius_animation_complete_2(\n    e: ap.AnimationEvent[ap.Circle], options: dict\n) -> None:\n    """\n    The handler that the radius-animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_radius(\n        radius=50,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_radius_animation_complete_1).start()\n\n\nsprite.graphics.draw_circle(x=475, y=275, radius=25,).animation_radius(\n    radius=50,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(on_radius_animation_complete_1).start()\n\n\ndef on_rotation_around_center_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_center(\n        rotation_around_center=0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_center_animation_complete_2,\n    ).start()\n\n\ndef on_rotation_around_center_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_center(\n        rotation_around_center=90,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_center_animation_complete_1,\n    ).start()\n\n\nsprite.graphics.draw_rect(\n    x=50,\n    y=350,\n    width=50,\n    height=50,\n).animation_rotation_around_center(\n    rotation_around_center=90,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_rotation_around_center_animation_complete_1\n).start()\n\n\ndef on_rotation_around_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_point(\n        rotation_around_point=0,\n        x=200,\n        y=400,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_point_animation_complete_2,\n    ).start()\n\n\ndef on_rotation_around_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the rotation around the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_rotation_around_point(\n        rotation_around_point=90,\n        x=200,\n        y=400,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(\n        on_rotation_around_point_animation_complete_1,\n    ).start()\n\n\nsprite.graphics.draw_rect(\n    x=150,\n    y=350,\n    width=50,\n    height=50,\n).animation_rotation_around_point(\n    rotation_around_point=90,\n    x=200,\n    y=400,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_rotation_around_point_animation_complete_1\n).start()\n\n\ndef on_scale_x_from_center_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_center(\n        scale_x_from_center=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_center_animation_complete_2).start()\n\n\ndef on_scale_x_from_center_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the center point animation\n    calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_center(\n        scale_x_from_center=0.5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_center_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=250,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_x_from_center(\n    scale_x_from_center=0.5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_x_from_center_animation_complete_1\n).start()\n\n\ndef on_scale_y_from_center_animation_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the center point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_center(\n        scale_y_from_center=1.0,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_center_animation_2).start()\n\n\ndef on_scale_y_from_center_animation_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the center point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_center(\n        scale_y_from_center=0.5,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_center_animation_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=350,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_y_from_center(\n    scale_y_from_center=0.5,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_y_from_center_animation_1\n).start()\n\n\ndef on_scale_x_from_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_point(\n        scale_x_from_point=1.0,\n        x=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_point_animation_complete_2).start()\n\n\ndef on_scale_x_from_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-x from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_x_from_point(\n        scale_x_from_point=0.5,\n        x=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_x_from_point_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=450,\n    y=350,\n    width=50,\n    height=50,\n).animation_scale_x_from_point(\n    scale_x_from_point=0.5,\n    x=500,\n    duration=DURATION,\n    delay=DELAY,\n    easing=EASING,\n).animation_complete(\n    on_scale_x_from_point_animation_complete_1\n).start()\n\n\ndef on_scale_y_from_point_animation_complete_1(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_point(\n        scale_y_from_point=1.0,\n        y=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_point_animation_complete_2).start()\n\n\ndef on_scale_y_from_point_animation_complete_2(\n    e: ap.AnimationEvent[ap.Rectangle], options: dict\n) -> None:\n    """\n    The handler that the scale-y from the specified point\n    animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    e.this.target.animation_scale_y_from_point(\n        scale_y_from_point=0.5,\n        y=500,\n        duration=DURATION,\n        delay=DELAY,\n        easing=EASING,\n    ).animation_complete(on_scale_y_from_point_animation_complete_1).start()\n\n\nsprite.graphics.draw_rect(\n    x=50,\n    y=450,\n    width=50,\n    height=50,\n).animation_scale_y_from_point(\n    scale_y_from_point=0.5,\n    y=500,\n    duration=DURATION,\n    delay=DELAY,\n).animation_complete(\n    on_scale_y_from_point_animation_complete_1\n).start()\n\n\nap.save_overall_html(dest_dir_path="animation_interfaces_abstract_each_attr/")\n```',  # noqa
     ##################################################
     "</details>": "</details>",
     ##################################################
     "## Easing": "## イージング",
     ##################################################
     "The easing setting can be set with the `easing` argument of each animation interface. For more details:": "イージング設定は各インターフェイスの`easing`引数で設定することができます。詳細は以下を参照してください:",  # noqa
     ##################################################
```

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_line_alpha.py` & `apysc-2.8.0/apysc/_translation/jp/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_line_color.py` & `apysc-2.8.0/apysc/_translation/jp/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_line_thickness.py` & `apysc-2.8.0/apysc/_translation/jp/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_method_chaining.py` & `apysc-2.8.0/apysc/_translation/jp/animation_method_chaining.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_move.py` & `apysc-2.8.0/apysc/_translation/jp/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_parallel.py` & `apysc-2.8.0/apysc/_translation/jp/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_pause_and_play.py` & `apysc-2.8.0/apysc/_translation/jp/animation_pause_and_play.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_radius.py` & `apysc-2.8.0/apysc/_translation/jp/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_reset.py` & `apysc-2.8.0/apysc/_translation/jp/animation_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_return_value.py` & `apysc-2.8.0/apysc/_translation/jp/animation_return_value.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_reverse.py` & `apysc-2.8.0/apysc/_translation/jp/animation_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_rotation_around_center.py` & `apysc-2.8.0/apysc/_translation/jp/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_rotation_around_point.py` & `apysc-2.8.0/apysc/_translation/jp/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_scale_x_and_y_from_center.py` & `apysc-2.8.0/apysc/_translation/jp/animation_scale_x_and_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_scale_x_and_y_from_point.py` & `apysc-2.8.0/apysc/_translation/jp/animation_scale_x_and_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_time.py` & `apysc-2.8.0/apysc/_translation/jp/animation_time.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_width_and_height.py` & `apysc-2.8.0/apysc/_translation/jp/animation_width_and_height.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_x.py` & `apysc-2.8.0/apysc/_translation/jp/animation_x.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ##################################################
     "The following example sets the x-coordinate animation (from 50 to 100) with the `animation_x` method:": "以下の例では`animation_x`メソッドを使ってX座標（50から100）のアニメーションを設定しています。",  # noqa
     ##################################################
     '```py\n# runnable\nimport apysc as ap\n\nEASING: ap.Easing = ap.Easing.EASE_OUT_QUINT\nDURATION: int = 1000\n\n\ndef on_animation_complete_1(e: ap.AnimationEvent[ap.Rectangle], options: dict) -> None:\n    """\n    The handler that the animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = e.this.target\n    animation_x: ap.AnimationX = rectangle.animation_x(\n        x=50, duration=DURATION, easing=EASING\n    )\n    animation_x.animation_complete(on_animation_complete_2)\n    animation_x.start()\n\n\ndef on_animation_complete_2(e: ap.AnimationEvent[ap.Rectangle], options: dict) -> None:\n    """\n    The handler that the animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = e.this.target\n    animation_x: ap.AnimationX = rectangle.animation_x(\n        x=100, duration=DURATION, easing=EASING\n    )\n    animation_x.animation_complete(on_animation_complete_1)\n    animation_x.start()\n\n\nap.Stage(\n    stage_width=200, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#00aaff")\nrectangle: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\nanimation_x: ap.AnimationX = rectangle.animation_x(\n    x=100, duration=DURATION, easing=EASING\n)\nanimation_x.animation_complete(on_animation_complete_1)\nanimation_x.start()\n\nap.save_overall_html(dest_dir_path="./animation_x_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nEASING: ap.Easing = ap.Easing.EASE_OUT_QUINT\nDURATION: int = 1000\n\n\ndef on_animation_complete_1(e: ap.AnimationEvent[ap.Rectangle], options: dict) -> None:\n    """\n    The handler that the animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = e.this.target\n    animation_x: ap.AnimationX = rectangle.animation_x(\n        x=50, duration=DURATION, easing=EASING\n    )\n    animation_x.animation_complete(on_animation_complete_2)\n    animation_x.start()\n\n\ndef on_animation_complete_2(e: ap.AnimationEvent[ap.Rectangle], options: dict) -> None:\n    """\n    The handler that the animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = e.this.target\n    animation_x: ap.AnimationX = rectangle.animation_x(\n        x=100, duration=DURATION, easing=EASING\n    )\n    animation_x.animation_complete(on_animation_complete_1)\n    animation_x.start()\n\n\nap.Stage(\n    stage_width=200, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#00aaff")\nrectangle: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\nanimation_x: ap.AnimationX = rectangle.animation_x(\n    x=100, duration=DURATION, easing=EASING\n)\nanimation_x.animation_complete(on_animation_complete_1)\nanimation_x.start()\n\nap.save_overall_html(dest_dir_path="./animation_x_basic_usage/")\n```',  # noqa
     ##################################################
     "## Notes for the Circle and Ellipse classes": "## Circle と Ellipse の各クラスの特記事項",
     ##################################################
-    "The `Circle` and `Ellipse` classes' `animation_x` interface will return an `AnimationCx` (center-x) class instance, instead of a `AnimationX` instance, for internal implementation reason.": "内部実装が異なるため`Circle`と`Ellipse`の各クラスの`animation_x`インターフェイスは`AnimationX`の代わりに`AnimationCx`クラス（center-x）のインスタンスを返却します。",  # noqa
+    "The `Circle` and `Ellipse` classes' `animation_x` interface will return an `AnimationCx` (center x) class instance, instead of an `AnimationX` instance, for internal implementation reasons.": "内部実装が異なるため`Circle`と`Ellipse`の各クラスの`animation_x`インターフェイスは`AnimationX`の代わりに`AnimationCx`クラス（center x）のインスタンスを返却します。",  # noqa
     ##################################################
     '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=200, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#00aaff")\ncircle: ap.Circle = sprite.graphics.draw_circle(x=100, y=100, radius=50)\nanimation_cx: ap.AnimationCx = circle.animation_x(\n    x=100, duration=1000, easing=ap.Easing.EASE_OUT_QUINT\n)\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=200, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#00aaff")\ncircle: ap.Circle = sprite.graphics.draw_circle(x=100, y=100, radius=50)\nanimation_cx: ap.AnimationCx = circle.animation_x(\n    x=100, duration=1000, easing=ap.Easing.EASE_OUT_QUINT\n)\n```',  # noqa
     ##################################################
     "## animation_x API": "## animation_x API",
     ##################################################
     '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
```

### Comparing `apysc-2.7.9/apysc/_translation/jp/animation_y.py` & `apysc-2.8.0/apysc/_translation/jp/animation_y.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ##################################################
     "The following example sets the y-coordinate animation (from 50 to 100) with the `animation_y` method.": "以下のコード例では`animation_y`メソッドを使ってY座標（50から100）のアニメーションを設定しています。",  # noqa
     ##################################################
     '```py\n# runnable\nimport apysc as ap\n\nEASING: ap.Easing = ap.Easing.EASE_OUT_QUINT\nDURATION: int = 1000\n\n\ndef on_animation_complete_1(e: ap.AnimationEvent[ap.Rectangle], options: dict) -> None:\n    """\n    The handler that the animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = e.this.target\n    animation_y: ap.AnimationY = rectangle.animation_y(\n        y=50, duration=DURATION, easing=EASING\n    )\n    animation_y.animation_complete(on_animation_complete_2)\n    animation_y.start()\n\n\ndef on_animation_complete_2(e: ap.AnimationEvent[ap.Rectangle], options: dict) -> None:\n    """\n    The handler that the animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = e.this.target\n    animation_y: ap.AnimationY = rectangle.animation_y(\n        y=100, duration=DURATION, easing=EASING\n    )\n    animation_y.animation_complete(on_animation_complete_1)\n    animation_y.start()\n\n\nap.Stage(\n    stage_width=150, stage_height=200, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#00aaff")\nrectangle: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\nanimation_y: ap.AnimationY = rectangle.animation_y(\n    y=100, duration=DURATION, easing=EASING\n)\nanimation_y.animation_complete(on_animation_complete_1)\nanimation_y.start()\n\nap.save_overall_html(dest_dir_path="./animation_y_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nEASING: ap.Easing = ap.Easing.EASE_OUT_QUINT\nDURATION: int = 1000\n\n\ndef on_animation_complete_1(e: ap.AnimationEvent[ap.Rectangle], options: dict) -> None:\n    """\n    The handler that the animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = e.this.target\n    animation_y: ap.AnimationY = rectangle.animation_y(\n        y=50, duration=DURATION, easing=EASING\n    )\n    animation_y.animation_complete(on_animation_complete_2)\n    animation_y.start()\n\n\ndef on_animation_complete_2(e: ap.AnimationEvent[ap.Rectangle], options: dict) -> None:\n    """\n    The handler that the animation calls when its end.\n\n    Parameters\n    ----------\n    e : ap.AnimationEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = e.this.target\n    animation_y: ap.AnimationY = rectangle.animation_y(\n        y=100, duration=DURATION, easing=EASING\n    )\n    animation_y.animation_complete(on_animation_complete_1)\n    animation_y.start()\n\n\nap.Stage(\n    stage_width=150, stage_height=200, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#00aaff")\nrectangle: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\nanimation_y: ap.AnimationY = rectangle.animation_y(\n    y=100, duration=DURATION, easing=EASING\n)\nanimation_y.animation_complete(on_animation_complete_1)\nanimation_y.start()\n\nap.save_overall_html(dest_dir_path="./animation_y_basic_usage/")\n```',  # noqa
     ##################################################
     "## Notes for the Circle and Ellipse classes": "## Circle と Ellipse の各クラスの特記事項",
     ##################################################
-    "The `Circle` and `Ellipse` classes' `animation_y` interface will return an `AnimationCy` (center-y) class instance, instead of a `AnimationY` instance, for internal implementation reason.": "内部の実装が異なる都合で`Circle`と`Ellipse`の各クラスの`animation_y`のインターフェイスは`AnimationY`クラスの代わりに`AnimationCy`クラスのインスタンスを返却します。",  # noqa
+    "The `Circle` and `Ellipse` classes' `animation_y` interface will return an `AnimationCy` (center y) class instance, instead of a `AnimationY` instance, for internal implementation reason.": "内部の実装が異なる都合で`Circle`と`Ellipse`の各クラスの`animation_y`のインターフェイスは`AnimationY`クラスの代わりに`AnimationCy`クラスのインスタンスを返却します。",  # noqa
     ##################################################
     '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=200, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#00aaff")\ncircle: ap.Circle = sprite.graphics.draw_circle(x=100, y=100, radius=50)\nanimation_cy: ap.AnimationCy = circle.animation_y(\n    y=100, duration=1000, easing=ap.Easing.EASE_OUT_QUINT\n)\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    stage_width=200, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#00aaff")\ncircle: ap.Circle = sprite.graphics.draw_circle(x=100, y=100, radius=50)\nanimation_cy: ap.AnimationCy = circle.animation_y(\n    y=100, duration=1000, easing=ap.Easing.EASE_OUT_QUINT\n)\n```',  # noqa
     ##################################################
     "## animation_y API": "## animation_y API",
     ##################################################
     '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
```

### Comparing `apysc-2.7.9/apysc/_translation/jp/append_js_expression.py` & `apysc-2.8.0/apysc/_translation/jp/append_js_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array.py` & `apysc-2.8.0/apysc/_translation/jp/array.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_append_and_push.py` & `apysc-2.8.0/apysc/_translation/jp/array_append_and_push.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_clear.py` & `apysc-2.8.0/apysc/_translation/jp/array_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_comparison.py` & `apysc-2.8.0/apysc/_translation/jp/array_comparison.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_extend_and_concat.py` & `apysc-2.8.0/apysc/_translation/jp/array_extend_and_concat.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_index_of.py` & `apysc-2.8.0/apysc/_translation/jp/array_index_of.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_insert_and_insert_at.py` & `apysc-2.8.0/apysc/_translation/jp/array_insert_and_insert_at.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_join.py` & `apysc-2.8.0/apysc/_translation/jp/array_join.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_length.py` & `apysc-2.8.0/apysc/_translation/jp/array_length.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_pop.py` & `apysc-2.8.0/apysc/_translation/jp/array_pop.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_remove_and_remove_at.py` & `apysc-2.8.0/apysc/_translation/jp/array_remove_and_remove_at.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_reverse.py` & `apysc-2.8.0/apysc/_translation/jp/array_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_slice.py` & `apysc-2.8.0/apysc/_translation/jp/array_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/array_sort.py` & `apysc-2.8.0/apysc/_translation/jp/array_sort.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py` & `apysc-2.8.0/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/assert_defined_and_undefined.py` & `apysc-2.8.0/apysc/_translation/jp/assert_defined_and_undefined.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py` & `apysc-2.8.0/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/assert_equal_and_not_equal.py` & `apysc-2.8.0/apysc/_translation/jp/assert_equal_and_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/assert_greater_and_greater_equal.py` & `apysc-2.8.0/apysc/_translation/jp/assert_greater_and_greater_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/assert_less_and_less_equal.py` & `apysc-2.8.0/apysc/_translation/jp/assert_less_and_less_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/assert_true_and_false.py` & `apysc-2.8.0/apysc/_translation/jp/assert_true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/assertion_basic_behavior.py` & `apysc-2.8.0/apysc/_translation/jp/assertion_basic_behavior.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/bind_and_trigger_custom_event.py` & `apysc-2.8.0/apysc/_translation/jp/bind_and_trigger_custom_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/boolean.py` & `apysc-2.8.0/apysc/_translation/jp/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py` & `apysc-2.8.0/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/circle.py` & `apysc-2.8.0/apysc/_translation/jp/circle.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ##################################################
     "## What class is this?": "## クラス概要",
     ##################################################
     "The `Circle` class creates a circle vector graphics object.": "`Circle`クラスは円のベクターグラフィックスを生成します。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
-    "The `Circle` class constructor requires the `x` (center-x), `y` (center-y), and `radius` arguments.": "`Circle`クラスのコンストラクタでは`x`（円の中央のX座標）、`y`（円の中央のY座標）、そして半径としての`radius`引数が必要となります。",  # noqa
+    "The `Circle` class constructor requires the `x` (center x), `y` (center y), and `radius` arguments.": "`Circle`クラスのコンストラクタでは`x`（円の中央のX座標）、`y`（円の中央のY座標）、そして半径としての`radius`引数が必要となります。",  # noqa
     ##################################################
     "The constructor also accepts each style's argument, such as the `fill_color`.": "コンストラクタでは他の`fill_color`などのスタイル設定の各引数も受け付けます。",  # noqa
     ##################################################
     '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=150, stage_height=150, stage_elem_id="stage"\n)\ncircle: ap.Circle = ap.Circle(x=75, y=75, radius=50, fill_color="#0af")\n\nap.save_overall_html(dest_dir_path="circle_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=150, stage_height=150, stage_elem_id="stage"\n)\ncircle: ap.Circle = ap.Circle(x=75, y=75, radius=50, fill_color="#0af")\n\nap.save_overall_html(dest_dir_path="circle_basic_usage/")\n```',  # noqa
     ##################################################
     "## Note of the draw_circle interface": "## draw_circle インターフェイスに対する特記事項",
     ##################################################
```

### Comparing `apysc-2.7.9/apysc/_translation/jp/click.py` & `apysc-2.8.0/apysc/_translation/jp/click.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/contains.py` & `apysc-2.8.0/apysc/_translation/jp/contains.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/continue.py` & `apysc-2.8.0/apysc/_translation/jp/continue.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime.py` & `apysc-2.8.0/apysc/_translation/jp/datetime.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_day.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_day.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_hour.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_hour.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_millisecond.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_millisecond.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_minute.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_minute.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_month.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_month.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_now.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_now.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_second.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_second.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_set_month_end.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_set_month_end.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/datetime_year.py` & `apysc-2.8.0/apysc/_translation/jp/datetime_year.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/dblclick.py` & `apysc-2.8.0/apysc/_translation/jp/dblclick.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/delete.py` & `apysc-2.8.0/apysc/_translation/jp/delete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/dictionary.py` & `apysc-2.8.0/apysc/_translation/jp/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/dictionary_generic.py` & `apysc-2.8.0/apysc/_translation/jp/dictionary_generic.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/dictionary_get.py` & `apysc-2.8.0/apysc/_translation/jp/dictionary_get.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/dictionary_length.py` & `apysc-2.8.0/apysc/_translation/jp/dictionary_length.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/display_object.py` & `apysc-2.8.0/apysc/_translation/jp/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py` & `apysc-2.8.0/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/display_object_get_and_set_css.py` & `apysc-2.8.0/apysc/_translation/jp/display_object_get_and_set_css.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/display_object_mouse_event.py` & `apysc-2.8.0/apysc/_translation/jp/display_object_mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/display_object_parent.py` & `apysc-2.8.0/apysc/_translation/jp/display_object_parent.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/display_object_visible.py` & `apysc-2.8.0/apysc/_translation/jp/display_object_visible.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/display_object_x_and_y.py` & `apysc-2.8.0/apysc/_translation/jp/display_object_x_and_y.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/display_on_colaboratory.py` & `apysc-2.8.0/apysc/_translation/jp/display_on_colaboratory.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/display_on_jupyter.py` & `apysc-2.8.0/apysc/_translation/jp/display_on_jupyter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/draw_interfaces_abstract.py` & `apysc-2.8.0/apysc/_translation/jp/draw_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/easing_enum.py` & `apysc-2.8.0/apysc/_translation/jp/easing_enum.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/elif.py` & `apysc-2.8.0/apysc/_translation/jp/elif.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/ellipse.py` & `apysc-2.8.0/apysc/_translation/jp/ellipse.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ##################################################
     "## What class is this?": "## クラス概要",
     ##################################################
     "The `Ellipse` class creates an ellipse vector graphics object.": "`Ellipse`クラスは楕円のベクターグラフィックスのオブジェクトを生成します。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
-    "The `Ellipse` class constructor requires the `x` (center-x), `y` (center-y), `width`, and `height` arguments.": "`Ellipse`クラスのコンストラクタでは`x`（楕円の中央のX座標）、`y`（楕円の中央のY座標）、`width`、`height`の各引数の指定が必要です。",  # noqa
+    "The `Ellipse` class constructor requires the `x` (center x), `y` (center y), `width`, and `height` arguments.": "`Ellipse`クラスのコンストラクタでは`x`（楕円の中央のX座標）、`y`（楕円の中央のY座標）、`width`、`height`の各引数の指定が必要です。",  # noqa
     ##################################################
     "The constructor also accepts each style's argument, such as the `fill_color`.": "コンストラクタでは他の`fill_color`などのスタイル設定の各引数も受け付けます。",  # noqa
     ##################################################
     '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=150, stage_height=150, stage_elem_id="stage"\n)\nellipse: ap.Ellipse = ap.Ellipse(x=75, y=75, width=100, height=75, fill_color="#0af")\n\nap.save_overall_html(dest_dir_path="ellipse_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=150, stage_height=150, stage_elem_id="stage"\n)\nellipse: ap.Ellipse = ap.Ellipse(x=75, y=75, width=100, height=75, fill_color="#0af")\n\nap.save_overall_html(dest_dir_path="ellipse_basic_usage/")\n```',  # noqa
     ##################################################
     "## Note of the draw_ellipse interface": "## draw_ellipse インターフェイスについての特記事項",
     ##################################################
```

### Comparing `apysc-2.7.9/apysc/_translation/jp/else.py` & `apysc-2.8.0/apysc/_translation/jp/else.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/enter_frame.py` & `apysc-2.8.0/apysc/_translation/jp/enter_frame.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py` & `apysc-2.8.0/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/for.py` & `apysc-2.8.0/apysc/_translation/jp/for.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/fps.py` & `apysc-2.8.0/apysc/_translation/jp/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/fundamental_data_classes_value_interface.py` & `apysc-2.8.0/apysc/_translation/jp/fundamental_data_classes_value_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/get_child_at.py` & `apysc-2.8.0/apysc/_translation/jp/get_child_at.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics.py` & `apysc-2.8.0/apysc/_translation/jp/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_fill_alpha.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_fill_color.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_flip_interfaces.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_flip_interfaces.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_line_alpha.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_line_color.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_line_dash_setting.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_line_dot_setting.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_line_round_dot_setting.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_line_thickness.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_rotation_around_center.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_rotation_around_point.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_scale_from_center.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_scale_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_scale_from_point.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_scale_from_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ##################################################
     "Return value is set for each coordinate. For example, if you set the scale-x value at the 50px x-coordinate, 100px x-coordinate scale will not be affected.": "返却値は各座標ごとに設定されます。例えば水平方向の拡縮を50pxのX座標の位置で設定した場合、100pxのX座標の位置における拡縮値には影響しません。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
     "The `get_scale_x_from_point` method requires the `x` argument (`Int` value), and the `set_scale_x_from_point` requires the `scale_x` (`Number` value) and `x` arguments.": "`get_scale_x_from_point`メソッドは`Int`型の`x`引数の指定を必要とし、`set_scale_x_from_point`メソッドは`Number`型の`scale_x`と`x`の各引く数の指定が必要になります。",  # noqa
     ##################################################
-    "The following example creates three rectangles and increments (or decrements) for each rectangle scale-x value. The top rectangle scales from the left-x position. The middle one scales from the center-x. And the bottom one scales from the right-x.": "以下のコード例では3つの四角を生成し水平方向の拡縮を増減させています。上の四角は左端を基準に拡縮を、真ん中の四角は中央を基準に拡縮を、そして下の四角では右右端を基準に拡縮を行っています。",  # noqa
+    "The following example creates three rectangles and increments (or decrements) for each rectangle scale-x value. The top rectangle scales from the left x position. The middle one scales from the center x. And the bottom one scales from the right x.": "以下のコード例では3つの四角を生成し水平方向の拡縮を増減させています。上の四角は左端を基準に拡縮を、真ん中の四角は中央を基準に拡縮を、そして下の四角では右右端を基準に拡縮を行っています。",  # noqa
     ##################################################
     '```py\n# runnable\nfrom typing_extensions import TypedDict\n\nimport apysc as ap\n\n\nclass _Options(TypedDict):\n    rectangle: ap.Rectangle\n    x: ap.Int\n    direction: ap.Int\n\n\ndef on_timer(e: ap.TimerEvent, options: _Options) -> None:\n    """\n    The handler that the timer calls.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = options["rectangle"]\n    x: ap.Int = options["x"]\n    direction: ap.Int = options["direction"]\n    current_scale_x: ap.Number = rectangle.get_scale_x_from_point(x=x)\n    current_scale_x += direction * 0.03\n    rectangle.set_scale_x_from_point(scale_x=current_scale_x, x=x)\n    with ap.If(current_scale_x >= 2.0):\n        direction *= -1\n    with ap.If(current_scale_x <= 0.0):\n        direction *= -1\n\n\nap.Stage(\n    stage_width=150, stage_height=350, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\n\ntop_rect: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\nmiddle_rect: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=150, width=50, height=50)\nbottom_rect: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=250, width=50, height=50)\n\ntop_rect_direction: ap.Int = ap.Int(1)\noptions: _Options = {\n    "rectangle": top_rect,\n    "x": ap.Int(50),\n    "direction": top_rect_direction,\n}\ntop_rect_timer: ap.Timer = ap.Timer(on_timer, delay=ap.FPS.FPS_60, options=options)\ntop_rect_timer.start()\n\nmiddle_rect_direction: ap.Int = ap.Int(1)\noptions = {\n    "rectangle": middle_rect,\n    "x": ap.Int(75),\n    "direction": middle_rect_direction,\n}\nmiddle_rect_timer: ap.Timer = ap.Timer(on_timer, delay=ap.FPS.FPS_60, options=options)\nmiddle_rect_timer.start()\n\nbottom_rect_direction: ap.Int = ap.Int(1)\noptions = {\n    "rectangle": bottom_rect,\n    "x": ap.Int(100),\n    "direction": bottom_rect_direction,\n}\nbottom_rect_timer: ap.Timer = ap.Timer(on_timer, delay=ap.FPS.FPS_60, options=options)\nbottom_rect_timer.start()\n\nap.save_overall_html(dest_dir_path="graphics_base_scale_from_point_basic_usage_x/")\n```': '```py\n# runnable\nfrom typing_extensions import TypedDict\n\nimport apysc as ap\n\n\nclass _Options(TypedDict):\n    rectangle: ap.Rectangle\n    x: ap.Int\n    direction: ap.Int\n\n\ndef on_timer(e: ap.TimerEvent, options: _Options) -> None:\n    """\n    The handler that the timer calls.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = options["rectangle"]\n    x: ap.Int = options["x"]\n    direction: ap.Int = options["direction"]\n    current_scale_x: ap.Number = rectangle.get_scale_x_from_point(x=x)\n    current_scale_x += direction * 0.03\n    rectangle.set_scale_x_from_point(scale_x=current_scale_x, x=x)\n    with ap.If(current_scale_x >= 2.0):\n        direction *= -1\n    with ap.If(current_scale_x <= 0.0):\n        direction *= -1\n\n\nap.Stage(\n    stage_width=150, stage_height=350, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\n\ntop_rect: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\nmiddle_rect: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=150, width=50, height=50)\nbottom_rect: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=250, width=50, height=50)\n\ntop_rect_direction: ap.Int = ap.Int(1)\noptions: _Options = {\n    "rectangle": top_rect,\n    "x": ap.Int(50),\n    "direction": top_rect_direction,\n}\ntop_rect_timer: ap.Timer = ap.Timer(on_timer, delay=ap.FPS.FPS_60, options=options)\ntop_rect_timer.start()\n\nmiddle_rect_direction: ap.Int = ap.Int(1)\noptions = {\n    "rectangle": middle_rect,\n    "x": ap.Int(75),\n    "direction": middle_rect_direction,\n}\nmiddle_rect_timer: ap.Timer = ap.Timer(on_timer, delay=ap.FPS.FPS_60, options=options)\nmiddle_rect_timer.start()\n\nbottom_rect_direction: ap.Int = ap.Int(1)\noptions = {\n    "rectangle": bottom_rect,\n    "x": ap.Int(100),\n    "direction": bottom_rect_direction,\n}\nbottom_rect_timer: ap.Timer = ap.Timer(on_timer, delay=ap.FPS.FPS_60, options=options)\nbottom_rect_timer.start()\n\nap.save_overall_html(dest_dir_path="graphics_base_scale_from_point_basic_usage_x/")\n```',  # noqa
     ##################################################
     "The `get_scale_y_from_point` and `set_scale_y_from_point` methods have the similar arguments, `scale_y` and `y`. These interfaces work the same way as the x-axis interfaces, except that the axis directions are different.": "似たような形で`get_scale_y_from_point`と`set_scale_y_from_point`のメソッドは`scale_y`と`y`の引数を必要とします。これらは拡縮の方向が垂直方向になっている以外は水平方向のインターフェイスと同じように動作します。",  # noqa
     ##################################################
     '```py\n# runnable\nfrom typing_extensions import TypedDict\n\nimport apysc as ap\n\n\nclass _Options(TypedDict):\n    rectangle: ap.Rectangle\n    y: ap.Int\n    direction: ap.Int\n\n\ndef on_timer(e: ap.TimerEvent, options: _Options) -> None:\n    """\n    The handler that the timer calls.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = options["rectangle"]\n    y: ap.Int = options["y"]\n    direction: ap.Int = options["direction"]\n    current_scale_y: ap.Number = rectangle.get_scale_y_from_point(y=y)\n    current_scale_y += direction * 0.03\n    rectangle.set_scale_y_from_point(scale_y=current_scale_y, y=y)\n    with ap.If(current_scale_y >= 2.0):\n        direction *= -1\n    with ap.If(current_scale_y <= 0.0):\n        direction *= -1\n\n\nap.Stage(\n    stage_width=150, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\n\nrectangle: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\ndirection: ap.Int = ap.Int(1)\noptions: _Options = {"rectangle": rectangle, "y": ap.Int(50), "direction": direction}\ntimer: ap.Timer = ap.Timer(on_timer, delay=ap.FPS.FPS_60, options=options)\ntimer.start()\n\nap.save_overall_html(dest_dir_path="graphics_base_scale_from_point_basic_usage_y/")\n```': '```py\n# runnable\nfrom typing_extensions import TypedDict\n\nimport apysc as ap\n\n\nclass _Options(TypedDict):\n    rectangle: ap.Rectangle\n    y: ap.Int\n    direction: ap.Int\n\n\ndef on_timer(e: ap.TimerEvent, options: _Options) -> None:\n    """\n    The handler that the timer calls.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional arguments dictionary.\n    """\n    rectangle: ap.Rectangle = options["rectangle"]\n    y: ap.Int = options["y"]\n    direction: ap.Int = options["direction"]\n    current_scale_y: ap.Number = rectangle.get_scale_y_from_point(y=y)\n    current_scale_y += direction * 0.03\n    rectangle.set_scale_y_from_point(scale_y=current_scale_y, y=y)\n    with ap.If(current_scale_y >= 2.0):\n        direction *= -1\n    with ap.If(current_scale_y <= 0.0):\n        direction *= -1\n\n\nap.Stage(\n    stage_width=150, stage_height=150, background_color="#333", stage_elem_id="stage"\n)\nsprite: ap.Sprite = ap.Sprite()\nsprite.graphics.begin_fill(color="#0af")\n\nrectangle: ap.Rectangle = sprite.graphics.draw_rect(x=50, y=50, width=50, height=50)\ndirection: ap.Int = ap.Int(1)\noptions: _Options = {"rectangle": rectangle, "y": ap.Int(50), "direction": direction}\ntimer: ap.Timer = ap.Timer(on_timer, delay=ap.FPS.FPS_60, options=options)\ntimer.start()\n\nap.save_overall_html(dest_dir_path="graphics_base_scale_from_point_basic_usage_y/")\n```',  # noqa
     ##################################################
```

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_base_skew.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_base_skew.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_begin_fill.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_begin_fill.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_clear.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_circle.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_circle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_dash_dotted_line.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_dash_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_dashed_line.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_dashed_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_dotted_line.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_ellipse.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_line.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_path.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_path.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_polygon.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_rect.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_round_dotted_line.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_round_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_round_rect.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_round_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_draw_triangle.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_draw_triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_line_style.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_line_style.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/graphics_move_to_and_line_to.py` & `apysc-2.8.0/apysc/_translation/jp/graphics_move_to_and_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/if.py` & `apysc-2.8.0/apysc/_translation/jp/if.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/import_conventions.py` & `apysc-2.8.0/apysc/_translation/jp/import_conventions.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/index.py` & `apysc-2.8.0/apysc/_translation/jp/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,19 @@
     ##################################################
     "The parent class, such as the `Sprite` or `Stage`, has the following interfaces:": "`Sprite`や`Stage`などの親となれる各クラスは以下のインターフェイスを持っています:",  # noqa
     ##################################################
     "```{toctree}\n:maxdepth: 1\nadd_child_and_remove_child\nremove_children\ncontains\nnum_children\nget_child_at\n```": "```{toctree}\n:maxdepth: 1\njp_add_child_and_remove_child\njp_remove_children\njp_contains\njp_num_children\njp_get_child_at\n```",  # noqa
     ##################################################
     "## apysc basic data classes": "## apyscの基本的な各データクラス",
     ##################################################
-    "```{toctree}\n:maxdepth: 1\nwhy_apysc_doesnt_use_python_builtin_data_type\nfundamental_data_classes_value_interface\n```": "```{toctree}\n:maxdepth: 1\njp_why_apysc_doesnt_use_python_builtin_data_type\njp_fundamental_data_classes_value_interface\n```",  # noqa
+    "```{toctree}\n:maxdepth: 1\nwhy_apysc_doesnt_use_python_builtin_data_type\nfundamental_data_classes_value_interface\nto_string\n```": "```{toctree}\n:maxdepth: 1\njp_why_apysc_doesnt_use_python_builtin_data_type\njp_fundamental_data_classes_value_interface\njp_to_string\n```",  # noqa
     ##################################################
     "### Int and Number classes": "### Int と Number クラス",
     ##################################################
-    "```{toctree}\n:maxdepth: 1\nint_and_number\nint_and_number_arithmetic_operations\nint_and_number_comparison_operations\n```": "```{toctree}\n:maxdepth: 1\njp_int_and_number\njp_int_and_number_arithmetic_operations\njp_int_and_number_comparison_operations\n```",  # noqa
+    "```{toctree}\n:maxdepth: 1\nint_and_number\nint_and_number_arithmetic_operations\nint_and_number_comparison_operations\nint_and_number_to_fixed\n```": "```{toctree}\n:maxdepth: 1\njp_int_and_number\njp_int_and_number_arithmetic_operations\njp_int_and_number_comparison_operations\njp_int_and_number_to_fixed\n```",  # noqa
     ##################################################
     "### String class": "### String クラス",
     ##################################################
     "```{toctree}\n:maxdepth: 1\nstring\nstring_comparison_operations\nstring_addition_and_multiplication\nstring_split\n```": "```{toctree}\n:maxdepth: 1\njp_string\njp_string_comparison_operations\njp_string_addition_and_multiplication\njp_string_split\n```",  # noqa
     ##################################################
     "### Boolean class": "### Boolean クラス",
     ##################################################
@@ -87,15 +87,15 @@
     ##################################################
     "## SVG text": "## SVG テキスト",
     ##################################################
     "```{toctree}\n:maxdepth: 1\nsvg_text\nsvg_text_span\n```": "```{toctree}\n:maxdepth: 1\njp_svg_text\njp_svg_text_span\n```",  # noqa
     ##################################################
     "## Geometry-related classes": "## 座標・サイズ等のデータの各クラス",
     ##################################################
-    "```{toctree}\n:maxdepth: 1\npoint2d\npath_move_to\npath_line_to\npath_horizontal\npath_vertical\npath_close\npath_bezier_2d\npath_bezier_2d_continual\npath_bezier_3d\npath_bezier_3d_continual\n```": "```{toctree}\n:maxdepth: 1\njp_point2d\njp_path_move_to\njp_path_line_to\njp_path_horizontal\njp_path_vertical\njp_path_close\njp_path_bezier_2d\njp_path_bezier_2d_continual\njp_path_bezier_3d\njp_path_bezier_3d_continual\n```",  # noqa
+    "```{toctree}\n:maxdepth: 1\npoint2d\npath_move_to\npath_line_to\npath_horizontal\npath_vertical\npath_close\npath_bezier_2d\npath_bezier_2d_continual\npath_bezier_3d\npath_bezier_3d_continual\nrectangle_geom\nget_bounds\n```": "```{toctree}\n:maxdepth: 1\njp_point2d\njp_path_move_to\njp_path_line_to\njp_path_horizontal\njp_path_vertical\njp_path_close\njp_path_bezier_2d\njp_path_bezier_2d_continual\njp_path_bezier_3d\njp_path_bezier_3d_continual\njp_rectangle_geom\njp_get_bounds\n```",  # noqa
     ##################################################
     "## Common event interfaces": "## イベントの共通の各インターフェイス",
     ##################################################
     "```{toctree}\n:maxdepth: 1\nabout_handler_options_type\nevent_prevent_default_and_stop_propagation\nbind_and_trigger_custom_event\n```": "```{toctree}\n:maxdepth: 1\njp_about_handler_options_type\njp_event_prevent_default_and_stop_propagation\njp_bind_and_trigger_custom_event\n```",  # noqa
     ##################################################
     "## MouseEvent class and mouse event binding": "## MouseEvent クラスとマウスイベントの設定",
     ##################################################
@@ -103,15 +103,15 @@
     ##################################################
     "## Branch instruction": "## 条件分岐の制御",
     ##################################################
     "```{toctree}\n:maxdepth: 1\nif\nelif\nelse\nbranch_instruction_variables_reverting_setting\nreturn\n```": "```{toctree}\n:maxdepth: 1\njp_if\njp_elif\njp_else\njp_branch_instruction_variables_reverting_setting\njp_return\n```",  # noqa
     ##################################################
     "## Loop": "## ループ",
     ##################################################
-    "```{toctree}\n:maxdepth: 1\nfor\ncontinue\n```": "```{toctree}\n:maxdepth: 1\njp_for\njp_continue\n```",  # noqa
+    "```{toctree}\n:maxdepth: 1\nfor\ncontinue\nrange\n```": "```{toctree}\n:maxdepth: 1\njp_for\njp_continue\njp_range\n```",  # noqa
     ##################################################
     "## Timer and enter frame": "## タイマーとenter frame",
     ##################################################
     "```{toctree}\n:maxdepth: 1\ntimer\ntimer_event\ntimer_delay\nfps\ntimer_repeat_count\ntimer_start_and_stop\ntimer_complete\ntimer_reset\nenter_frame\nunbind_enter_frame_and_unbind_enter_frame_all\n```": "```{toctree}\n:maxdepth: 1\njp_timer\njp_timer_event\njp_timer_delay\njp_fps\njp_timer_repeat_count\njp_timer_start_and_stop\njp_timer_complete\njp_timer_reset\njp_enter_frame\njp_unbind_enter_frame_and_unbind_enter_frame_all\n```",  # noqa
     ##################################################
     "## DateTime class": "## DateTime クラス",
     ##################################################
```

### Comparing `apysc-2.7.9/apysc/_translation/jp/int_and_number.py` & `apysc-2.8.0/apysc/_translation/jp/int_and_number.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/int_and_number_arithmetic_operations.py` & `apysc-2.8.0/apysc/_translation/jp/int_and_number_arithmetic_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/int_and_number_comparison_operations.py` & `apysc-2.8.0/apysc/_translation/jp/int_and_number_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/line.py` & `apysc-2.8.0/apysc/_translation/jp/line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/math_max.py` & `apysc-2.8.0/apysc/_translation/jp/math_max.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/math_min.py` & `apysc-2.8.0/apysc/_translation/jp/math_min.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/math_trunc.py` & `apysc-2.8.0/apysc/_translation/jp/math_trunc.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/mouse_event_abstract.py` & `apysc-2.8.0/apysc/_translation/jp/mouse_event_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/mouse_event_basic.py` & `apysc-2.8.0/apysc/_translation/jp/mouse_event_basic.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/mousedown_and_mouseup.py` & `apysc-2.8.0/apysc/_translation/jp/mousedown_and_mouseup.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/mousemove.py` & `apysc-2.8.0/apysc/_translation/jp/mousemove.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/mouseover_and_mouseout.py` & `apysc-2.8.0/apysc/_translation/jp/mouseover_and_mouseout.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/num_children.py` & `apysc-2.8.0/apysc/_translation/jp/num_children.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path.py` & `apysc-2.8.0/apysc/_translation/jp/path.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path_bezier_2d.py` & `apysc-2.8.0/apysc/_translation/jp/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path_bezier_2d_continual.py` & `apysc-2.8.0/apysc/_translation/jp/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path_bezier_3d.py` & `apysc-2.8.0/apysc/_translation/jp/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path_bezier_3d_continual.py` & `apysc-2.8.0/apysc/_translation/jp/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path_close.py` & `apysc-2.8.0/apysc/_translation/jp/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path_horizontal.py` & `apysc-2.8.0/apysc/_translation/jp/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path_line_to.py` & `apysc-2.8.0/apysc/_translation/jp/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path_move_to.py` & `apysc-2.8.0/apysc/_translation/jp/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/path_vertical.py` & `apysc-2.8.0/apysc/_translation/jp/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/point2d.py` & `apysc-2.8.0/apysc/_translation/jp/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/polygon.py` & `apysc-2.8.0/apysc/_translation/jp/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/polyline.py` & `apysc-2.8.0/apysc/_translation/jp/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/quick_start.py` & `apysc-2.8.0/apysc/_translation/jp/quick_start.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/recommended_type_checker_settings.py` & `apysc-2.8.0/apysc/_translation/jp/recommended_type_checker_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/rectangle.py` & `apysc-2.8.0/apysc/_translation/jp/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/remove_children.py` & `apysc-2.8.0/apysc/_translation/jp/remove_children.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/return.py` & `apysc-2.8.0/apysc/_translation/jp/return.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/save_overall_html.py` & `apysc-2.8.0/apysc/_translation/jp/save_overall_html.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/sequential_animation.py` & `apysc-2.8.0/apysc/_translation/jp/sequential_animation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/set_debug_mode.py` & `apysc-2.8.0/apysc/_translation/jp/set_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/sprite.py` & `apysc-2.8.0/apysc/_translation/jp/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/stage.py` & `apysc-2.8.0/apysc/_translation/jp/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/string.py` & `apysc-2.8.0/apysc/_translation/jp/string.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/string_addition_and_multiplication.py` & `apysc-2.8.0/apysc/_translation/jp/string_addition_and_multiplication.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/string_comparison_operations.py` & `apysc-2.8.0/apysc/_translation/jp/string_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/string_split.py` & `apysc-2.8.0/apysc/_translation/jp/string_split.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/svg_text.py` & `apysc-2.8.0/apysc/_translation/jp/svg_text.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,169 +17,169 @@
     ##################################################
     "The `SVGText` class creates an SVG text object.": "`SVGText`クラスはSVGテキストのオブジェクトを生成します。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
     "The `SVGText` class constructor requires the `text` argument.": "`SVGText`クラスのコンストラクタは`text`引数の指定を必要とします。",  # noqa
     ##################################################
-    "The constructor also accepts each font\'s and style\'s argument, such as the `font_size`, `font_family`, `fill_color`, and `bold`.": "コンストラクタでは`font_size`や`font_family`、`fill_color`、`bold`などのフォントやスタイルなどの引数を指定することもできます。",  # noqa
+    "The constructor also accepts each font's and style's argument, such as the `font_size`, `font_family`, `fill_color`, and `bold`.": "コンストラクタでは`font_size`や`font_family`、`fill_color`、`bold`などのフォントやスタイルなどの引数を指定することもできます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nap.save_overall_html(dest_dir_path=\"svg_text_basic_usage/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nap.save_overall_html(dest_dir_path=\"svg_text_basic_usage/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nap.save_overall_html(dest_dir_path="svg_text_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nap.save_overall_html(dest_dir_path="svg_text_basic_usage/")\n```',  # noqa
     ##################################################
-    "## Note on the baseline of a text\'s y-coordinate": "## テキストのY座標の基準点に対する特記事項",
+    "## Note on the baseline of a text's y-coordinate": "## テキストのY座標の基準点に対する特記事項",
     ##################################################
-    "The baseline of a text\'s y-coordinate is the text\'s bottom position (this is the specification of the SVG text).": "テキストのY座標の基準点はテキストの下部付近の位置となります（これはSVGテキストの仕様となります）。",  # noqa
+    "The baseline of a text's y-coordinate is the text's bottom position (this is the specification of the SVG text).": "テキストのY座標の基準点はテキストの下部付近の位置となります（これはSVGテキストの仕様となります）。",  # noqa
     ##################################################
-    "So if you specify `y=0` as the coordinate, you can see almost nothing of a text\'s content (barely see the bottom of the comma in the following example).": "そのためもしもY座標に`y=0`を指定した場合、テキストのコンテンツがほとんど見えなくなります（以下の例では辛うじてコンマの一部が確認できます）。",  # noqa
+    "So if you specify `y=0` as the coordinate, you can see almost nothing of a text's content (barely see the bottom of the comma in the following example).": "そのためもしもY座標に`y=0`を指定した場合、テキストのコンテンツがほとんど見えなくなります（以下の例では辛うじてコンマの一部が確認できます）。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=0,\n    fill_color=\"#aaa\",\n)\nap.save_overall_html(dest_dir_path=\"svg_text_note_on_the_y_baseline/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=0,\n    fill_color=\"#aaa\",\n)\nap.save_overall_html(dest_dir_path=\"svg_text_note_on_the_y_baseline/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=0,\n    fill_color="#aaa",\n)\nap.save_overall_html(dest_dir_path="svg_text_note_on_the_y_baseline/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=0,\n    fill_color="#aaa",\n)\nap.save_overall_html(dest_dir_path="svg_text_note_on_the_y_baseline/")\n```',  # noqa
     ##################################################
     "## text property interface example": "## text 属性のインターフェイス例",
     ##################################################
-    "The `text` property updates or gets the instance\'s text.": "`text`属性ではインスタンスのテキストの更新もしくは取得を行えます。",  # noqa
+    "The `text` property updates or gets the instance's text.": "`text`属性ではインスタンスのテキストの更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.text = ap.String(\"Lorem ipsum\")\nap.save_overall_html(dest_dir_path=\"svg_text_text/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.text = ap.String(\"Lorem ipsum\")\nap.save_overall_html(dest_dir_path=\"svg_text_text/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.text = ap.String("Lorem ipsum")\nap.save_overall_html(dest_dir_path="svg_text_text/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.text = ap.String("Lorem ipsum")\nap.save_overall_html(dest_dir_path="svg_text_text/")\n```',  # noqa
     ##################################################
     "## font_size property interface example": "## font_size 属性のインターフェイス例",
     ##################################################
-    "The `font_size` property updates or gets the instance\'s font size.": "`font_size`属性ではインスタンスのフォントサイズの更新もしくは取得を行えます。",  # noqa
+    "The `font_size` property updates or gets the instance's font size.": "`font_size`属性ではインスタンスのフォントサイズの更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    fill_color=\"#aaa\",\n)\nsvg_text.font_size = ap.Int(24)\nap.save_overall_html(dest_dir_path=\"svg_text_font_size/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    fill_color=\"#aaa\",\n)\nsvg_text.font_size = ap.Int(24)\nap.save_overall_html(dest_dir_path=\"svg_text_font_size/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    fill_color="#aaa",\n)\nsvg_text.font_size = ap.Int(24)\nap.save_overall_html(dest_dir_path="svg_text_font_size/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    fill_color="#aaa",\n)\nsvg_text.font_size = ap.Int(24)\nap.save_overall_html(dest_dir_path="svg_text_font_size/")\n```',  # noqa
     ##################################################
     "## font_family property interface example": "## font_family 属性のインターフェイス例",
     ##################################################
-    "The `font_family` property updates or gets the instance\'s font family.": "`font_family`属性ではインスタンスのフォントファミリー（フォントの指定）の更新もしくは取得を行えます。",  # noqa
+    "The `font_family` property updates or gets the instance's font family.": "`font_family`属性ではインスタンスのフォントファミリー（フォントの指定）の更新もしくは取得を行えます。",  # noqa
     ##################################################
     "This property requires an `Array` of each font name `String`.": "この属性は各フォント名の`String`型の文字列を格納した`Array`型の配列を必要とします。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.font_family = ap.Array([ap.String(\"Impact\"), ap.String(\"Times New Roman\")])\nap.save_overall_html(dest_dir_path=\"svg_text_font_family/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.font_family = ap.Array([ap.String(\"Impact\"), ap.String(\"Times New Roman\")])\nap.save_overall_html(dest_dir_path=\"svg_text_font_family/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.font_family = ap.Array([ap.String("Impact"), ap.String("Times New Roman")])\nap.save_overall_html(dest_dir_path="svg_text_font_family/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.font_family = ap.Array([ap.String("Impact"), ap.String("Times New Roman")])\nap.save_overall_html(dest_dir_path="svg_text_font_family/")\n```',  # noqa
     ##################################################
     "## x property interface example": "## x属性のインターフェイス例",
     ##################################################
-    "The `x` property updates or gets the instance\'s x-coordinate:": "`x`属性ではX座標の値の更新もしくは取得を行えます:",  # noqa
+    "The `x` property updates or gets the instance's x-coordinate:": "`x`属性ではX座標の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.x = ap.Number(50)\nap.save_overall_html(dest_dir_path=\"svg_text_x/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.x = ap.Number(50)\nap.save_overall_html(dest_dir_path=\"svg_text_x/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.x = ap.Number(50)\nap.save_overall_html(dest_dir_path="svg_text_x/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.x = ap.Number(50)\nap.save_overall_html(dest_dir_path="svg_text_x/")\n```',  # noqa
     ##################################################
     "## y property interface example": "## y属性のインターフェイス例",
     ##################################################
-    "The `y` property updates or gets the instance\'s y-coordinate:": "`y`属性ではY座標の値の更新もしくは取得を行えます:",  # noqa
+    "The `y` property updates or gets the instance's y-coordinate:": "`y`属性ではY座標の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=70, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.y = ap.Number(45)\nap.save_overall_html(dest_dir_path=\"svg_text_y/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=70, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.y = ap.Number(45)\nap.save_overall_html(dest_dir_path=\"svg_text_y/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=70, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.y = ap.Number(45)\nap.save_overall_html(dest_dir_path="svg_text_y/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=70, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.y = ap.Number(45)\nap.save_overall_html(dest_dir_path="svg_text_y/")\n```',  # noqa
     ##################################################
     "## fill_color property interface example": "## fill_color属性のインターフェイス例",
     ##################################################
-    "The `fill_color` property updates or gets the instance\'s fill color:": "`fill_color`属性は塗りの色の値の更新もしくは取得を行えます:",  # noqa
+    "The `fill_color` property updates or gets the instance's fill color:": "`fill_color`属性は塗りの色の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n)\nsvg_text.fill_color = ap.String(\"#0af\")\nap.save_overall_html(dest_dir_path=\"svg_text_fill_color/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n)\nsvg_text.fill_color = ap.String(\"#0af\")\nap.save_overall_html(dest_dir_path=\"svg_text_fill_color/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n)\nsvg_text.fill_color = ap.String("#0af")\nap.save_overall_html(dest_dir_path="svg_text_fill_color/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n)\nsvg_text.fill_color = ap.String("#0af")\nap.save_overall_html(dest_dir_path="svg_text_fill_color/")\n```',  # noqa
     ##################################################
     "## fill_alpha property interface example": "## fill_alpha属性のインターフェイス例",
     ##################################################
-    "The `fill_alpha` property updates or gets the instance\'s fill alpha (opacity):": "`fill_alpha`属性は塗りの透明度の値の更新もしくは取得を行えます:",  # noqa
+    "The `fill_alpha` property updates or gets the instance's fill alpha (opacity):": "`fill_alpha`属性は塗りの透明度の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.fill_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path=\"svg_text_fill_alpha/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.fill_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path=\"svg_text_fill_alpha/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.fill_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path="svg_text_fill_alpha/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.fill_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path="svg_text_fill_alpha/")\n```',  # noqa
     ##################################################
     "## line_color property interface example": "## line_color属性のインターフェイス例",
     ##################################################
-    "The `line_color` property updates or gets the instance\'s line color:": "`line_color`属性では線の色の値の更新もしくは取得を行えます:",  # noqa
+    "The `line_color` property updates or gets the instance's line color:": "`line_color`属性では線の色の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=\"\",\n    line_thickness=1,\n)\nsvg_text.line_color = ap.String(\"#0af\")\nap.save_overall_html(dest_dir_path=\"svg_text_line_color/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=\"\",\n    line_thickness=1,\n)\nsvg_text.line_color = ap.String(\"#0af\")\nap.save_overall_html(dest_dir_path=\"svg_text_line_color/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color="",\n    line_thickness=1,\n)\nsvg_text.line_color = ap.String("#0af")\nap.save_overall_html(dest_dir_path="svg_text_line_color/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color="",\n    line_thickness=1,\n)\nsvg_text.line_color = ap.String("#0af")\nap.save_overall_html(dest_dir_path="svg_text_line_color/")\n```',  # noqa
     ##################################################
     "## line_alpha property interface example": "## line_alpha属性のインターフェイス例",
     ##################################################
-    "The `line_alpha` property updates or gets the instance\'s line alpha (opacity):": "`line_alpha`属性では線の透明度の値の更新もしくは取得を行えます:",  # noqa
+    "The `line_alpha` property updates or gets the instance's line alpha (opacity):": "`line_alpha`属性では線の透明度の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=\"\",\n    line_color=\"#0af\",\n    line_thickness=1,\n)\nsvg_text.line_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path=\"svg_text_line_alpha/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=\"\",\n    line_color=\"#0af\",\n    line_thickness=1,\n)\nsvg_text.line_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path=\"svg_text_line_alpha/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color="",\n    line_color="#0af",\n    line_thickness=1,\n)\nsvg_text.line_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path="svg_text_line_alpha/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color="",\n    line_color="#0af",\n    line_thickness=1,\n)\nsvg_text.line_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path="svg_text_line_alpha/")\n```',  # noqa
     ##################################################
     "## line_thickness property interface example": "## line_thickness属性のインターフェイス例",
     ##################################################
-    "The `line_thickness` property updates or gets the instance\'s line thickness (line width):": "`line_thickness`属性では線の幅の更新もしくは取得を行えます:",  # noqa
+    "The `line_thickness` property updates or gets the instance's line thickness (line width):": "`line_thickness`属性では線の幅の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=\"\",\n    line_color=\"#0af\",\n)\nsvg_text.line_thickness = ap.Int(3)\nap.save_overall_html(dest_dir_path=\"svg_text_line_thickness/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=\"\",\n    line_color=\"#0af\",\n)\nsvg_text.line_thickness = ap.Int(3)\nap.save_overall_html(dest_dir_path=\"svg_text_line_thickness/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color="",\n    line_color="#0af",\n)\nsvg_text.line_thickness = ap.Int(3)\nap.save_overall_html(dest_dir_path="svg_text_line_thickness/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color="",\n    line_color="#0af",\n)\nsvg_text.line_thickness = ap.Int(3)\nap.save_overall_html(dest_dir_path="svg_text_line_thickness/")\n```',  # noqa
     ##################################################
     "## leading property interface example": "## leading 属性のインターフェイス例",
     ##################################################
-    "The `leading` property updates or gets the instance\'s text leading (line height).": "`leading`属性ではインスタンスの行間の更新もしくは取得を行えます。",  # noqa
+    "The `leading` property updates or gets the instance's text leading (line height).": "`leading`属性ではインスタンスの行間の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=500, stage_height=120, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n\"\n    \"sed do eiusmod tempor incididunt\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.leading = ap.Number(2.0)\n\nap.save_overall_html(dest_dir_path=\"svg_text_leading/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=500, stage_height=120, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n\"\n    \"sed do eiusmod tempor incididunt\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.leading = ap.Number(2.0)\n\nap.save_overall_html(dest_dir_path=\"svg_text_leading/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=500, stage_height=120, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n"\n    "sed do eiusmod tempor incididunt",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.leading = ap.Number(2.0)\n\nap.save_overall_html(dest_dir_path="svg_text_leading/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=500, stage_height=120, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n"\n    "sed do eiusmod tempor incididunt",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.leading = ap.Number(2.0)\n\nap.save_overall_html(dest_dir_path="svg_text_leading/")\n```',  # noqa
     ##################################################
     "## align property interface example": "## align 属性のインターフェイス例",
     ##################################################
-    "The `align` property updates or gets the instance\'s horizontal text alignment (left, center, or right).": "`align`属性ではインスタンスの水平方向の行揃えの設定（左端、中央、右端）の更新もしくは取得を行えます。",  # noqa
+    "The `align` property updates or gets the instance's horizontal text alignment (left, center, or right).": "`align`属性ではインスタンスの水平方向の行揃えの設定（左端、中央、右端）の更新もしくは取得を行えます。",  # noqa
     ##################################################
     "This property requires the `SVGTextAlign` enum.": "この属性は`SVGTextAlign`のenumの値を必要とします。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=500, stage_height=100, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n\"\n    \"sed do eiusmod tempor incididunt\",\n    x=250,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.align = ap.SVGTextAlign.CENTER\n\nap.save_overall_html(dest_dir_path=\"svg_text_align/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=500, stage_height=100, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n\"\n    \"sed do eiusmod tempor incididunt\",\n    x=250,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.align = ap.SVGTextAlign.CENTER\n\nap.save_overall_html(dest_dir_path=\"svg_text_align/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=500, stage_height=100, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n"\n    "sed do eiusmod tempor incididunt",\n    x=250,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.align = ap.SVGTextAlign.CENTER\n\nap.save_overall_html(dest_dir_path="svg_text_align/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=500, stage_height=100, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n"\n    "sed do eiusmod tempor incididunt",\n    x=250,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.align = ap.SVGTextAlign.CENTER\n\nap.save_overall_html(dest_dir_path="svg_text_align/")\n```',  # noqa
     ##################################################
     "Note: This property setting changes x coordinate baseline (position of `x=0`), as follows:": "特記事項: この属性はX座標の基準位置（`x=0`の位置）を以下のように変更します:",  # noqa
     ##################################################
-    "- SVGTextAlign.CENTER: X coordinate baseline becomes the text\'s center position.": "- SVGTextAlign.CENTER: X座標の基準位置はテキストの中央位置になります。",  # noqa
+    "- SVGTextAlign.CENTER: X coordinate baseline becomes the text's center position.": "- SVGTextAlign.CENTER: X座標の基準位置はテキストの中央位置になります。",  # noqa
     ##################################################
-    "- SVGTextAlign.RIGHT: X coordinate baseline becomes the text\'s right position.": "- SVGTextAlign.RIGHT: X座標の基準位置はテキストの右端の位置になります。",  # noqa
+    "- SVGTextAlign.RIGHT: X coordinate baseline becomes the text's right position.": "- SVGTextAlign.RIGHT: X座標の基準位置はテキストの右端の位置になります。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nSTAGE_WIDTH: int = 500\nSTAGE_HEIGHT: int = 120\nap.Stage(\n    background_color=\"#333\",\n    stage_width=STAGE_WIDTH,\n    stage_height=STAGE_HEIGHT,\n    stage_elem_id=\"stage\",\n)\ncontainer_sprite: ap.Sprite = ap.Sprite()\ncontainer_sprite.x = ap.Number(STAGE_WIDTH / 2)\n\nvertical_x0_line: ap.Line = ap.Line(\n    start_point=ap.Point2D(0, 0),\n    end_point=ap.Point2D(0, STAGE_HEIGHT),\n    line_color=\"#666\",\n    parent=container_sprite,\n)\nx0_text: ap.SVGText = ap.SVGText(\n    text=\"Text\'s x=0 position\",\n    fill_color=\"#666\",\n    x=5,\n    y=20,\n    parent=container_sprite,\n)\n\nleft_align_sample_text: ap.SVGText = ap.SVGText(\n    text=\"Left align sample (default)\",\n    x=0,\n    y=52,\n    fill_color=\"#aaa\",\n    parent=container_sprite,\n)\n\ncenter_align_sample_text: ap.SVGText = ap.SVGText(\n    text=\"Center align sample\",\n    x=0,\n    y=72,\n    fill_color=\"#aaa\",\n    parent=container_sprite,\n)\ncenter_align_sample_text.align = ap.SVGTextAlign.CENTER\n\nright_align_sample_text: ap.SVGText = ap.SVGText(\n    text=\"Right align sample\",\n    x=0,\n    y=92,\n    fill_color=\"#aaa\",\n    parent=container_sprite,\n)\nright_align_sample_text.align = ap.SVGTextAlign.RIGHT\n\nap.save_overall_html(dest_dir_path=\"svg_text_align_note/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nSTAGE_WIDTH: int = 500\nSTAGE_HEIGHT: int = 120\nap.Stage(\n    background_color=\"#333\",\n    stage_width=STAGE_WIDTH,\n    stage_height=STAGE_HEIGHT,\n    stage_elem_id=\"stage\",\n)\ncontainer_sprite: ap.Sprite = ap.Sprite()\ncontainer_sprite.x = ap.Number(STAGE_WIDTH / 2)\n\nvertical_x0_line: ap.Line = ap.Line(\n    start_point=ap.Point2D(0, 0),\n    end_point=ap.Point2D(0, STAGE_HEIGHT),\n    line_color=\"#666\",\n    parent=container_sprite,\n)\nx0_text: ap.SVGText = ap.SVGText(\n    text=\"Text\'s x=0 position\",\n    fill_color=\"#666\",\n    x=5,\n    y=20,\n    parent=container_sprite,\n)\n\nleft_align_sample_text: ap.SVGText = ap.SVGText(\n    text=\"Left align sample (default)\",\n    x=0,\n    y=52,\n    fill_color=\"#aaa\",\n    parent=container_sprite,\n)\n\ncenter_align_sample_text: ap.SVGText = ap.SVGText(\n    text=\"Center align sample\",\n    x=0,\n    y=72,\n    fill_color=\"#aaa\",\n    parent=container_sprite,\n)\ncenter_align_sample_text.align = ap.SVGTextAlign.CENTER\n\nright_align_sample_text: ap.SVGText = ap.SVGText(\n    text=\"Right align sample\",\n    x=0,\n    y=92,\n    fill_color=\"#aaa\",\n    parent=container_sprite,\n)\nright_align_sample_text.align = ap.SVGTextAlign.RIGHT\n\nap.save_overall_html(dest_dir_path=\"svg_text_align_note/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nSTAGE_WIDTH: int = 500\nSTAGE_HEIGHT: int = 120\nap.Stage(\n    background_color="#333",\n    stage_width=STAGE_WIDTH,\n    stage_height=STAGE_HEIGHT,\n    stage_elem_id="stage",\n)\ncontainer_sprite: ap.Sprite = ap.Sprite()\ncontainer_sprite.x = ap.Number(STAGE_WIDTH / 2)\n\nvertical_x0_line: ap.Line = ap.Line(\n    start_point=ap.Point2D(0, 0),\n    end_point=ap.Point2D(0, STAGE_HEIGHT),\n    line_color="#666",\n    parent=container_sprite,\n)\nx0_text: ap.SVGText = ap.SVGText(\n    text="Text\'s x=0 position",\n    fill_color="#666",\n    x=5,\n    y=20,\n    parent=container_sprite,\n)\n\nleft_align_sample_text: ap.SVGText = ap.SVGText(\n    text="Left align sample (default)",\n    x=0,\n    y=52,\n    fill_color="#aaa",\n    parent=container_sprite,\n)\n\ncenter_align_sample_text: ap.SVGText = ap.SVGText(\n    text="Center align sample",\n    x=0,\n    y=72,\n    fill_color="#aaa",\n    parent=container_sprite,\n)\ncenter_align_sample_text.align = ap.SVGTextAlign.CENTER\n\nright_align_sample_text: ap.SVGText = ap.SVGText(\n    text="Right align sample",\n    x=0,\n    y=92,\n    fill_color="#aaa",\n    parent=container_sprite,\n)\nright_align_sample_text.align = ap.SVGTextAlign.RIGHT\n\nap.save_overall_html(dest_dir_path="svg_text_align_note/")\n```': '```py\n# runnable\nimport apysc as ap\n\nSTAGE_WIDTH: int = 500\nSTAGE_HEIGHT: int = 120\nap.Stage(\n    background_color="#333",\n    stage_width=STAGE_WIDTH,\n    stage_height=STAGE_HEIGHT,\n    stage_elem_id="stage",\n)\ncontainer_sprite: ap.Sprite = ap.Sprite()\ncontainer_sprite.x = ap.Number(STAGE_WIDTH / 2)\n\nvertical_x0_line: ap.Line = ap.Line(\n    start_point=ap.Point2D(0, 0),\n    end_point=ap.Point2D(0, STAGE_HEIGHT),\n    line_color="#666",\n    parent=container_sprite,\n)\nx0_text: ap.SVGText = ap.SVGText(\n    text="Text\'s x=0 position",\n    fill_color="#666",\n    x=5,\n    y=20,\n    parent=container_sprite,\n)\n\nleft_align_sample_text: ap.SVGText = ap.SVGText(\n    text="Left align sample (default)",\n    x=0,\n    y=52,\n    fill_color="#aaa",\n    parent=container_sprite,\n)\n\ncenter_align_sample_text: ap.SVGText = ap.SVGText(\n    text="Center align sample",\n    x=0,\n    y=72,\n    fill_color="#aaa",\n    parent=container_sprite,\n)\ncenter_align_sample_text.align = ap.SVGTextAlign.CENTER\n\nright_align_sample_text: ap.SVGText = ap.SVGText(\n    text="Right align sample",\n    x=0,\n    y=92,\n    fill_color="#aaa",\n    parent=container_sprite,\n)\nright_align_sample_text.align = ap.SVGTextAlign.RIGHT\n\nap.save_overall_html(dest_dir_path="svg_text_align_note/")\n```',  # noqa
     ##################################################
     "## bold property interface example": "## bold 属性のインターフェイス例",
     ##################################################
-    "The `bold` property updates or gets the instance\'s `bold` text setting.": "`bold`属性ではインスタンスの太字設定の更新もしくは取得を行えます。",  # noqa
+    "The `bold` property updates or gets the instance's `bold` text setting.": "`bold`属性ではインスタンスの太字設定の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Bold style sample\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.bold = ap.Boolean(True)\nap.save_overall_html(dest_dir_path=\"svg_text_bold/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Bold style sample\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.bold = ap.Boolean(True)\nap.save_overall_html(dest_dir_path=\"svg_text_bold/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Bold style sample",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.bold = ap.Boolean(True)\nap.save_overall_html(dest_dir_path="svg_text_bold/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Bold style sample",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.bold = ap.Boolean(True)\nap.save_overall_html(dest_dir_path="svg_text_bold/")\n```',  # noqa
     ##################################################
     "## italic property interface example": "## italic 属性のインターフェイス例",
     ##################################################
-    "The `italic` property updates or gets the instance\'s `italic` style setting.": "`italic`属性ではインスタンスの斜体の設定の更新もしくは取得を行えます。",  # noqa
+    "The `italic` property updates or gets the instance's `italic` style setting.": "`italic`属性ではインスタンスの斜体の設定の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Italic style sample\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.italic = ap.Boolean(True)\nap.save_overall_html(dest_dir_path=\"svg_text_italic/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Italic style sample\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\nsvg_text.italic = ap.Boolean(True)\nap.save_overall_html(dest_dir_path=\"svg_text_italic/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Italic style sample",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.italic = ap.Boolean(True)\nap.save_overall_html(dest_dir_path="svg_text_italic/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Italic style sample",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\nsvg_text.italic = ap.Boolean(True)\nap.save_overall_html(dest_dir_path="svg_text_italic/")\n```',  # noqa
     ##################################################
     "## rotation_around_center property interface example": "## rotation_around_center属性のインターフェイス例",  # noqa
     ##################################################
-    "The `rotation_around_center` property updates or gets the instance\'s rotation value (0 to 359) from the center point:": "`rotation_around_center`属性ではインスタンスの中央座標での回転量（0～359）の更新もしくは取得を行えます:",  # noqa
+    "The `rotation_around_center` property updates or gets the instance's rotation value (0 to 359) from the center point:": "`rotation_around_center`属性ではインスタンスの中央座標での回転量（0～359）の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=100,\n    y=32,\n    fill_color=\"#aaa\",\n    align=ap.SVGTextAlign.CENTER,\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.rotation_around_center += 1\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_rotation_around_center/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=100,\n    y=32,\n    fill_color=\"#aaa\",\n    align=ap.SVGTextAlign.CENTER,\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.rotation_around_center += 1\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_rotation_around_center/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=100,\n    y=32,\n    fill_color="#aaa",\n    align=ap.SVGTextAlign.CENTER,\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    svg_text.rotation_around_center += 1\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_rotation_around_center/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=100,\n    y=32,\n    fill_color="#aaa",\n    align=ap.SVGTextAlign.CENTER,\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    svg_text.rotation_around_center += 1\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_rotation_around_center/")\n```',  # noqa
     ##################################################
     "## set_rotation_around_point and get_rotation_around_point methods interface example": "## set_rotation_around_pointとget_rotation_around_pointメソッドのインターフェイス例",  # noqa
     ##################################################
-    "The `set_rotation_around_point` method updates the instance\'s rotation value (0 to 359) from a specified point.": "`set_rotation_around_point`メソッドは指定された座標からのインスタンスの回転量（0～359）を更新します。",  # noqa
+    "The `set_rotation_around_point` method updates the instance's rotation value (0 to 359) from a specified point.": "`set_rotation_around_point`メソッドは指定された座標からのインスタンスの回転量（0～359）を更新します。",  # noqa
     ##################################################
-    "Similarly, the `get_rotation_around_point` method gets the instance\'s rotation value (0 to 359) from a specified point:": "同様に、`get_rotation_around_point`メソッドでは指定された座標のインスタンスの回転量（0～359）を取得します:",  # noqa
+    "Similarly, the `get_rotation_around_point` method gets the instance's rotation value (0 to 359) from a specified point:": "同様に、`get_rotation_around_point`メソッドでは指定された座標のインスタンスの回転量（0～359）を取得します:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=120, stage_elem_id=\"stage\"\n)\nX: ap.Number = ap.Number(20)\nY: ap.Number = ap.Number(32)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=X,\n    y=Y,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    rotation: ap.Int = (\n        svg_text.get_rotation_around_point(\n            x=X,\n            y=Y,\n        )\n        + 1\n    )\n    svg_text.set_rotation_around_point(\n        rotation=rotation,\n        x=X,\n        y=Y,\n    )\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_rotation_around_point/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=120, stage_elem_id=\"stage\"\n)\nX: ap.Number = ap.Number(20)\nY: ap.Number = ap.Number(32)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=X,\n    y=Y,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    rotation: ap.Int = (\n        svg_text.get_rotation_around_point(\n            x=X,\n            y=Y,\n        )\n        + 1\n    )\n    svg_text.set_rotation_around_point(\n        rotation=rotation,\n        x=X,\n        y=Y,\n    )\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_rotation_around_point/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=120, stage_elem_id="stage"\n)\nX: ap.Number = ap.Number(20)\nY: ap.Number = ap.Number(32)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=X,\n    y=Y,\n    fill_color="#aaa",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    rotation: ap.Int = (\n        svg_text.get_rotation_around_point(\n            x=X,\n            y=Y,\n        )\n        + 1\n    )\n    svg_text.set_rotation_around_point(\n        rotation=rotation,\n        x=X,\n        y=Y,\n    )\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_rotation_around_point/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=120, stage_elem_id="stage"\n)\nX: ap.Number = ap.Number(20)\nY: ap.Number = ap.Number(32)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=X,\n    y=Y,\n    fill_color="#aaa",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    rotation: ap.Int = (\n        svg_text.get_rotation_around_point(\n            x=X,\n            y=Y,\n        )\n        + 1\n    )\n    svg_text.set_rotation_around_point(\n        rotation=rotation,\n        x=X,\n        y=Y,\n    )\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_rotation_around_point/")\n```',  # noqa
     ##################################################
     "## Scale-related interfaces note": "## 拡縮関係のインターフェイスに対する特記事項",
     ##################################################
     "The scale-related interfaces are not recommended as the display may become distorted depending on the settings.": "拡縮関係のインターフェイスは設定次第では表示が崩れたりするため利用は非推奨です。",  # noqa
     ##################################################
     "## scale_x_from_center property interface example": "## scale_x_from_center属性のインターフェイス例",  # noqa
     ##################################################
-    "The `scale_x_from_center` property updates or gets the instance\'s scale-x from the center point:": "`scale_x_from_center`属性ではインスタンスの中央座標でのX軸の拡縮値の更新もしくは取得を行えます:",  # noqa
+    "The `scale_x_from_center` property updates or gets the instance's scale-x from the center point:": "`scale_x_from_center`属性ではインスタンスの中央座標でのX軸の拡縮値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    scale: ap.Number = svg_text.scale_x_from_center\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.scale_x_from_center = scale\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_scale_x_from_center/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    scale: ap.Number = svg_text.scale_x_from_center\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.scale_x_from_center = scale\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_scale_x_from_center/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    scale: ap.Number = svg_text.scale_x_from_center\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.scale_x_from_center = scale\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_scale_x_from_center/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    scale: ap.Number = svg_text.scale_x_from_center\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.scale_x_from_center = scale\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_scale_x_from_center/")\n```',  # noqa
     ##################################################
     "## set_scale_x_from_point and get_scale_x_from_point methods interface example": "## set_scale_x_from_pointとget_scale_x_from_pointメソッドのインターフェイス例",  # noqa
     ##################################################
-    "The `set_scale_x_from_point` method updates the instance\'s scale-x from a specified point.": "`set_scale_x_from_point`メソッドは指定されたX座標を基準としてX軸の拡縮値を更新します。",  # noqa
+    "The `set_scale_x_from_point` method updates the instance's scale-x from a specified point.": "`set_scale_x_from_point`メソッドは指定されたX座標を基準としてX軸の拡縮値を更新します。",  # noqa
     ##################################################
-    "Similarly, the `get_scale_x_from_point` method gets the instance\'s scale-x from a specified point:": "同様に、`get_scale_x_from_point`メソッドでは指定されたX座標を基準としたX軸の拡縮値を取得します:",  # noqa
+    "Similarly, the `get_scale_x_from_point` method gets the instance's scale-x from a specified point:": "同様に、`get_scale_x_from_point`メソッドでは指定されたX座標を基準としたX軸の拡縮値を取得します:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nX: ap.Number = ap.Number(20)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=X,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    scale: ap.Number = svg_text.get_scale_x_from_point(x=X)\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.set_scale_x_from_point(scale_x=scale, x=X)\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_scale_x_from_point/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nX: ap.Number = ap.Number(20)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=X,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    scale: ap.Number = svg_text.get_scale_x_from_point(x=X)\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.set_scale_x_from_point(scale_x=scale, x=X)\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_scale_x_from_point/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nX: ap.Number = ap.Number(20)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=X,\n    y=32,\n    fill_color="#aaa",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    scale: ap.Number = svg_text.get_scale_x_from_point(x=X)\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.set_scale_x_from_point(scale_x=scale, x=X)\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_scale_x_from_point/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nX: ap.Number = ap.Number(20)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=X,\n    y=32,\n    fill_color="#aaa",\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    scale: ap.Number = svg_text.get_scale_x_from_point(x=X)\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.set_scale_x_from_point(scale_x=scale, x=X)\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_scale_x_from_point/")\n```',  # noqa
     ##################################################
     "## flip_x property interface example": "## flip_x属性のインターフェイス例",
     ##################################################
-    "The `flip_x` property updates or gets the instance\'s flip-x (reflecting state) boolean value:": "`flip_x`属性ではインスタンスのX軸の反転状況の真偽値の更新もしくは取得を行えます:",  # noqa
+    "The `flip_x` property updates or gets the instance's flip-x (reflecting state) boolean value:": "`flip_x`属性ではインスタンスのX軸の反転状況の真偽値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.flip_x = svg_text.flip_x.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path=\"svg_txt_flip_x/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.flip_x = svg_text.flip_x.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path=\"svg_txt_flip_x/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    """\n    svg_text.flip_x = svg_text.flip_x.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path="svg_txt_flip_x/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    """\n    svg_text.flip_x = svg_text.flip_x.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path="svg_txt_flip_x/")\n```',  # noqa
     ##################################################
     "## flip_y property interface example": "## flip_y属性のインターフェイス例",
     ##################################################
-    "The `flip_y` property updates or gets the instance\'s flip-y (reflecting state) boolean value:": "`flip_y`属性ではインスタンスのX軸の反転状況の真偽値の更新もしくは取得を行えます:",  # noqa
+    "The `flip_y` property updates or gets the instance's flip-y (reflecting state) boolean value:": "`flip_y`属性ではインスタンスのX軸の反転状況の真偽値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.flip_y = svg_text.flip_y.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path=\"svg_txt_flip_y/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.flip_y = svg_text.flip_y.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path=\"svg_txt_flip_y/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    """\n    svg_text.flip_y = svg_text.flip_y.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path="svg_txt_flip_y/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    """\n    svg_text.flip_y = svg_text.flip_y.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path="svg_txt_flip_y/")\n```',  # noqa
     ##################################################
     "## SVGText constructor API": "## SVGText クラスのコンストラクタのAPI",
     ##################################################
-    "<span class=\"inconspicuous-txt\">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>": "<span class=\"inconspicuous-txt\">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>",  # noqa
+    '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
     "The class for an SVG text.<hr>": "SVGテキストのためのクラスです。<hr>",
     ##################################################
     "**[Parameters]**": "**[引数]**",
     ##################################################
@@ -207,15 +207,15 @@
     ##################################################
     "  - A fill-color setting.": "  - 塗りの色の設定。",
     ##################################################
     "- `fill_alpha`: float or Number, optional": "- `fill_alpha`: float or Number, optional",  # noqa
     ##################################################
     "  - A fill-alpha setting.": "  - 塗りの透明度の設定。",
     ##################################################
-    "- `line_color`: str or String, default \'\'": "- `line_color`: str or String, default \'\'",  # noqa
+    "- `line_color`: str or String, default ''": "- `line_color`: str or String, default ''",  # noqa
     ##################################################
     "  - A line-color setting.": "  - 線の色の設定。",
     ##################################################
     "- `line_alpha`: float or Number, optional": "- `line_alpha`: float or Number, optional",  # noqa
     ##################################################
     "  - A line-alpha setting.": "  - 線の透明度の設定。",
     ##################################################
@@ -229,15 +229,15 @@
     ##################################################
     "- `align`: SVGTextAlign, default SVGTextAlign.LEFT": "- `align`: SVGTextAlign, default SVGTextAlign.LEFT",  # noqa
     ##################################################
     "  - A text-align setting.": "  - テキストの行揃えの設定。",
     ##################################################
     "- `bold`: Union[bool, Boolean], optional": "- `bold`: Union[bool, Boolean], optional",  # noqa
     ##################################################
-    "  - A boolean, whether this text is bold style or not.": "  - テキストに太字のスタイル設定を行うかどうかの真偽値。",  # noqa
+    "  - A boolean, whether this text is a bold style or not.": "  - テキストに太字のスタイル設定を行うかどうかの真偽値。",  # noqa
     ##################################################
     "- `italic`: Union[bool, Boolean], optional": "- `italic`: Union[bool, Boolean], optional",  # noqa
     ##################################################
     "  - A boolean, whether a text is an italic style or not (normal).": "  - テキストを斜体表示のスタイル設定を行うかどうかの真偽値。",  # noqa
     ##################################################
     "- `parent`: ChildMixIn or None, optional": "- `parent`: ChildMixIn or None, optional",  # noqa
     ##################################################
@@ -247,13 +247,13 @@
     ##################################################
     "  - A JavaScript variable name suffix string. This setting is sometimes useful for JavaScript debugging.": "  - JavaScript上の変数のサフィックスの設定です。この設定はJavaScriptのデバッグ時に役立つことがあります。",  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[Notes]**": "**[特記事項]**",
     ##################################################
-    " ・SVGText\'s y-coordinate zero-position starts at the bottom of a text. So if you set y=0, a text becomes almost invisible.<hr>": " ・SVGTextクラスの座標の0の位置はテキストの下部からスタートします。そのためもしもy=0を指定した場合、テキストはほとんど見えない状態になります。<hr>",  # noqa
+    " ・SVGText's y-coordinate zero-position starts at the bottom of a text. So if you set y=0, a text becomes almost invisible.<hr>": " ・SVGTextクラスの座標の0の位置はテキストの下部からスタートします。そのためもしもy=0を指定した場合、テキストはほとんど見えない状態になります。<hr>",  # noqa
     ##################################################
     "**[Examples]**": "**[コードサンプル]**",
     ##################################################
-    "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n... )\n>>> svg_text: ap.SVGText = ap.SVGText(\n...     text=\"Hello, world!\",\n...     font_size=20,\n...     fill_color=\"#0af\",\n... )\n>>> svg_text.text\nString(\"Hello, world!\")\n\n>>> svg_text.font_size\nInt(20)\n\n>>> svg_text.fill_color\nString(\"#00aaff\")\n```": "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n... )\n>>> svg_text: ap.SVGText = ap.SVGText(\n...     text=\"Hello, world!\",\n...     font_size=20,\n...     fill_color=\"#0af\",\n... )\n>>> svg_text.text\nString(\"Hello, world!\")\n\n>>> svg_text.font_size\nInt(20)\n\n>>> svg_text.fill_color\nString(\"#00aaff\")\n```",  # noqa
+    '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color="#333",\n...     stage_width=200,\n...     stage_height=50,\n...     stage_elem_id="stage",\n... )\n>>> svg_text: ap.SVGText = ap.SVGText(\n...     text="Hello, world!",\n...     font_size=20,\n...     fill_color="#0af",\n... )\n>>> svg_text.text\nString("Hello, world!")\n\n>>> svg_text.font_size\nInt(20)\n\n>>> svg_text.fill_color\nString("#00aaff")\n```': '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color="#333",\n...     stage_width=200,\n...     stage_height=50,\n...     stage_elem_id="stage",\n... )\n>>> svg_text: ap.SVGText = ap.SVGText(\n...     text="Hello, world!",\n...     font_size=20,\n...     fill_color="#0af",\n... )\n>>> svg_text.text\nString("Hello, world!")\n\n>>> svg_text.font_size\nInt(20)\n\n>>> svg_text.fill_color\nString("#00aaff")\n```',  # noqa
 }
```

### Comparing `apysc-2.7.9/apysc/_translation/jp/svg_text_span.py` & `apysc-2.8.0/apysc/_translation/jp/svg_text_span.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,111 +19,111 @@
     ##################################################
     "You can create an `SVGText` instance with multiple `SVGTextSpan` class instances and set different text styles.": "複数の`SVGTextSpan`クラスのインスタンスを使ってそれぞれに異なるテキストのスタイルを設定した状態の`SVGText`のインスタンスを作成することができます。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
     "The `SVGTextSpan` class constructor requires the `text` argument.": "`SVGTextSpan`クラスのコンストラクタには`text`引数を必要とします。",  # noqa
     ##################################################
-    "The constructor also accepts each font\'s and style\'s argument, such as the `font_size`, `font_family`, `fill_color`, and `bold`.": "コンストラクタでは`font_size`や`font_family`、`fill_color`、`bold`などの各スタイル設定の引数を受け付けます。",  # noqa
+    "The constructor also accepts each font's and style's argument, such as the `font_size`, `font_family`, `fill_color`, and `bold`.": "コンストラクタでは`font_size`や`font_family`、`fill_color`、`bold`などの各スタイル設定の引数を受け付けます。",  # noqa
     ##################################################
-    "If you skip the style settings\' arguments, these settings become the parent SVGText\'s styles.": "もしもそれらのスタイル設定の引数指定を省略した場合、親のSVGTextのインスタンスのスタイルが反映されます。",  # noqa
+    "If you skip the style settings' arguments, these settings become the parent SVGText's styles.": "もしもそれらのスタイル設定の引数指定を省略した場合、親のSVGTextのインスタンスのスタイルが反映されます。",  # noqa
     ##################################################
     "You can use `SVGTextSpan` instances to create an `SVGText` instance with the `create_with_svg_text_spans` class method.": "また、複数の`SVGTextSpan`のインスタンスを使って`SVGText`のインスタンスの作成するには`create_with_svg_text_spans`のクラスメソッドを使うことで対応ができます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SVGTextSpan(text=\"Lorem \"),\n        ap.SVGTextSpan(text=\"ipsum \", font_size=20, fill_color=\"#0af\"),\n        ap.SVGTextSpan(text=\"dolor \", font_size=12),\n    ],\n    fill_color=\"#aaa\",\n    font_size=16,\n    x=20,\n    y=32,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_basic_usage/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SVGTextSpan(text=\"Lorem \"),\n        ap.SVGTextSpan(text=\"ipsum \", font_size=20, fill_color=\"#0af\"),\n        ap.SVGTextSpan(text=\"dolor \", font_size=12),\n    ],\n    fill_color=\"#aaa\",\n    font_size=16,\n    x=20,\n    y=32,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_basic_usage/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SVGTextSpan(text="Lorem "),\n        ap.SVGTextSpan(text="ipsum ", font_size=20, fill_color="#0af"),\n        ap.SVGTextSpan(text="dolor ", font_size=12),\n    ],\n    fill_color="#aaa",\n    font_size=16,\n    x=20,\n    y=32,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SVGTextSpan(text="Lorem "),\n        ap.SVGTextSpan(text="ipsum ", font_size=20, fill_color="#0af"),\n        ap.SVGTextSpan(text="dolor ", font_size=12),\n    ],\n    fill_color="#aaa",\n    font_size=16,\n    x=20,\n    y=32,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_basic_usage/")\n```',  # noqa
     ##################################################
     "## Notes of the line breaking": "## 改行に対する特記事項",
     ##################################################
     "The `SVGTextSpan` class ignores line breaks.": "`SVGTextSpan`クラスは改行設定を無視します。",
     ##################################################
-    "For instance, the following example\'s text contains a line break (`\n`), but the text line becomes a single line.": "例えば、以下の例では改行用の文字列（`\n`）を含んでいますがテキストの行は単一行になっています。",  # noqa
+    "For instance, the following example's text contains a line break (`\n`), but the text line becomes a single line.": "例えば、以下の例では改行用の文字列（`\n`）を含んでいますがテキストの行は単一行になっています。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SVGTextSpan(text=\"Lorem \n\"),\n        ap.SVGTextSpan(text=\"ipsum \n\"),\n        ap.SVGTextSpan(text=\"dolor\"),\n    ],\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_notes_of_the_line_break/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SVGTextSpan(text=\"Lorem \n\"),\n        ap.SVGTextSpan(text=\"ipsum \n\"),\n        ap.SVGTextSpan(text=\"dolor\"),\n    ],\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_notes_of_the_line_break/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SVGTextSpan(text="Lorem \n"),\n        ap.SVGTextSpan(text="ipsum \n"),\n        ap.SVGTextSpan(text="dolor"),\n    ],\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_notes_of_the_line_break/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SVGTextSpan(text="Lorem \n"),\n        ap.SVGTextSpan(text="ipsum \n"),\n        ap.SVGTextSpan(text="dolor"),\n    ],\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_notes_of_the_line_break/")\n```',  # noqa
     ##################################################
     "If you want to add a line break, please use the `SVGText` class (not the `SVGTextSpan`) or create multiple `SVGText` instances.": "もしも改行を加えたい場合には`SVGTextSpan`クラスではなく`SVGText`クラスを使用するか、もしくは複数のインスタンスを作成して対応をお願いします。",  # noqa
     ##################################################
     "## text property interface example": "## text 属性のインターフェイス例",
     ##################################################
-    "The `text` property updates or gets the instance\'s text.": "`text`属性ではインスタンスのテキストの更新もしくは取得を行えます。",  # noqa
+    "The `text` property updates or gets the instance's text.": "`text`属性ではインスタンスのテキストの更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.text = ap.String(\"dolor\")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_text/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.text = ap.String(\"dolor\")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_text/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.text = ap.String("dolor")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_text/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.text = ap.String("dolor")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_text/")\n```',  # noqa
     ##################################################
     "## font_size property interface example": "## font_size 属性のインターフェイス例",
     ##################################################
-    "The `font_size` property updates or gets the instance\'s font size.": "`font_size`属性ではインスタンスのフォントサイズの更新もしくは取得を行えます。",  # noqa
+    "The `font_size` property updates or gets the instance's font size.": "`font_size`属性ではインスタンスのフォントサイズの更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.font_size = ap.Int(25)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_font_size/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.font_size = ap.Int(25)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_font_size/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.font_size = ap.Int(25)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_font_size/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.font_size = ap.Int(25)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_font_size/")\n```',  # noqa
     ##################################################
     "## font_family property interface example": "## font_family 属性のインターフェイス例",
     ##################################################
-    "The `font_family` property updates or gets the instance\'s font family.": "`font_family`属性ではインスタンスのフォントファミリー（フォントの指定）の更新もしくは取得を行えます。",  # noqa
+    "The `font_family` property updates or gets the instance's font family.": "`font_family`属性ではインスタンスのフォントファミリー（フォントの指定）の更新もしくは取得を行えます。",  # noqa
     ##################################################
     "This property requires an `Array` of each font name `String`.": "この属性は各フォント名の`String`型の文字列を格納した`Array`型の配列を必要とします。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.font_family = ap.Array([ap.String(\"Impact\"), ap.String(\"Arial\")])\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_font_family/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.font_family = ap.Array([ap.String(\"Impact\"), ap.String(\"Arial\")])\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_font_family/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.font_family = ap.Array([ap.String("Impact"), ap.String("Arial")])\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_font_family/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.font_family = ap.Array([ap.String("Impact"), ap.String("Arial")])\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_font_family/")\n```',  # noqa
     ##################################################
     "## fill_color property interface example": "## fill_color属性のインターフェイス例",
     ##################################################
-    "The `fill_color` property updates or gets the instance\'s fill color:": "`fill_color`属性は塗りの色の値の更新もしくは取得を行えます:",  # noqa
+    "The `fill_color` property updates or gets the instance's fill color:": "`fill_color`属性は塗りの色の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.fill_color = ap.String(\"#0af\")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_fill_color/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.fill_color = ap.String(\"#0af\")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_fill_color/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.fill_color = ap.String("#0af")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_fill_color/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.fill_color = ap.String("#0af")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_fill_color/")\n```',  # noqa
     ##################################################
     "## fill_alpha property interface example": "## fill_alpha属性のインターフェイス例",
     ##################################################
-    "The `fill_alpha` property updates or gets the instance\'s fill alpha (opacity):": "`fill_alpha`属性は塗りの透明度の値の更新もしくは取得を行えます:",  # noqa
+    "The `fill_alpha` property updates or gets the instance's fill alpha (opacity):": "`fill_alpha`属性は塗りの透明度の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.fill_alpha = ap.Number(0.3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_fill_alpha/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.fill_alpha = ap.Number(0.3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_fill_alpha/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.fill_alpha = ap.Number(0.3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_fill_alpha/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.fill_alpha = ap.Number(0.3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_fill_alpha/")\n```',  # noqa
     ##################################################
     "## line_color property interface example": "## line_color属性のインターフェイス例",
     ##################################################
-    "The `line_color` property updates or gets the instance\'s line color:": "`line_color`属性では線の色の値の更新もしくは取得を行えます:",  # noqa
+    "The `line_color` property updates or gets the instance's line color:": "`line_color`属性では線の色の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"Lorem \", line_thickness=1, font_size=20, bold=True\n)\ntext_span_1.line_color = ap.String(\"#aaa\")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"ipsum\", line_thickness=1, font_size=20, bold=True\n)\ntext_span_2.line_color = ap.String(\"#0af\")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_color/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"Lorem \", line_thickness=1, font_size=20, bold=True\n)\ntext_span_1.line_color = ap.String(\"#aaa\")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"ipsum\", line_thickness=1, font_size=20, bold=True\n)\ntext_span_2.line_color = ap.String(\"#0af\")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_color/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="Lorem ", line_thickness=1, font_size=20, bold=True\n)\ntext_span_1.line_color = ap.String("#aaa")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="ipsum", line_thickness=1, font_size=20, bold=True\n)\ntext_span_2.line_color = ap.String("#0af")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_color/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="Lorem ", line_thickness=1, font_size=20, bold=True\n)\ntext_span_1.line_color = ap.String("#aaa")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="ipsum", line_thickness=1, font_size=20, bold=True\n)\ntext_span_2.line_color = ap.String("#0af")\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_color/")\n```',  # noqa
     ##################################################
     "## line_alpha property interface example": "## line_alpha属性のインターフェイス例",
     ##################################################
-    "The `line_alpha` property updates or gets the instance\'s line alpha (opacity):": "`line_alpha`属性では線の透明度の値の更新もしくは取得を行えます:",  # noqa
+    "The `line_alpha` property updates or gets the instance's line alpha (opacity):": "`line_alpha`属性では線の透明度の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"Lorem \",\n    line_color=\"#0af\",\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"ipsum\",\n    line_color=\"#0af\",\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2.line_alpha = ap.Number(0.3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_alpha/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"Lorem \",\n    line_color=\"#0af\",\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"ipsum\",\n    line_color=\"#0af\",\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2.line_alpha = ap.Number(0.3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_alpha/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="Lorem ",\n    line_color="#0af",\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="ipsum",\n    line_color="#0af",\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2.line_alpha = ap.Number(0.3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_alpha/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="Lorem ",\n    line_color="#0af",\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="ipsum",\n    line_color="#0af",\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2.line_alpha = ap.Number(0.3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_alpha/")\n```',  # noqa
     ##################################################
     "## line_thickness property interface example": "## line_thickness属性のインターフェイス例",
     ##################################################
-    "The `line_thickness` property updates or gets the instance\'s line thickness (line width):": "`line_thickness`属性では線の幅の更新もしくは取得を行えます:",  # noqa
+    "The `line_thickness` property updates or gets the instance's line thickness (line width):": "`line_thickness`属性では線の幅の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"Lorem \",\n    line_color=\"#0af\",\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"ipsum\",\n    line_color=\"#0af\",\n    font_size=20,\n    bold=True,\n)\ntext_span_1.line_thickness = ap.Int(3)\ntext_span_2.line_thickness = ap.Int(3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_thickness/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"Lorem \",\n    line_color=\"#0af\",\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text=\"ipsum\",\n    line_color=\"#0af\",\n    font_size=20,\n    bold=True,\n)\ntext_span_1.line_thickness = ap.Int(3)\ntext_span_2.line_thickness = ap.Int(3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_thickness/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="Lorem ",\n    line_color="#0af",\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="ipsum",\n    line_color="#0af",\n    font_size=20,\n    bold=True,\n)\ntext_span_1.line_thickness = ap.Int(3)\ntext_span_2.line_thickness = ap.Int(3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_thickness/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="Lorem ",\n    line_color="#0af",\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(\n    text="ipsum",\n    line_color="#0af",\n    font_size=20,\n    bold=True,\n)\ntext_span_1.line_thickness = ap.Int(3)\ntext_span_2.line_thickness = ap.Int(3)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_thickness/")\n```',  # noqa
     ##################################################
     "## bold property interface example": "## bold 属性のインターフェイス例",
     ##################################################
-    "The `bold` property updates or gets the instance\'s `bold` text setting.": "`bold`属性ではインスタンスの太字設定の更新もしくは取得を行えます。",  # noqa
+    "The `bold` property updates or gets the instance's `bold` text setting.": "`bold`属性ではインスタンスの太字設定の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.bold = ap.Boolean(True)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_bold/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.bold = ap.Boolean(True)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_bold/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.bold = ap.Boolean(True)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_bold/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.bold = ap.Boolean(True)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_bold/")\n```',  # noqa
     ##################################################
     "## italic property interface example": "## italic 属性のインターフェイス例",
     ##################################################
-    "The `italic` property updates or gets the instance\'s `italic` style setting.": "`italic`属性ではインスタンスの斜体の設定の更新もしくは取得を行えます。",  # noqa
+    "The `italic` property updates or gets the instance's `italic` style setting.": "`italic`属性ではインスタンスの斜体の設定の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.italic = ap.Boolean(True)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_italic/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.italic = ap.Boolean(True)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_italic/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.italic = ap.Boolean(True)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_italic/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.italic = ap.Boolean(True)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_italic/")\n```',  # noqa
     ##################################################
     "## delta_x property interface example": "## delta_x 属性のインターフェイス例",
     ##################################################
-    "The `delta_x` property updates or gets the instance\'s delta-x (x-coordinate adjustment).": "`delta_x`属性ではインスタンスのX座標の調整値の更新もしくは取得を行えます。",  # noqa
+    "The `delta_x` property updates or gets the instance's delta-x (x-coordinate adjustment).": "`delta_x`属性ではインスタンスのX座標の調整値の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.delta_x = ap.Number(-20)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_delta_x/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=50, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum\")\ntext_span_2.delta_x = ap.Number(-20)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_delta_x/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.delta_x = ap.Number(-20)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_delta_x/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=50, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum")\ntext_span_2.delta_x = ap.Number(-20)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_delta_x/")\n```',  # noqa
     ##################################################
     "## delta_y property interface example": "## delta_y 属性のインターフェイス例",
     ##################################################
-    "The `delta_y` property updates or gets the instance\'s delta-y (y-coordinate adjustment).": "`delta_y`属性ではインスタンスのY座標の調整値の更新もくしは取得を行えます。",  # noqa
+    "The `delta_y` property updates or gets the instance's delta-y (y-coordinate adjustment).": "`delta_y`属性ではインスタンスのY座標の調整値の更新もくしは取得を行えます。",  # noqa
     ##################################################
     "Note: This setting inherits a y-coordinate from the previous `SVGTextSpan` instance.": "特記事項: この設定は直前の`SVGTextSpan`インスタンスの設定を引き継ぎます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=80, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum \")\ntext_span_3: ap.SVGTextSpan = ap.SVGTextSpan(text=\"dolar\")\n\ntext_span_2.delta_y = ap.Number(10)\ntext_span_3.delta_y = ap.Number(10)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_delta_y/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=\"#333\", stage_width=200, stage_height=80, stage_elem_id=\"stage\"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text=\"Lorem \")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text=\"ipsum \")\ntext_span_3: ap.SVGTextSpan = ap.SVGTextSpan(text=\"dolar\")\n\ntext_span_2.delta_y = ap.Number(10)\ntext_span_3.delta_y = ap.Number(10)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=\"#aaa\",\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_delta_y/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=80, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum ")\ntext_span_3: ap.SVGTextSpan = ap.SVGTextSpan(text="dolar")\n\ntext_span_2.delta_y = ap.Number(10)\ntext_span_3.delta_y = ap.Number(10)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_delta_y/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color="#333", stage_width=200, stage_height=80, stage_elem_id="stage"\n)\ntext_span_1: ap.SVGTextSpan = ap.SVGTextSpan(text="Lorem ")\ntext_span_2: ap.SVGTextSpan = ap.SVGTextSpan(text="ipsum ")\ntext_span_3: ap.SVGTextSpan = ap.SVGTextSpan(text="dolar")\n\ntext_span_2.delta_y = ap.Number(10)\ntext_span_3.delta_y = ap.Number(10)\n\nsvg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color="#aaa",\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_delta_y/")\n```',  # noqa
     ##################################################
     "## SVGTextSpan constructor API": "## SVGTextSpan クラスのコンストラクタのAPI",
     ##################################################
-    "<span class=\"inconspicuous-txt\">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>": "<span class=\"inconspicuous-txt\">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>",  # noqa
+    '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
     "The class for an SVG text-span (the child class of `SVGText`).<hr>": "`SVGText`の子となるSVGのtext-span要素のためのクラスです。<hr>",  # noqa
     ##################################################
     "**[Parameters]**": "**[引数]**",
     ##################################################
@@ -157,51 +157,51 @@
     ##################################################
     "- `line_thickness`: Optional[Union[int, Int]], optional": "- `line_thickness`: Optional[Union[int, Int]], optional",  # noqa
     ##################################################
     "  - A line-thickness (line-width) to set.": "  - 設定の線幅。",
     ##################################################
     "- `bold`: Optional[Union[bool, Boolean]], optional": "- `bold`: Optional[Union[bool, Boolean]], optional",  # noqa
     ##################################################
-    "  - A boolean, whether this text is bold style or not.": "  - テキストに太字のスタイル設定を行うかどうかの真偽値。",  # noqa
+    "  - A boolean, whether this text is a bold style or not.": "  - テキストに太字のスタイル設定を行うかどうかの真偽値。",  # noqa
     ##################################################
     "- `italic`: Optional[Union[bool, Boolean]], optional": "- `italic`: Optional[Union[bool, Boolean]], optional",  # noqa
     ##################################################
     "  - A boolean, whether a text is an italic style or not (normal).": "  - テキストを斜体表示のスタイル設定を行うかどうかの真偽値。",  # noqa
     ##################################################
     "- `delta_x`: Union[float, Number], optional": "- `delta_x`: Union[float, Number], optional",  # noqa
     ##################################################
-    "  - A coordinate delta-x setting. Notes: This setting also changes a coordinate of subsequent `SVGTextSpan`\'s instance.": "  - X座標の調整値の設定。特記事項 : この設定は後に続く`SVGTextSpan`のインスタンスの座標も変更します。",  # noqa
+    "  - A coordinate delta-x setting. Notes: This setting also changes a coordinate of subsequent `SVGTextSpan`'s instance.": "  - X座標の調整値の設定。特記事項 : この設定は後に続く`SVGTextSpan`のインスタンスの座標も変更します。",  # noqa
     ##################################################
     "- `delta_y`: Union[float, Number], optional": "- `delta_y`: Union[float, Number], optional",  # noqa
     ##################################################
-    "  - A coordinate delta-y setting. Notes: This setting also changes a coordinate of subsequent `SVGTextSpan`\'s instance.": "  - Y座標の調整値の設定。特記事項 : この設定は後に続く`SVGTextSpan`のインスタンスの座標も更新します。",  # noqa
+    "  - A coordinate delta-y setting. Notes: This setting also changes a coordinate of subsequent `SVGTextSpan`'s instance.": "  - Y座標の調整値の設定。特記事項 : この設定は後に続く`SVGTextSpan`のインスタンスの座標も更新します。",  # noqa
     ##################################################
     "- `variable_name_suffix`: str, optional": "- `variable_name_suffix`: str, optional",  # noqa
     ##################################################
     "  - A JavaScript variable name suffix string. This setting is sometimes useful for JavaScript debugging.": "  - JavaScript上の変数のサフィックスの設定です。この設定はJavaScriptのデバッグ時に役立つことがあります。",  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[Notes]**": "**[特記事項]**",
     ##################################################
     " ・If style settings are `None`, its styles inherit parent style settings.<hr>": " ・もしも各種スタイル設定に`None`が指定された場合、そのスタイルは親のスタイル設定を引き継ぎます。<hr>",  # noqa
     ##################################################
     "**[Examples]**": "**[コードサンプル]**",
     ##################################################
-    "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=\"#333\", stage_width=200, stage_height=50\n... )\n>>> svg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SVGTextSpan(text=\"Hello, \"),\n...         ap.SVGTextSpan(text=\"Hello, \", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=\"#0af\",\n... )\n```": "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=\"#333\", stage_width=200, stage_height=50\n... )\n>>> svg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SVGTextSpan(text=\"Hello, \"),\n...         ap.SVGTextSpan(text=\"Hello, \", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=\"#0af\",\n... )\n```",  # noqa
+    '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color="#333", stage_width=200, stage_height=50\n... )\n>>> svg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SVGTextSpan(text="Hello, "),\n...         ap.SVGTextSpan(text="Hello, ", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color="#0af",\n... )\n```': '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color="#333", stage_width=200, stage_height=50\n... )\n>>> svg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SVGTextSpan(text="Hello, "),\n...         ap.SVGTextSpan(text="Hello, ", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color="#0af",\n... )\n```',  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[References]**": "**[関連資料]**",
     ##################################################
     "- [SVGText class](https://simon-ritchie.github.io/apysc/en/svg_text.html)": "- [SVGText クラス](https://simon-ritchie.github.io/apysc/jp/jp_svg_text.html)",  # noqa
     ##################################################
     "## SVGText create_with_svg_text_spans class method API": "## SVGText クラスの create_with_svg_text_spans クラスメソッドのAPI",  # noqa
     ##################################################
-    "<span class=\"inconspicuous-txt\">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>": "<span class=\"inconspicuous-txt\">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>",  # noqa
+    '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
     "Create an `SVGText` instance with specified text spans.<hr>": "指定された各text spanのインスタンスを使用して`SVGText`のインスタンスを生成します。<hr>",  # noqa
     ##################################################
     "**[Parameters]**": "**[引数]**",
     ##################################################
@@ -251,15 +251,15 @@
     ##################################################
     "- `align`: SVGTextAlign, optional": "- `align`: SVGTextAlign, optional",
     ##################################################
     "  - A text-align setting for an overall text.": "  - テキスト全体に設定する行揃え設定。",
     ##################################################
     "- `bold`: Union[bool, Boolean], optional": "- `bold`: Union[bool, Boolean], optional",  # noqa
     ##################################################
-    "  - A boolean, whether this text is bold style or not.": "  - テキストに太字のスタイル設定を行うかどうかの真偽値。",  # noqa
+    "  - A boolean, whether this text is a bold style or not.": "  - テキストに太字のスタイル設定を行うかどうかの真偽値。",  # noqa
     ##################################################
     "- `italic`: Union[bool, Boolean], optional": "- `italic`: Union[bool, Boolean], optional",  # noqa
     ##################################################
     "  - A boolean, whether a text is an italic style or not (normal).": "  - テキストを斜体表示のスタイル設定を行うかどうかの真偽値。",  # noqa
     ##################################################
     "- `parent`: Optional[ChildMixIn], optional": "- `parent`: Optional[ChildMixIn], optional",  # noqa
     ##################################################
@@ -277,19 +277,19 @@
     ##################################################
     "  - A created `SVGText` instance.": "  - 生成された`SVGText`のインスタンス。",
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[Notes]**": "**[特記事項]**",
     ##################################################
-    " ・SVGText\'s y-coordinate zero-position starts at the bottom of a text. So if you set y=0, a text becomes almost invisible.<hr>": " ・SVGTextクラスの座標の0の位置はテキストの下部からスタートします。そのためもしもy=0を指定した場合、テキストはほとんど見えない状態になります。<hr>",  # noqa
+    " ・SVGText's y-coordinate zero-position starts at the bottom of a text. So if you set y=0, a text becomes almost invisible.<hr>": " ・SVGTextクラスの座標の0の位置はテキストの下部からスタートします。そのためもしもy=0を指定した場合、テキストはほとんど見えない状態になります。<hr>",  # noqa
     ##################################################
     "**[Examples]**": "**[コードサンプル]**",
     ##################################################
-    "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=\"#333\", stage_width=200, stage_height=50,\n... )\n>>> svg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SVGTextSpan(text=\"Hello, \"),\n...         ap.SVGTextSpan(text=\"Hello, \", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=\"#0af\",\n... )\n```": "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=\"#333\", stage_width=200, stage_height=50,\n... )\n>>> svg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SVGTextSpan(text=\"Hello, \"),\n...         ap.SVGTextSpan(text=\"Hello, \", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=\"#0af\",\n... )\n```",  # noqa
+    '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color="#333",\n...     stage_width=200,\n...     stage_height=50,\n... )\n>>> svg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SVGTextSpan(text="Hello, "),\n...         ap.SVGTextSpan(text="Hello, ", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color="#0af",\n... )\n```': '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color="#333",\n...     stage_width=200,\n...     stage_height=50,\n... )\n>>> svg_text: ap.SVGText = ap.SVGText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SVGTextSpan(text="Hello, "),\n...         ap.SVGTextSpan(text="Hello, ", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color="#0af",\n... )\n```',  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[References]**": "**[関連資料]**",
     ##################################################
     "- [SVGText class](https://simon-ritchie.github.io/apysc/en/svg_text.html)": "- [SVGText クラス](https://simon-ritchie.github.io/apysc/jp/jp_svg_text.html)",  # noqa
 }
```

### Comparing `apysc-2.7.9/apysc/_translation/jp/timedelta.py` & `apysc-2.8.0/apysc/_translation/jp/timedelta.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/timedelta_days.py` & `apysc-2.8.0/apysc/_translation/jp/timedelta_days.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/timedelta_total_seconds.py` & `apysc-2.8.0/apysc/_translation/jp/timedelta_total_seconds.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/timer.py` & `apysc-2.8.0/apysc/_translation/jp/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/timer_complete.py` & `apysc-2.8.0/apysc/_translation/jp/timer_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/timer_delay.py` & `apysc-2.8.0/apysc/_translation/jp/timer_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/timer_event.py` & `apysc-2.8.0/apysc/_translation/jp/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/timer_repeat_count.py` & `apysc-2.8.0/apysc/_translation/jp/timer_repeat_count.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/timer_reset.py` & `apysc-2.8.0/apysc/_translation/jp/timer_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/timer_start_and_stop.py` & `apysc-2.8.0/apysc/_translation/jp/timer_start_and_stop.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/trace.py` & `apysc-2.8.0/apysc/_translation/jp/trace.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/triangle.py` & `apysc-2.8.0/apysc/_translation/jp/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py` & `apysc-2.8.0/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/unset_debug_mode.py` & `apysc-2.8.0/apysc/_translation/jp/unset_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/variable_name_suffix.py` & `apysc-2.8.0/apysc/_translation/jp/variable_name_suffix.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/what_apysc_can_do.py` & `apysc-2.8.0/apysc/_translation/jp/what_apysc_can_do.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py` & `apysc-2.8.0/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/_delete.py` & `apysc-2.8.0/apysc/_type/_delete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/_return.py` & `apysc-2.8.0/apysc/_type/_return.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/any_value.py` & `apysc-2.8.0/apysc/_type/any_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,27 @@
 from typing_extensions import final
 
 from apysc._event.custom_event_mixin import CustomEventMixIn
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.boolean import Boolean
 from apysc._type.copy_mixin import CopyMixIn
 from apysc._type.revert_mixin import RevertMixIn
+from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._type.variable_name_mixin import VariableNameMixIn
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
-class AnyValue(CopyMixIn, RevertMixIn, CustomEventMixIn, VariableNameSuffixMixIn):
+class AnyValue(
+    ToStringMixIn,
+    CopyMixIn,
+    RevertMixIn,
+    CustomEventMixIn,
+    VariableNameSuffixMixIn,
+):
     """
     Class implementation of any value (a value that can't
     determine type).
 
     Examples
     --------
     >>> import apysc as ap
```

### Comparing `apysc-2.7.9/apysc/_type/array.py` & `apysc-2.8.0/apysc/_type/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 from apysc._type.boolean import Boolean
 from apysc._type.copy_mixin import CopyMixIn
 from apysc._type.initial_substitution_exp_mixin import InitialSubstitutionExpMixIn
 from apysc._type.int import Int
 from apysc._type.py_builtin_iter_disabling_mixin import PyBuiltInIterDisablingMixIn
 from apysc._type.revert_mixin import RevertMixIn
 from apysc._type.string import String
+from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._type.variable_name_mixin import VariableNameMixIn
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 _ArrValue = TypeVar("_ArrValue")
 
 
 class Array(
+    ToStringMixIn,
     CopyMixIn,
     RevertMixIn,
     CustomEventMixIn,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
     PyBuiltInIterDisablingMixIn,
     Generic[_ArrValue],
@@ -1158,15 +1160,15 @@
         """
         raise Exception(
             "Array instance can't apply len function."
             " Please use length property instead."
         )
 
     @final
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def join(self, sep: Union[str, String]) -> String:
         """
         Join this array value with a specified separator string.
 
         Parameters
         ----------
```

### Comparing `apysc-2.7.9/apysc/_type/attr_linking_mixin.py` & `apysc-2.8.0/apysc/_type/attr_linking_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py` & `apysc-2.8.0/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/blank_object_mixin.py` & `apysc-2.8.0/apysc/_type/blank_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/boolean.py` & `apysc-2.8.0/apysc/_type/boolean.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 
 from apysc._event.custom_event_mixin import CustomEventMixIn
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.copy_mixin import CopyMixIn
 from apysc._type.initial_substitution_exp_mixin import InitialSubstitutionExpMixIn
 from apysc._type.int import Int
 from apysc._type.revert_mixin import RevertMixIn
+from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._type.variable_name_mixin import VariableNameMixIn
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Boolean(
+    ToStringMixIn,
     CopyMixIn,
     RevertMixIn,
     CustomEventMixIn,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
 ):
     """
```

### Comparing `apysc-2.7.9/apysc/_type/copy_mixin.py` & `apysc-2.8.0/apysc/_type/copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/deleted_object_mixin.py` & `apysc-2.8.0/apysc/_type/deleted_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/dictionary.py` & `apysc-2.8.0/apysc/_type/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/expression_string.py` & `apysc-2.8.0/apysc/_type/expression_string.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/initial_substitution_exp_mixin.py` & `apysc-2.8.0/apysc/_type/initial_substitution_exp_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/int.py` & `apysc-2.8.0/apysc/_type/int.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,24 @@
 
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.number_value_mixin import NumberValueMixIn
+from apysc._type.to_fixed_mixin import ToFixedMixIn
+from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._validation import arg_validation_decos
 
 
-class Int(NumberValueMixIn[int, "Int"]):
+class Int(
+    NumberValueMixIn[int, "Int"],
+    ToStringMixIn,
+    ToFixedMixIn,
+):
     """
     Integer class for the apysc library.
 
     References
     ----------
     - Int and Number
         - https://simon-ritchie.github.io/apysc/en/int_and_number.html
@@ -44,15 +50,15 @@
     Int(20)
 
     >>> int_val = ap.Int(10.5)
     >>> int_val
     Int(10)
     """
 
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         value: Union[int, float, NumberValueMixIn],
         *,
         variable_name_suffix: str = "",
```

### Comparing `apysc-2.7.9/apysc/_type/number.py` & `apysc-2.8.0/apysc/_type/number.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,24 @@
 from typing import Any
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.number_value_mixin import NumberValueMixIn
+from apysc._type.to_fixed_mixin import ToFixedMixIn
+from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._validation import arg_validation_decos
 
 
-class Number(NumberValueMixIn[float, "Number"]):
+class Number(
+    NumberValueMixIn[float, "Number"],
+    ToStringMixIn,
+    ToFixedMixIn,
+):
     """
     Floating point number class for the apysc library.
 
     Notes
     -----
     The `Float` class is the alias of the Number,
     and it behaves the same as the Number class.
@@ -46,15 +52,15 @@
     Boolean(True)
 
     >>> number += 10.3
     >>> number
     Number(20.8)
     """
 
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         value: Union[int, float, NumberValueMixIn],
         *,
         variable_name_suffix: str = "",
@@ -128,15 +134,15 @@
             self._append_constructor_expression()
 
         self._append_initial_substitution_expression_if_in_handler_scope(
             skip_appending=skip_init_substitution_expression_appending,
         )
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     def _set_value_and_skip_expression_appending(
         self, *, value: Union[int, float, Any]
     ) -> None:
         """
         Update value attribute and skip expression appending.
 
         Parameters
```

### Comparing `apysc-2.7.9/apysc/_type/number_value_mixin.py` & `apysc-2.8.0/apysc/_type/number_value_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Generic[_ValueType, _InstanceType],
     ABC,
 ):
 
     _initial_value: _NumType
     _value: _ValueType
 
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self, *, value: _NumType, type_name: str, variable_name_suffix: str = ""
     ) -> None:
         """
         Class for number value interface.
 
@@ -126,15 +126,15 @@
         >>> int_val.value = ap.Int(30)
         >>> int_val.value
         30
         """
         return self._value
 
     @value.setter
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def value(self, value: _NumType) -> None:
         """
         Set number value.
 
         Parameters
         ----------
@@ -180,15 +180,15 @@
             right_value: Union[str, int, float] = value.variable_name
         else:
             right_value = value  # type: ignore
         expression: str = f"{self.variable_name} = {right_value};"
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __add__(self, other: _NumType) -> Any:
         """
         Method for addition.
 
         Parameters
         ----------
@@ -230,15 +230,15 @@
         right_value: str = get_value_str_for_expression(value=other)
         expression: str = (
             f"var {result.variable_name} = " f"{self.variable_name} + {right_value};"
         )
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __sub__(self, other: _NumType) -> Any:
         """
         Method for subtraction.
 
         Parameters
         ----------
@@ -280,15 +280,15 @@
         right_value: str = get_value_str_for_expression(value=other)
         expression: str = (
             f"var {result.variable_name} = " f"{self.variable_name} - {right_value};"
         )
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __mul__(self, other: _NumType) -> _InstanceType:
         """
         Method for multiplication.
 
         Parameters
         ----------
@@ -330,15 +330,15 @@
         right_value: str = get_value_str_for_expression(value=other)
         expression: str = (
             f"var {result.variable_name} = " f"{self.variable_name} * {right_value};"
         )
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __truediv__(self, other: _NumType) -> Any:
         """
         Method for true division (returns floating-point number).
 
         Parameters
         ----------
@@ -382,15 +382,15 @@
         right_value: str = get_value_str_for_expression(value=other)
         expression: str = (
             f"{result.variable_name} = {self.variable_name} / " f"{right_value};"
         )
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __floordiv__(self, other: _NumType) -> Any:
         """
         Method for floor division (return integer).
 
         Parameters
         ----------
@@ -452,15 +452,15 @@
         expression_variables_util.append_substitution_expression_with_names(
             left_variable_name=self._incremental_calc_prev_name,
             right_variable_name=self.variable_name,
         )
         self._incremental_calc_prev_name = ""
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __iadd__(self, other: _NumType) -> _InstanceType:
         """
         Method for incremental addition.
 
         Parameters
         ----------
@@ -479,15 +479,15 @@
         expression_variables_util.append_substitution_expression(
             left_value=self, right_value=result
         )
         result.variable_name = self.variable_name
         return result
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __isub__(self, other: _NumType) -> Any:
         """
         Method for incremental subtraction.
 
         Parameters
         ----------
@@ -506,15 +506,15 @@
         expression_variables_util.append_substitution_expression(
             left_value=self, right_value=result
         )
         result.variable_name = self.variable_name
         return result
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __imul__(self, other: _NumType) -> _InstanceType:
         """
         Method for incremental multiplication.
 
         Parameters
         ----------
@@ -533,15 +533,15 @@
         expression_variables_util.append_substitution_expression(
             left_value=self, right_value=result
         )
         result.variable_name = self.variable_name
         return result
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __itruediv__(self, other: _NumType) -> Any:
         """
         Method for incremental true division.
 
         Parameters
         ----------
@@ -561,15 +561,15 @@
         expression_variables_util.append_substitution_expression(
             left_value=self, right_value=result
         )
         result.variable_name = self.variable_name
         return result
 
     @final
-    @arg_validation_decos.is_num(arg_position_index=1)
+    @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __mod__(self, other: _NumType) -> _InstanceType:
         """
         Method for the modulo operation.
 
         Parameters
         ----------
```

### Comparing `apysc-2.7.9/apysc/_type/py_builtin_iter_disabling_mixin.py` & `apysc-2.8.0/apysc/_type/py_builtin_iter_disabling_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/revert_interface.py` & `apysc-2.8.0/apysc/_type/revert_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/revert_mixin.py` & `apysc-2.8.0/apysc/_type/revert_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/string.py` & `apysc-2.8.0/apysc/_type/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 from typing_extensions import final
 
 from apysc._event.custom_event_mixin import CustomEventMixIn
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._type.copy_mixin import CopyMixIn
 from apysc._type.initial_substitution_exp_mixin import InitialSubstitutionExpMixIn
 from apysc._type.revert_mixin import RevertMixIn
+from apysc._type.string_lstrip_mixin import StringLStripMixIn
 from apysc._type.string_split_mixin import StringSplitMixIn
 from apysc._type.variable_name_mixin import VariableNameMixIn
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 
 class String(
     StringSplitMixIn,
+    StringLStripMixIn,
     CopyMixIn,
     RevertMixIn,
     CustomEventMixIn,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
 ):
     """
@@ -63,15 +65,15 @@
     >>> string
     String("Hello!Hello!Hello!")
     """
 
     _initial_value: Union[str, "String"]
     _value: str
 
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @arg_validation_decos.is_builtin_string(arg_position_index=2, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
         value: Union[str, "String"],
         *,
         variable_name_suffix: str = "",
@@ -116,14 +118,15 @@
         String("Hello World!")
         """
         from apysc._expression import expression_variables_util
         from apysc._expression import var_names
         from apysc._expression.event_handler_scope import TemporaryNotHandlerScope
 
         with TemporaryNotHandlerScope():
+            value = _escape_str_value(value=value)
             self._variable_name_suffix = variable_name_suffix
             TYPE_NAME: str = var_names.STRING
             self._initial_value = value
             self._type_name = TYPE_NAME
             self._value = self._get_str_value(value=value)
             self.variable_name = expression_variables_util.get_next_variable_name(
                 type_name=TYPE_NAME
@@ -205,15 +208,15 @@
         >>> string.value = "World!"
         >>> string.value
         'World!'
         """
         return self._value
 
     @value.setter
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def value(self, value: Union[str, "String"]) -> None:
         """
         Set string value.
 
         Parameters
         ----------
@@ -245,15 +248,15 @@
         if isinstance(value, String):
             expression += f"{value.variable_name};"
         else:
             expression += f'"{value}";'
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __add__(self, other: Union[str, "String"]) -> "String":
         """
         Method for addition (string concatenation).
 
         Parameters
         ----------
@@ -351,15 +354,15 @@
             expression += f"{other}"
         expression += "; i++) {"
         expression += f"\n  {result.variable_name} += {self.variable_name};"
         expression += "\n}"
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __iadd__(self, other: Union[str, "String"]) -> Any:
         """
         Method for incremental addition (string concatenation).
 
         Parameters
         ----------
@@ -556,15 +559,15 @@
         expression: str = (
             f"{result.variable_name} = "
             f"{self.variable_name} !== {other.variable_name};"
         )
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __lt__(self, other: Union[str, Any]) -> Any:
         """
         Method for less than comparison.
 
         Parameters
         ----------
@@ -607,15 +610,15 @@
         expression: str = (
             f"{result.variable_name} = "
             f"{self.variable_name} < {other.variable_name};"
         )
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __le__(self, other: Union[str, Any]) -> Any:
         """
         Method for less than or equal comparison.
 
         Parameters
         ----------
@@ -658,15 +661,15 @@
         expression: str = (
             f"{result.variable_name} = "
             f"{self.variable_name} <= {other.variable_name};"
         )
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __gt__(self, other: Union[str, Any]) -> Any:
         """
         Method for greater than comparison.
 
         Parameters
         ----------
@@ -709,15 +712,15 @@
         expression: str = (
             f"{result.variable_name} = "
             f"{self.variable_name} > {other.variable_name};"
         )
         ap.append_js_expression(expression=expression)
 
     @final
-    @arg_validation_decos.is_string(arg_position_index=1)
+    @arg_validation_decos.is_string(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __ge__(self, other: Union[str, Any]) -> Any:
         """
         Method for greater than or equal comparison.
 
         Parameters
         ----------
@@ -827,7 +830,35 @@
             Target snapshot name.
         """
         self._value = self._get_snapshot_val_if_exists(
             current_value=self._value,
             snapshot_dict=self._value_snapshots,
             snapshot_name=snapshot_name,
         )
+
+
+def _escape_str_value(*, value: Union[str, "String"]) -> Union[str, "String"]:
+    """
+    Escape a specified string value.
+
+    Notes
+    -----
+    This function only applies to escape only when a specified value type
+    is `str`.
+
+    Parameters
+    ----------
+    value : Union[str, "String"]
+        A specified string value.
+
+    Returns
+    -------
+    value : Unjion[str, "String"]
+        An escaped string value.
+    """
+    from apysc._string import string_util
+
+    if isinstance(value, str):
+        value = string_util.escape_str(string=value)
+        return value
+
+    return value
```

### Comparing `apysc-2.7.9/apysc/_type/string_split_mixin.py` & `apysc-2.8.0/apysc/_type/string_split_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/type_util.py` & `apysc-2.8.0/apysc/_type/type_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/value_util.py` & `apysc-2.8.0/apysc/_type/value_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/variable_name_mixin.py` & `apysc-2.8.0/apysc/_type/variable_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/variable_name_suffix_attr_or_var_mixin.py` & `apysc-2.8.0/apysc/_type/variable_name_suffix_attr_or_var_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/variable_name_suffix_mixin.py` & `apysc-2.8.0/apysc/_type/variable_name_suffix_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_type/variable_name_suffix_utils.py` & `apysc-2.8.0/apysc/_type/variable_name_suffix_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_validation/arg_validation_decos.py` & `apysc-2.8.0/apysc/_validation/arg_validation_decos.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,35 @@
         is the `int` or `ap.Int`.
 - is_builtin_integer
     - Set a validation to check a specified argument's type
         is the built-in `int`.
 - is_apysc_integer
     - Set a validation to check a specified argument's type
         is the `ap.Int`.
+- is_apysc_int_or_number
+    - Set a validation to check a specified argument's type
+        is the `ap.Int` or `ap.Number`.
 - num_is_gt_zero
     - Set a validation to check that a specified argument's value
         is greater than zero.
 - num_is_gte_zero
     - Set a validation to check that a specified argument's value
         is greater than or equal to zero.
 - num_is_0_to_1_range
     - Set a validation to check that a specified argument's value
         is 0.0 to 1.0 range.
+- num_is_between
+    - Set a validation to check whether a specified argument's value
+        is between minimum and maximum values.
+- variadic_args_len_is_between
+    - Set a validation to check a variadic arguments' length is
+        a range of minimum and maximum values.
+- all_variadic_args_are_integers
+    - Set a validation to check a specified variadic arguments'
+        types are all integers.
 - is_boolean
     - Set a validation to check that a specified argument's type
         is the `bool` or `ap.Boolean`.
 - is_builtin_boolean
     - Set a validation to check that a specified argument's type
         is the built-in `bool`.
 - is_apysc_boolean
@@ -159,25 +171,35 @@
         is list of Python's str or Array of apysc's String.
 - is_svg_text_align
     - Set a validation to check a specified argument's type
         is the `SVGTextAlign`.
 - are_text_spans
     - Set a validation to check a specified argument's type
         is the list or `ap.Array` of `ap.SVGTextSpan`.
+- is_x_axis_label_position
+    - Set a validation to check a specified argument's type
+        is the `XAxisLabelPosition`.
+- is_y_axis_label_position
+    - Set a validation to check a specified argument's type
+        is the `YAxisLabelPosition`.
+- is_list_or_array_matrix_data
+    - Set a validation to check a specified argument's type
+        is list of dicts or `ap.Array` of `ap.Dictionary`.
 """
 
 import functools
 import inspect
 from inspect import Signature
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import TypeVar
+from typing import Union
 
 # pyright: reportInvalidTypeVarUse=false
 _Callable = TypeVar("_Callable", bound=Callable)
 
 
 def _extract_arg_value(
     *, args: Any, kwargs: Dict[str, Any], arg_position_index: int, callable_: Callable
@@ -439,15 +461,15 @@
     """
     Set a validation to check a specified argument's type
     is the `ap.Event` or its subclass type.
 
     Parameters
     ----------
     arg_position_index : int
-        _description_
+        A target argument position index.
 
     Returns
     -------
     wrapped : Callable
         Wrapped callable object.
     """
 
@@ -471,23 +493,26 @@
             return callable_(*args, **kwargs)
 
         return inner_wrapped  # type: ignore
 
     return wrapped  # type: ignore
 
 
-def is_num(*, arg_position_index: int) -> _Callable:
+def is_num(*, arg_position_index: int, optional: bool) -> _Callable:
     """
     Set a validation to check a specified argument's type
     is the number-related type.
 
     Parameters
     ----------
     arg_position_index : int
-        _description_
+        A target argument position index.
+    optional : bool
+        A boolean, whether a target argument accepts
+        optional None value or not.
 
     Returns
     -------
     wrapped : Callable
         Wrapped callable object.
     """
 
@@ -498,14 +523,16 @@
 
             num: Any = _extract_arg_value(
                 args=args,
                 kwargs=kwargs,
                 arg_position_index=arg_position_index,
                 callable_=callable_,
             )
+            if optional and num is None:
+                return callable_(*args, **kwargs)
 
             callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
                 callable_=callable_, arg_position_index=arg_position_index
             )
             validate_num(num=num, additional_err_msg=callable_and_arg_names_msg)
 
             return callable_(*args, **kwargs)
@@ -544,15 +571,15 @@
             )
 
             callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
                 callable_=callable_, arg_position_index=arg_position_index
             )
             if not isinstance(num, NumberValueMixIn):
                 raise TypeError(
-                    "A specified argument value is not the `ap.Int` or "
+                    "A specified argument value is not `ap.Int` or "
                     f"`ap.Number` type: {type(num)}"
                     f"\n{callable_and_arg_names_msg}"
                 )
 
             return callable_(*args, **kwargs)
 
         return inner_wrapped  # type: ignore
@@ -678,26 +705,69 @@
             )
 
             callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
                 callable_=callable_, arg_position_index=arg_position_index
             )
             if not isinstance(integer, ap.Int):
                 raise TypeError(
-                    "A specified argument value is not the `ap.Int` "
+                    "A specified argument value is not `ap.Int` "
                     f"type: {type(integer)}"
                     f"\n{callable_and_arg_names_msg}"
                 )
 
             return callable_(*args, **kwargs)
 
         return inner_wrapped  # type: ignore
 
     return wrapped  # type: ignore
 
 
+def is_apysc_int_or_number(*, arg_position_index: int) -> _Callable:
+    """
+    Set a validation to check a specified argument's type
+    is the `ap.Int` or `ap.Number`.
+
+    Parameters
+    ----------
+    arg_position_index : int
+        A target argument position index.
+
+    Returns
+    -------
+    wrapped : Callable
+        Wrapped callable object.
+    """
+
+    def wrapped(callable_: _Callable) -> _Callable:
+        @functools.wraps(callable_)
+        def inner_wrapped(*args: Any, **kwargs: Any) -> Any:
+            import apysc as ap
+
+            int_or_number: Any = _extract_arg_value(
+                args=args,
+                kwargs=kwargs,
+                arg_position_index=arg_position_index,
+                callable_=callable_,
+            )
+            if not isinstance(int_or_number, (ap.Int, ap.Number)):
+                callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
+                    callable_=callable_, arg_position_index=arg_position_index
+                )
+                raise TypeError(
+                    f"A specified argument is not `ap.Int` or `ap.Number` type: "
+                    f"{type(int_or_number).__name__}, {int_or_number}"
+                    f"\n{callable_and_arg_names_msg}"
+                )
+            return callable_(*args, **kwargs)
+
+        return inner_wrapped  # type: ignore
+
+    return wrapped  # type: ignore
+
+
 def num_is_gt_zero(*, arg_position_index: int, optional: bool) -> _Callable:
     """
     Set a validation to check that a specified argument's value
     is greater than zero.
 
     Parameters
     ----------
@@ -834,14 +904,155 @@
             return callable_(*args, **kwargs)
 
         return inner_wrapped  # type: ignore
 
     return wrapped  # type: ignore
 
 
+def num_is_between(
+    *,
+    arg_position_index: int,
+    min_value: Union[int, float],
+    max_value: Union[int, float],
+) -> _Callable:
+    """
+    Set a validation to check whether a specified argument's value
+    is between minimum and maximum values.
+
+    Notes
+    -----
+    This decorator only checks `int` and `float` values.
+
+    Parameters
+    ----------
+    arg_position_index : int
+        A target argument position index.
+    min_value : Union[int, float]
+        A minimum threshold value.
+    max_value : Union[int, float]
+        A maximum threshold value.
+
+    Returns
+    -------
+    wrapped : Callable
+        Wrapped callable object.
+    """
+
+    def wrapped(callable_: _Callable) -> _Callable:
+        @functools.wraps(callable_)
+        def inner_wrapped(*args: Any, **kwargs: Any) -> Any:
+            num: Any = _extract_arg_value(
+                args=args,
+                kwargs=kwargs,
+                arg_position_index=arg_position_index,
+                callable_=callable_,
+            )
+            if isinstance(num, (int, float)):
+                callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
+                    callable_=callable_, arg_position_index=arg_position_index
+                )
+                if num < min_value:
+                    raise ValueError(
+                        f"A specified argument value ({num}) is less than {min_value}."
+                        f"\n{callable_and_arg_names_msg}"
+                    )
+                if num > max_value:
+                    raise ValueError(
+                        f"A specified argument value ({num}) is greater than "
+                        f"{max_value}.\n{callable_and_arg_names_msg}"
+                    )
+            return callable_(*args, **kwargs)
+
+        return inner_wrapped  # type: ignore
+
+    return wrapped  # type: ignore
+
+
+def variadic_args_len_is_between(
+    *,
+    min_length: int,
+    max_length: int,
+) -> _Callable:
+    """
+    Set a validation to check a variadic arguments' length is
+    a range of minimum and maximum values.
+
+    Parameters
+    ----------
+    min_length : int
+        A minimum list length.
+    max_length : int
+        A maximum list length.
+
+    Returns
+    -------
+    wrapped : Callable
+        Wrapped callable object.
+    """
+
+    def wrapped(callable_: _Callable) -> _Callable:
+        @functools.wraps(callable_)
+        def inner_wrapped(*args: Any, **kwargs: Any) -> Any:
+            args_len: int = len(args)
+            if args_len < min_length:
+                raise ValueError(
+                    "A specified variadic argument's length is less than "
+                    f"{min_length}.\nActual length: {args_len}"
+                )
+            if args_len > max_length:
+                raise ValueError(
+                    "A specified variadic argument's length is greater than "
+                    f"{max_length}.\nActual length: {args_len}"
+                )
+
+            return callable_(*args, **kwargs)
+
+        return inner_wrapped  # type: ignore
+
+    return wrapped  # type: ignore
+
+
+def all_variadic_args_are_integers(*, optional: bool) -> _Callable:
+    """
+    Set a validation to check a specified variadic arguments'
+    types are all integers.
+
+    Parameters
+    ----------
+    optional : bool
+        A boolean, whether a target argument accepts
+        optional None value or not.
+
+    Returns
+    -------
+    wrapped : Callable
+        Wrapped callable object.
+    """
+
+    def wrapped(callable_: _Callable) -> _Callable:
+        @functools.wraps(callable_)
+        def inner_wrapped(*args: Any, **kwargs: Any) -> Any:
+            import apysc as ap
+
+            for arg in args:
+                if optional and arg is None:
+                    continue
+                if isinstance(arg, (int, ap.Int)):
+                    continue
+                raise TypeError(
+                    "A specified variadic argument value is not `int` or "
+                    f"`ap.Int`: {type(arg)}, {arg}"
+                )
+            return callable_(*args, **kwargs)
+
+        return inner_wrapped  # type: ignore
+
+    return wrapped  # type: ignore
+
+
 def is_boolean(*, arg_position_index: int, optional: bool) -> _Callable:
     """
     Set a validation to check that a specified argument's type
     is the `bool` or `ap.Boolean`.
 
     Parameters
     ----------
@@ -1012,23 +1223,26 @@
             return callable_(*args, **kwargs)
 
         return inner_wrapped  # type: ignore
 
     return wrapped  # type: ignore
 
 
-def is_string(*, arg_position_index: int) -> _Callable:
+def is_string(*, arg_position_index: int, optional: bool) -> _Callable:
     """
     Set a validation to check a specified argument's type
     is the str or `ap.String`.
 
     Parameters
     ----------
     arg_position_index : int
         A target argument position index.
+    optional : bool
+        A boolean, whether a target argument accepts
+        optional None value or not.
 
     Returns
     -------
     wrapped : Callable
         Wrapped callable object.
     """
 
@@ -1040,14 +1254,17 @@
             string: Any = _extract_arg_value(
                 args=args,
                 kwargs=kwargs,
                 arg_position_index=arg_position_index,
                 callable_=callable_,
             )
 
+            if optional and string is None:
+                return callable_(*args, **kwargs)
+
             callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
                 callable_=callable_, arg_position_index=arg_position_index
             )
             validate_string_type(
                 string=string, additional_err_msg=callable_and_arg_names_msg
             )
 
@@ -1495,15 +1712,15 @@
                 callable_=callable_,
             )
             callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
                 callable_=callable_, arg_position_index=arg_position_index
             )
             if not isinstance(points, list) and not isinstance(points, ap.Array):
                 raise TypeError(
-                    "A specified points argument type is not the list or "
+                    "A specified points argument type is not a list or "
                     f"ap.Array: {type(points)}"
                     f"\n{callable_and_arg_names_msg}"
                 )
 
             value: List[ap.Point2D] = []
             if isinstance(points, list):
                 value = points
@@ -2848,7 +3065,147 @@
                         f"\n{callable_and_arg_names_msg}"
                     )
             return callable_(*args, **kwargs)
 
         return inner_wrapped  # type: ignore
 
     return wrapped  # type: ignore
+
+
+def is_x_axis_label_position(*, arg_position_index: int) -> _Callable:
+    """
+    Set a validation to check a specified argument's type
+    is the `XAxisLabelPosition`.
+
+    Parameters
+    ----------
+    arg_position_index : int
+        A target argument position index.
+
+    Returns
+    -------
+    wrapped : Callable
+        Wrapped callable object.
+    """
+
+    def wrapped(callable_: _Callable) -> _Callable:
+        @functools.wraps(callable_)
+        def inner_wrapped(*args: Any, **kwargs: Any) -> Any:
+            import apysc as ap
+
+            x_axis_label_position: Any = _extract_arg_value(
+                args=args,
+                kwargs=kwargs,
+                arg_position_index=arg_position_index,
+                callable_=callable_,
+            )
+            if not isinstance(x_axis_label_position, ap.XAxisLabelPosition):
+                callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
+                    callable_=callable_, arg_position_index=arg_position_index
+                )
+                raise TypeError(
+                    "A specified argument is not a `XAxisLabelPosition` value: "
+                    f"{type(x_axis_label_position).__name__}, {x_axis_label_position}"
+                    f"\n{callable_and_arg_names_msg}"
+                )
+            return callable_(*args, **kwargs)
+
+        return inner_wrapped  # type: ignore
+
+    return wrapped  # type: ignore
+
+
+def is_y_axis_label_position(*, arg_position_index: int) -> _Callable:
+    """
+    Set a validation to check a specified argument's type
+    is the `YAxisLabelPosition`.
+
+    Parameters
+    ----------
+    arg_position_index : int
+        A target argument position index.
+
+    Returns
+    -------
+    wrapped : Callable
+        Wrapped callable object.
+    """
+
+    def wrapped(callable_: _Callable) -> _Callable:
+        @functools.wraps(callable_)
+        def inner_wrapped(*args: Any, **kwargs: Any) -> Any:
+            import apysc as ap
+
+            y_axis_label_position: Any = _extract_arg_value(
+                args=args,
+                kwargs=kwargs,
+                arg_position_index=arg_position_index,
+                callable_=callable_,
+            )
+            if not isinstance(y_axis_label_position, ap.YAxisLabelPosition):
+                callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
+                    callable_=callable_, arg_position_index=arg_position_index
+                )
+                raise TypeError(
+                    "A specified argument is not a `YAxisLabelPosition` value: "
+                    f"{type(y_axis_label_position).__name__}, {y_axis_label_position}"
+                    f"\n{callable_and_arg_names_msg}"
+                )
+            return callable_(*args, **kwargs)
+
+        return inner_wrapped  # type: ignore
+
+    return wrapped  # type: ignore
+
+
+def is_list_or_array_matrix_data(*, arg_position_index: int) -> _Callable:
+    """
+    Set a validation to check a specified argument's type
+    is list of dicts or `ap.Array` of `ap.Dictionary`.
+
+    Parameters
+    ----------
+    arg_position_index : int
+        A target argument position index.
+
+    Returns
+    -------
+    wrapped : Callable
+        Wrapped callable object.
+    """
+
+    def wrapped(callable_: _Callable) -> _Callable:
+        @functools.wraps(callable_)
+        def inner_wrapped(*args: Any, **kwargs: Any) -> Any:
+            import apysc as ap
+            from apysc._validation import matrix_data_validation
+
+            matrix_data: Any = _extract_arg_value(
+                args=args,
+                kwargs=kwargs,
+                arg_position_index=arg_position_index,
+                callable_=callable_,
+            )
+            callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
+                callable_=callable_, arg_position_index=arg_position_index
+            )
+            if isinstance(matrix_data, list):
+                matrix_data_validation.validate_matrix_list_data(
+                    matrix_list_data=matrix_data,
+                    additional_err_msg=callable_and_arg_names_msg,
+                )
+                return callable_(*args, **kwargs)
+            if isinstance(matrix_data, ap.Array):
+                matrix_data_validation.validate_matrix_array_data(
+                    matrix_array_data=matrix_data,
+                    additional_err_msg=callable_and_arg_names_msg,
+                )
+                return callable_(*args, **kwargs)
+            raise TypeError(
+                "A specified argument is not a list of dicts or "
+                f"`ap.Array` of `ap.Dictionary`: {type(matrix_data).__name__}, "
+                f"\n{callable_and_arg_names_msg}"
+            )
+
+        return inner_wrapped  # type: ignore
+
+    return wrapped  # type: ignore
```

### Comparing `apysc-2.7.9/apysc/_validation/bool_validation.py` & `apysc-2.8.0/apysc/_validation/bool_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
     Raises
     ------
     ValueError
         If a specified value isn't the `bool` or `Boolean` type.
     """
     from apysc._type import type_util
+    from apysc._validation import validation_common_utils
 
     is_bool: bool = type_util.is_bool(value=value)
     if is_bool:
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        f"A specified value is not the bool or Boolean type: {type(value)}"
-        f"{additional_err_msg}"
+    err_msg: str = f"A specified value is not the bool or Boolean type: {type(value)}"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_builtin_bool(*, value: bool, additional_err_msg: str = "") -> None:
     """
     Validate whether a specified value is the built-in's
     `bool` type.
 
@@ -48,14 +48,16 @@
         An additional error message to display.
 
     Raises
     ------
     ValueError
         If a specified value isn't the `bool` type.
     """
+    from apysc._validation import validation_common_utils
+
     if isinstance(value, bool):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        f"A specified value is not the bool type: {type(value)}" f"{additional_err_msg}"
+    err_msg: str = f"A specified value is not the bool type: {type(value)}"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
```

### Comparing `apysc-2.7.9/apysc/_validation/color_validation.py` & `apysc-2.8.0/apysc/_validation/handler_validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,90 @@
-"""Validations related to color.
+"""This module is for the handler interfaces'
+validation implementations.
 """
 
-from string import hexdigits
-from typing import Tuple
-from typing import TypeVar
+import inspect
+from inspect import Signature
+from typing import Any
+from typing import Callable
+from typing import List
 
-from apysc._type.string import String
 
-StrOrString = TypeVar("StrOrString", str, String)
+def validate_options_type(*, options: Any, additional_err_msg: str = "") -> None:
+    """
+    Validate a specified options type.
+
+    Parameters
+    ----------
+    options : Any
+        Target options value.
+    additional_err_msg : str, optional
+        An additional error message to display.
+
+    Raises
+    ------
+    TypeError
+        If a specified options type is not the dictionary or None.
+    """
+    from apysc._validation import validation_common_utils
+
+    if options is None:
+        return
+    if isinstance(options, dict):
+        return
+    err_msg: str = (
+        f"Handler's options argument must be a dictionary: {type(options)}"
+        f"\n{options}"
+    )
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
+    )
+    raise TypeError(err_msg)
 
 
-def validate_hex_color_code_format(
-    *, hex_color_code: StrOrString, additional_err_msg: str = ""
+def validate_handler_args_num(
+    *, handler: Callable, additional_err_msg: str = ""
 ) -> None:
     """
-    Validate a specified hexadecimal color code format.
+    Validate specified handler's arguments number.
 
     Parameters
     ----------
-    hex_color_code : str
-        Hexadecimal color code (not including '#').
-        e.g., 'ff0000', '666', '0'.
-        A blank string is also acceptable.
+    handler : Callable
+        A target handler to validate.
     additional_err_msg : str, optional
         An additional error message to display.
 
     Raises
     ------
     ValueError
-        If invalid hex color code specified.
+        - If handler's arguments number is not 2.
+    TypeError
+        - If a specified handler is not callable.
     """
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    if not isinstance(hex_color_code, (str, String)):
-        raise ValueError(
-            "Hex color code only supports str type, specified: "
-            f"{type(hex_color_code)}{additional_err_msg}"
-        )
+    from apysc._validation import validation_common_utils
 
-    if isinstance(hex_color_code, String):
-        value_: str = hex_color_code._value
-    else:
-        value_ = hex_color_code
-
-    char_len: int = len(value_)
-    expected_char_lengths: Tuple[int, int, int, int] = (0, 1, 3, 6)
-    if char_len not in expected_char_lengths:
-        raise ValueError(
-            "Not supported hex color code number of digits is specified."
-            f"\nSupported number of digits are: {expected_char_lengths}"
-            f"\nSpecified: {hex_color_code} ({char_len} digits)"
-            f"{additional_err_msg}"
+    if not callable(handler):
+        raise TypeError(
+            "A specified handler's argument is not callable: " f"{type(handler)}"
         )
-
-    for char in value_:
-        if char in hexdigits:
+    signature: Signature = inspect.signature(obj=handler)
+    args_num: int = 0
+    skipping_arg_names: List[str] = ["*", "**", "self", "cls"]
+    arg_names: List[str] = []
+    for parameter in signature.parameters:
+        if parameter in skipping_arg_names:
             continue
-        raise ValueError(
-            "Invalid hexadecimal character is specified."
-            f"\nTarget character: {char}"
-            f"\nSupported characters: {hexdigits}"
-            f"{additional_err_msg}"
+        args_num += 1
+        arg_names.append(parameter)
+    if args_num != 2:
+        err_msg: str = (
+            "A specified handler's arguments number must be 2 "
+            f"(actual: {args_num})"
+            f"\nTarget argument names: {arg_names}"
+            "\n\nThe first argument becomes event instance and the second "
+            "one becomes the handler's option parameters."
+        )
+        err_msg = validation_common_utils.append_additional_err_msg(
+            err_msg=err_msg, additional_err_msg=additional_err_msg
         )
+        raise ValueError(err_msg)
```

### Comparing `apysc-2.7.9/apysc/_validation/display_validation.py` & `apysc-2.8.0/apysc/_validation/display_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,23 +66,26 @@
     Raises
     ------
     ValueError
         If a specified instance is not `DisplayObject` type
         or its subclass type.
     """
     from apysc._display.display_object import DisplayObject
+    from apysc._validation import validation_common_utils
 
     if isinstance(display_object, DisplayObject):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
+    err_msg: str = (
         "A specified instance is not DisplayObject or it's subclass type: "
-        f"{type(display_object)}{additional_err_msg}"
+        f"{type(display_object)}"
     )
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
+    )
+    raise ValueError(err_msg)
 
 
 def validate_display_object_container(
     *, container_object: Any, additional_err_msg: str = ""
 ) -> None:
     """
     Validate whether a specified instance is a container type
@@ -97,24 +100,26 @@
 
     Raises
     ------
     ValueError
         If a specified instance is not a container type instance.
     """
     from apysc._display.child_mixin import ChildMixIn
+    from apysc._validation import validation_common_utils
 
     if isinstance(container_object, ChildMixIn):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
+    err_msg: str = (
         "A specified instance is not a container type (e.g., "
         f"`Sprite`, `Stage`) instance: {type(container_object)}"
-        f"{additional_err_msg}"
     )
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
+    )
+    raise ValueError(err_msg)
 
 
 def validate_sprite(*, sprite: Any) -> None:
     """
     Validate specified instance is Sprite type.
 
     Parameters
@@ -169,32 +174,35 @@
     Raises
     ------
     ValueError
         If a specified cap setting type is not LineCaps or not defined
         string value.
     """
     import apysc as ap
+    from apysc._validation import validation_common_utils
 
     if isinstance(cap, ap.LineCaps):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
     if isinstance(cap, ap.String):
         for line_cap in ap.LineCaps:
             if line_cap.value == cap._value:
                 return
-        raise ValueError(
+        err_msg: str = (
             f"Not defined cap string is specified: {cap}"
             "\nPlease see definitions of LineCaps."
-            f"{additional_err_msg}"
         )
-    raise ValueError(
-        f"Specified cap style type is not LineCaps or String one: {type(cap)}"
-        f"{additional_err_msg}"
+        err_msg = validation_common_utils.append_additional_err_msg(
+            err_msg=err_msg, additional_err_msg=additional_err_msg
+        )
+        raise ValueError(err_msg)
+    err_msg = f"Specified cap style type is not LineCaps or String one: {type(cap)}"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_line_joints(*, joints: Any, additional_err_msg: str = "") -> None:
     """
     Validate specified line joints style setting.
 
     Parameters
@@ -207,33 +215,38 @@
     Raises
     ------
     ValueError
         If specified joints setting type is not LineJoints or not defined
         string value.
     """
     import apysc as ap
+    from apysc._validation import validation_common_utils
 
     if isinstance(joints, ap.LineJoints):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
     if isinstance(joints, ap.String):
         for line_joints in ap.LineJoints:
             if line_joints.value == joints._value:
                 return
-        raise ValueError(
+        err_msg: str = (
             f"Not defined joints string is specified: {joints}"
-            f"\nPlease see definitions of LineJoints."
-            f"\n{additional_err_msg}"
+            "\nPlease see definitions of LineJoints."
+        )
+        err_msg = validation_common_utils.append_additional_err_msg(
+            err_msg=err_msg, additional_err_msg=additional_err_msg
         )
-    raise ValueError(
-        "Specified joints type is not LineJoints or String one: "
-        f"{type(joints)}"
-        f"\n{additional_err_msg}"
+        raise ValueError(err_msg)
+
+    err_msg = (
+        "Specified joints type is not LineJoints or String one: " f"{type(joints)}"
+    )
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_multiple_line_settings_are_not_set(
     *, any_instance: Any, additional_err_msg: str = ""
 ) -> None:
     """
     Validate that there are no multiple line settings
@@ -252,14 +265,15 @@
         If there are multiple line settings.
     """
     from apysc._display.line_dash_dot_setting_mixin import LineDashDotSettingMixIn
     from apysc._display.line_dash_setting_mixin import LineDashSettingMixIn
     from apysc._display.line_dot_setting_mixin import LineDotSettingMixIn
     from apysc._display.line_round_dot_setting_mixin import LineRoundDotSettingMixIn
     from apysc._display.line_style_mixin import LineStyleMixIn
+    from apysc._validation import validation_common_utils
 
     valid_setting_names: List[str] = []
     if isinstance(any_instance, (LineStyleMixIn, LineDotSettingMixIn)):
         if (
             hasattr(any_instance, "_line_dot_setting")
             and any_instance._line_dot_setting is not None
         ):
@@ -280,14 +294,15 @@
         if (
             hasattr(any_instance, "_line_dash_dot_setting")
             and any_instance._line_dash_dot_setting is not None
         ):
             valid_setting_names.append("LineDashDotSetting")
     if len(valid_setting_names) < 2:
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
+    err_msg: str = (
         "Multiple line settings can not be set."
         f" Current settings: {valid_setting_names}"
-        f"{additional_err_msg}"
     )
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
+    )
+    raise ValueError(err_msg)
```

### Comparing `apysc-2.7.9/apysc/_validation/event_validation.py` & `apysc-2.8.0/apysc/_validation/event_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,21 +31,23 @@
         class instance.
 
     Returns
     -------
     e : Event
         Event instance.
     """
+    from apysc._validation import validation_common_utils
+
     if isinstance(e, Event):
         return e
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        f"Specified instance is not Event type: {type(e)}" f"{additional_err_msg}"
+    err_msg: str = f"Specified instance is not Event type: {type(e)}"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_event_type(*, mouse_event_type: Any) -> MouseEventType:
     """
     Validate whether specified value is MouseEventType one or not.
 
     Parameters
```

### Comparing `apysc-2.7.9/apysc/_validation/geom_validation.py` & `apysc-2.8.0/apysc/_validation/geom_validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
     Raises
     ------
     ValueError
         If a specified value's type is not Point2D.
     """
     import apysc as ap
+    from apysc._validation import validation_common_utils
 
     if isinstance(point, ap.Point2D):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        f"Specified value's type is not Point2D: {type(point)}" f"{additional_err_msg}"
+    err_msg: str = f"Specified value's type is not Point2D: {type(point)}"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
```

### Comparing `apysc-2.7.9/apysc/_validation/handler_validation.py` & `apysc-2.8.0/apysc/_validation/color_validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,74 @@
-"""This module is for the handler interfaces'
-validation implementations.
+"""Validations related to color.
 """
 
-import inspect
-from inspect import Signature
-from typing import Any
-from typing import Callable
-from typing import List
+from string import hexdigits
+from typing import Tuple
+from typing import TypeVar
 
+from apysc._type.string import String
 
-def validate_options_type(*, options: Any, additional_err_msg: str = "") -> None:
-    """
-    Validate a specified options type.
-
-    Parameters
-    ----------
-    options : Any
-        Target options value.
-    additional_err_msg : str, optional
-        An additional error message to display.
-
-    Raises
-    ------
-    TypeError
-        If a specified options type is not the dictionary or None.
-    """
-    if options is None:
-        return
-    if isinstance(options, dict):
-        return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise TypeError(
-        f"Handler's options argument must be a dictionary: {type(options)}"
-        f"\n{options}{additional_err_msg}"
-    )
+StrOrString = TypeVar("StrOrString", str, String)
 
 
-def validate_handler_args_num(
-    *, handler: Callable, additional_err_msg: str = ""
+def validate_hex_color_code_format(
+    *, hex_color_code: StrOrString, additional_err_msg: str = ""
 ) -> None:
     """
-    Validate specified handler's arguments number.
+    Validate a specified hexadecimal color code format.
 
     Parameters
     ----------
-    handler : Callable
-        A target handler to validate.
+    hex_color_code : str
+        Hexadecimal color code (not including '#').
+        e.g., 'ff0000', '666', '0'.
+        A blank string is also acceptable.
     additional_err_msg : str, optional
         An additional error message to display.
 
     Raises
     ------
     ValueError
-        - If handler's arguments number is not 2.
-    TypeError
-        - If a specified handler is not callable.
+        If invalid hex color code specified.
     """
-    if not callable(handler):
-        raise TypeError(
-            "A specified handler's argument is not callable: " f"{type(handler)}"
-        )
-    signature: Signature = inspect.signature(obj=handler)
-    args_num: int = 0
-    skipping_arg_names: List[str] = ["*", "**", "self", "cls"]
-    arg_names: List[str] = []
-    for parameter in signature.parameters:
-        if parameter in skipping_arg_names:
+    from apysc._validation import validation_common_utils
+
+    if not isinstance(hex_color_code, (str, String)):
+        err_msg: str = (
+            "Hex color code only supports str type, specified: "
+            f"{type(hex_color_code)}"
+        )
+        err_msg = validation_common_utils.append_additional_err_msg(
+            err_msg=err_msg, additional_err_msg=additional_err_msg
+        )
+        raise ValueError(err_msg)
+
+    if isinstance(hex_color_code, String):
+        value_: str = hex_color_code._value
+    else:
+        value_ = hex_color_code
+
+    char_len: int = len(value_)
+    expected_char_lengths: Tuple[int, int, int, int] = (0, 1, 3, 6)
+    if char_len not in expected_char_lengths:
+        err_msg = (
+            "Not supported hex color code number of digits is specified."
+            f"\nSupported number of digits are: {expected_char_lengths}"
+            f"\nSpecified: {hex_color_code} ({char_len} digits)"
+        )
+        err_msg = validation_common_utils.append_additional_err_msg(
+            err_msg=err_msg, additional_err_msg=additional_err_msg
+        )
+        raise ValueError(err_msg)
+
+    for char in value_:
+        if char in hexdigits:
             continue
-        args_num += 1
-        arg_names.append(parameter)
-    if args_num != 2:
-        if additional_err_msg != "":
-            additional_err_msg = f"\n{additional_err_msg}"
-        raise ValueError(
-            "A specified handler's arguments number must be 2 "
-            f"(actual: {args_num})"
-            f"\nTarget argument names: {arg_names}"
-            "\n\nThe first argument becomes event instance and the second "
-            "one becomes the handler's option parameters."
-            f"{additional_err_msg}"
+        err_msg = (
+            "Invalid hexadecimal character is specified."
+            f"\nTarget character: {char}"
+            f"\nSupported characters: {hexdigits}"
+        )
+        err_msg = validation_common_utils.append_additional_err_msg(
+            err_msg=err_msg, additional_err_msg=additional_err_msg
         )
+        raise ValueError(err_msg)
```

### Comparing `apysc-2.7.9/apysc/_validation/number_validation.py` & `apysc-2.8.0/apysc/_validation/number_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,22 +40,25 @@
         An additional error message to display.
 
     Raises
     ------
     ValueError
         If a specified value is not an integer and float value.
     """
+    from apysc._validation import validation_common_utils
+
     if isinstance(num, (int, float, NumberValueMixIn)):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        f"Specified value is not iteger or float type: {num}"
-        f"({type(num)}){additional_err_msg}"
+    err_msg: str = (
+        f"Specified value is not iteger or float type: {num}" f"({type(num)})"
+    )
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_integer(*, integer: Union[int, Int], additional_err_msg: str = "") -> None:
     """
     Validate whether a specified value is an integer or not.
 
     Parameters
@@ -66,22 +69,23 @@
         An additional error message to display.
 
     Raises
     ------
     ValueError
         If a specified value is not an integer.
     """
+    from apysc._validation import validation_common_utils
+
     if isinstance(integer, (int, Int)):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        f"A specified value is not an integer: {integer}({type(integer)})"
-        f"{additional_err_msg}"
+    err_msg: str = f"A specified value is not an integer: {integer}({type(integer)})"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_builtin_integer(*, integer: int, additional_err_msg: str = "") -> None:
     """
     Validate whether a specified value is a built-in integer or not.
 
     Parameters
@@ -92,23 +96,25 @@
         An additional error message to display.
 
     Raises
     ------
     ValueError
         If a specified value is not a built-in integer.
     """
+    from apysc._validation import validation_common_utils
+
     if isinstance(integer, int):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        "A specified value is not a built-in integer: "
-        f"{integer}({type(integer)})"
-        f"{additional_err_msg}"
+    err_msg: str = (
+        "A specified value is not a built-in integer: " f"{integer}({type(integer)})"
+    )
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_int_is_zero_or_one(*, integer: Union[int, Int]) -> None:
     """
     Validate specified integer value is zero or one.
 
     Notes
@@ -151,24 +157,26 @@
         An additional error message to display.
 
     Raises
     ------
     ValueError
         If a specified value is less than or equal to zero.
     """
+    from apysc._validation import validation_common_utils
+
     if isinstance(num, NumberValueMixIn):
         if num._value > 0:
             return
     elif num > 0:
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        f"Specified values is less than or equal to zero: {num}" f"{additional_err_msg}"
+    err_msg: str = f"Specified values is less than or equal to zero: {num}"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_num_is_gte_zero(
     *, num: Union[int, float, Int, Number], additional_err_msg: str = ""
 ) -> None:
     """
     Validate whether a specified value is greater than or equal to zero.
@@ -181,22 +189,26 @@
         An additional error message to display.
 
     Raises
     ------
     ValueError
         If a specified value is less than zero.
     """
+    from apysc._validation import validation_common_utils
+
     if isinstance(num, NumberValueMixIn):
         if num._value >= 0:
             return
     elif num >= 0:
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(f"Specified values is less than zero: {num}{additional_err_msg}")
+    err_msg: str = f"Specified values is less than zero: {num}"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
+    )
+    raise ValueError(err_msg)
 
 
 def validate_num_is_0_to_1_range(
     *, num: Union[float, NumberValueMixIn], additional_err_msg: str = ""
 ) -> None:
     """
     Validate whether a specified number is from 0.0 to 1.0.
@@ -209,21 +221,37 @@
         An additional error message to display.
 
     Raises
     ------
     ValueError
         If a specified opacity is out of the 0.0 to 1.0 range.
     """
+    from apysc._validation import validation_common_utils
+
     lt_err_msg: str = "Can't specify number value less than 0.0: "
     gt_err_msg: str = "Can't specify number value greater than 1.0: "
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
     if isinstance(num, NumberValueMixIn):
         if num._value < 0.0:
-            raise ValueError(f"{lt_err_msg}{num}{additional_err_msg}")
+            err_msg: str = f"{lt_err_msg}{num}"
+            err_msg = validation_common_utils.append_additional_err_msg(
+                err_msg=err_msg, additional_err_msg=additional_err_msg
+            )
+            raise ValueError(err_msg)
         if num._value > 1.0:
-            raise ValueError(f"{gt_err_msg}{num}{additional_err_msg}")
+            err_msg = f"{gt_err_msg}{num}"
+            err_msg = validation_common_utils.append_additional_err_msg(
+                err_msg=err_msg, additional_err_msg=additional_err_msg
+            )
+            raise ValueError(err_msg)
     else:
         if num < 0.0:
-            raise ValueError(f"{lt_err_msg}{num}{additional_err_msg}")
+            err_msg = f"{lt_err_msg}{num}"
+            err_msg = validation_common_utils.append_additional_err_msg(
+                err_msg=err_msg, additional_err_msg=additional_err_msg
+            )
+            raise ValueError(err_msg)
         if num > 1.0:
-            raise ValueError(f"{gt_err_msg}{num}{additional_err_msg}")
+            err_msg = f"{gt_err_msg}{num}"
+            err_msg = validation_common_utils.append_additional_err_msg(
+                err_msg=err_msg, additional_err_msg=additional_err_msg
+            )
+            raise ValueError(err_msg)
```

### Comparing `apysc-2.7.9/apysc/_validation/parent_validation.py` & `apysc-2.8.0/apysc/_validation/parent_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_validation/path_validation.py` & `apysc-2.8.0/apysc/_validation/path_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.7.9/apysc/_validation/string_validation.py` & `apysc-2.8.0/apysc/_validation/string_validation.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,23 +20,25 @@
         An additional error message to display.
 
     Raises
     ------
     ValueError
         - If a non-string value is specified.
     """
+    from apysc._validation import validation_common_utils
+
     if isinstance(string, str):
         return
     if isinstance(string, String):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        f"A specified value is not str type: {type(string)}" f"{additional_err_msg}"
+    err_msg: str = f"A specified value is not str type: {type(string)}"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_builtin_string_type(*, string: str, additional_err_msg: str = "") -> None:
     """
     Validate a specified string's type is Python built-in's str.
 
     Parameters
@@ -47,21 +49,23 @@
         An additional error message to display.
 
     Raises
     ------
     ValueError
         - If a non-string value is specified.
     """
+    from apysc._validation import validation_common_utils
+
     if isinstance(string, str):
         return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(
-        f"A specified value is not str type: {type(string)}" f"{additional_err_msg}"
+    err_msg: str = f"A specified value is not str type: {type(string)}"
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
     )
+    raise ValueError(err_msg)
 
 
 def validate_not_empty_string(
     *, string: Union[str, String], additional_err_msg: str = ""
 ) -> None:
     """
     Validate whether a specified string is not empty.
@@ -75,17 +79,21 @@
 
     Raises
     ------
     ValueError
         - If empty string ('' or "") is specified.
         - If specified value is not str type.
     """
+    from apysc._validation import validation_common_utils
+
     validate_string_type(string=string)
     if isinstance(string, str):
         if string != "":
             return
     elif isinstance(string, String):
         if string._value != "":
             return
-    if additional_err_msg != "":
-        additional_err_msg = f"\n{additional_err_msg}"
-    raise ValueError(f"Empty string is not acceptable.{additional_err_msg}")
+    err_msg: str = "Empty string is not acceptable."
+    err_msg = validation_common_utils.append_additional_err_msg(
+        err_msg=err_msg, additional_err_msg=additional_err_msg
+    )
+    raise ValueError(err_msg)
```

### Comparing `apysc-2.7.9/apysc.egg-info/PKG-INFO` & `apysc-2.8.0/apysc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 2.7.9
+Version: 2.8.0
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-2.7.9/apysc.egg-info/SOURCES.txt` & `apysc-2.8.0/apysc.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -57,21 +57,76 @@
 apysc/_animation/animation_width_for_ellipse_mixin.py
 apysc/_animation/animation_width_mixin.py
 apysc/_animation/animation_x.py
 apysc/_animation/animation_x_mixin.py
 apysc/_animation/animation_y.py
 apysc/_animation/animation_y_mixin.py
 apysc/_animation/easing.py
+apysc/_auto_reloading/__init__.py
+apysc/_auto_reloading/auto_reloading_decorator.py
 apysc/_branch/__init__.py
 apysc/_branch/_elif.py
 apysc/_branch/_else.py
 apysc/_branch/_if.py
 apysc/_branch/if_base.py
 apysc/_callable/__init__.py
 apysc/_callable/callable_util.py
+apysc/_chart/__init__.py
+apysc/_chart/add_background_mixin.py
+apysc/_chart/add_border_mixin.py
+apysc/_chart/axis_label_bold_mixin.py
+apysc/_chart/axis_label_fill_alpha_mixin.py
+apysc/_chart/axis_label_fill_color_mixin.py
+apysc/_chart/axis_label_font_family_mixin.py
+apysc/_chart/axis_label_font_size_mixin.py
+apysc/_chart/axis_label_italic_mixin.py
+apysc/_chart/axis_line_alpha_mixin.py
+apysc/_chart/axis_line_color_mixin.py
+apysc/_chart/axis_line_thickness_mixin.py
+apysc/_chart/background_container_mixin.py
+apysc/_chart/border_container_mixin.py
+apysc/_chart/chart_const.py
+apysc/_chart/chart_container_mixin.py
+apysc/_chart/create_single_column_y_axis_mixin.py
+apysc/_chart/initialize_each_container_mixin.py
+apysc/_chart/is_display_axis_label_mixin.py
+apysc/_chart/overall_container_mixin.py
+apysc/_chart/set_initial_background_fill_alpha_mixin.py
+apysc/_chart/set_initial_background_fill_color_mixin.py
+apysc/_chart/set_initial_border_alpha_mixin.py
+apysc/_chart/set_initial_border_color_mixin.py
+apysc/_chart/set_initial_border_thickness_mixin.py
+apysc/_chart/set_initial_height_mixin.py
+apysc/_chart/set_initial_horizontal_padding_mixin.py
+apysc/_chart/set_initial_matrix_data_mixin.py
+apysc/_chart/set_initial_overall_container_coordinates_mixin.py
+apysc/_chart/set_initial_vertical_padding_mixin.py
+apysc/_chart/set_initial_width_mixin.py
+apysc/_chart/set_initial_x_mixin.py
+apysc/_chart/set_initial_y_mixin.py
+apysc/_chart/tick_max_num_mixin.py
+apysc/_chart/tick_text_bold_mixin.py
+apysc/_chart/tick_text_fill_alpha_mixin.py
+apysc/_chart/tick_text_fill_color_mixin.py
+apysc/_chart/tick_text_font_family_mixin.py
+apysc/_chart/tick_text_font_size_mixin.py
+apysc/_chart/tick_text_italic_mixin.py
+apysc/_chart/vertical_bar_chart.py
+apysc/_chart/x_axis_column_name_mixin.py
+apysc/_chart/x_axis_container_mixin.py
+apysc/_chart/x_axis_label_position.py
+apysc/_chart/x_axis_label_position_mixin.py
+apysc/_chart/x_axis_settings.py
+apysc/_chart/y_axis_column_name_mixin.py
+apysc/_chart/y_axis_container_mixin.py
+apysc/_chart/y_axis_label_position.py
+apysc/_chart/y_axis_label_position_mixin.py
+apysc/_chart/y_axis_single_column_settings.py
+apysc/_chart/y_max_mixin.py
+apysc/_chart/y_min_mixin.py
 apysc/_color/__init__.py
 apysc/_color/color_util.py
 apysc/_console/__init__.py
 apysc/_console/_trace.py
 apysc/_console/assertion.py
 apysc/_console/loggers.py
 apysc/_converter/__init__.py
@@ -90,26 +145,28 @@
 apysc/_display/append_line_point_mixin.py
 apysc/_display/append_line_thickness_attr_expression_mixin.py
 apysc/_display/append_x_attr_expression_mixin.py
 apysc/_display/append_y_attr_expression_mixin.py
 apysc/_display/begin_fill_mixin.py
 apysc/_display/child_mixin.py
 apysc/_display/circle.py
+apysc/_display/css_interface.py
 apysc/_display/css_mixin.py
 apysc/_display/cx_mixin.py
 apysc/_display/cy_mixin.py
 apysc/_display/display_object.py
 apysc/_display/ellipse.py
 apysc/_display/ellipse_height_mixin.py
 apysc/_display/ellipse_width_mixin.py
 apysc/_display/fill_alpha_mixin.py
 apysc/_display/fill_color_mixin.py
 apysc/_display/flip_interface_helper.py
 apysc/_display/flip_x_mixin.py
 apysc/_display/flip_y_mixin.py
+apysc/_display/get_bounds_mixin.py
 apysc/_display/graphics.py
 apysc/_display/graphics_base.py
 apysc/_display/graphics_clear_mixin.py
 apysc/_display/graphics_expression.py
 apysc/_display/height_mixin.py
 apysc/_display/line.py
 apysc/_display/line_alpha_mixin.py
@@ -149,14 +206,15 @@
 apysc/_display/rotation_interface_helper.py
 apysc/_display/scale_interface_helper.py
 apysc/_display/scale_x_from_center_mixin.py
 apysc/_display/scale_x_from_point_mixin.py
 apysc/_display/scale_y_from_center_mixin.py
 apysc/_display/scale_y_from_point_mixin.py
 apysc/_display/set_lower_scale_limit_mixin.py
+apysc/_display/set_overflow_visible_setting_mixin.py
 apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
 apysc/_display/skew_x_mixin.py
 apysc/_display/skew_y_mixin.py
 apysc/_display/sprite.py
 apysc/_display/stage.py
 apysc/_display/svg_text.py
 apysc/_display/svg_text_align_mixin.py
@@ -251,14 +309,23 @@
 apysc/_geom/path_label.py
 apysc/_geom/path_line_to.py
 apysc/_geom/path_move_to.py
 apysc/_geom/path_vertical.py
 apysc/_geom/path_x_mixin.py
 apysc/_geom/path_y_mixin.py
 apysc/_geom/point2d.py
+apysc/_geom/rectangle_geom.py
+apysc/_geom/rectangle_geom_bottom_y_mixin.py
+apysc/_geom/rectangle_geom_center_x_mixin.py
+apysc/_geom/rectangle_geom_center_y_mixin.py
+apysc/_geom/rectangle_geom_height_mixin.py
+apysc/_geom/rectangle_geom_left_x_mixin.py
+apysc/_geom/rectangle_geom_right_x_mixin.py
+apysc/_geom/rectangle_geom_top_y_mixin.py
+apysc/_geom/rectangle_geom_width_mixin.py
 apysc/_geom/relative_mixin.py
 apysc/_html/__init__.py
 apysc/_html/debug_mode.py
 apysc/_html/exporter.py
 apysc/_html/html_const.py
 apysc/_html/html_util.py
 apysc/_jslib/__init__.py
@@ -284,14 +351,15 @@
 apysc/_lint_and_doc/translation_mapping_utils.py
 apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
 apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
 apysc/_lint_and_doc/fixed_translation_mapping/jp.py
 apysc/_loop/__init__.py
 apysc/_loop/_continue.py
 apysc/_loop/_for.py
+apysc/_loop/_range.py
 apysc/_loop/loop_count.py
 apysc/_math/__init__.py
 apysc/_math/math.py
 apysc/_math/max_mixin.py
 apysc/_math/min_mixin.py
 apysc/_math/trunc_mixin.py
 apysc/_string/__init__.py
@@ -414,14 +482,15 @@
 apysc/_translation/jp/ellipse.py
 apysc/_translation/jp/else.py
 apysc/_translation/jp/enter_frame.py
 apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
 apysc/_translation/jp/for.py
 apysc/_translation/jp/fps.py
 apysc/_translation/jp/fundamental_data_classes_value_interface.py
+apysc/_translation/jp/get_bounds.py
 apysc/_translation/jp/get_child_at.py
 apysc/_translation/jp/graphics.py
 apysc/_translation/jp/graphics_base_fill_alpha.py
 apysc/_translation/jp/graphics_base_fill_color.py
 apysc/_translation/jp/graphics_base_flip_interfaces.py
 apysc/_translation/jp/graphics_base_line_alpha.py
 apysc/_translation/jp/graphics_base_line_color.py
@@ -453,14 +522,15 @@
 apysc/_translation/jp/graphics_move_to_and_line_to.py
 apysc/_translation/jp/if.py
 apysc/_translation/jp/import_conventions.py
 apysc/_translation/jp/index.py
 apysc/_translation/jp/int_and_number.py
 apysc/_translation/jp/int_and_number_arithmetic_operations.py
 apysc/_translation/jp/int_and_number_comparison_operations.py
+apysc/_translation/jp/int_and_number_to_fixed.py
 apysc/_translation/jp/line.py
 apysc/_translation/jp/math_max.py
 apysc/_translation/jp/math_min.py
 apysc/_translation/jp/math_trunc.py
 apysc/_translation/jp/mouse_event_abstract.py
 apysc/_translation/jp/mouse_event_basic.py
 apysc/_translation/jp/mousedown_and_mouseup.py
@@ -477,16 +547,18 @@
 apysc/_translation/jp/path_line_to.py
 apysc/_translation/jp/path_move_to.py
 apysc/_translation/jp/path_vertical.py
 apysc/_translation/jp/point2d.py
 apysc/_translation/jp/polygon.py
 apysc/_translation/jp/polyline.py
 apysc/_translation/jp/quick_start.py
+apysc/_translation/jp/range.py
 apysc/_translation/jp/recommended_type_checker_settings.py
 apysc/_translation/jp/rectangle.py
+apysc/_translation/jp/rectangle_geom.py
 apysc/_translation/jp/remove_children.py
 apysc/_translation/jp/return.py
 apysc/_translation/jp/save_overall_html.py
 apysc/_translation/jp/sequential_animation.py
 apysc/_translation/jp/set_debug_mode.py
 apysc/_translation/jp/sprite.py
 apysc/_translation/jp/stage.py
@@ -502,14 +574,15 @@
 apysc/_translation/jp/timer.py
 apysc/_translation/jp/timer_complete.py
 apysc/_translation/jp/timer_delay.py
 apysc/_translation/jp/timer_event.py
 apysc/_translation/jp/timer_repeat_count.py
 apysc/_translation/jp/timer_reset.py
 apysc/_translation/jp/timer_start_and_stop.py
+apysc/_translation/jp/to_string.py
 apysc/_translation/jp/trace.py
 apysc/_translation/jp/triangle.py
 apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
 apysc/_translation/jp/unset_debug_mode.py
 apysc/_translation/jp/variable_name_suffix.py
 apysc/_translation/jp/what_apysc_can_do.py
 apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
@@ -528,18 +601,22 @@
 apysc/_type/dictionary_structure.py
 apysc/_type/expression_string.py
 apysc/_type/initial_substitution_exp_mixin.py
 apysc/_type/int.py
 apysc/_type/number.py
 apysc/_type/number_value_mixin.py
 apysc/_type/py_builtin_iter_disabling_mixin.py
+apysc/_type/repr_interface.py
 apysc/_type/revert_interface.py
 apysc/_type/revert_mixin.py
 apysc/_type/string.py
+apysc/_type/string_lstrip_mixin.py
 apysc/_type/string_split_mixin.py
+apysc/_type/to_fixed_mixin.py
+apysc/_type/to_string_mixin.py
 apysc/_type/type_name_mixin.py
 apysc/_type/type_util.py
 apysc/_type/value_util.py
 apysc/_type/variable_name_mixin.py
 apysc/_type/variable_name_suffix_attr_or_var_mixin.py
 apysc/_type/variable_name_suffix_mixin.py
 apysc/_type/variable_name_suffix_utils.py
@@ -547,12 +624,14 @@
 apysc/_validation/arg_validation_decos.py
 apysc/_validation/bool_validation.py
 apysc/_validation/color_validation.py
 apysc/_validation/display_validation.py
 apysc/_validation/event_validation.py
 apysc/_validation/geom_validation.py
 apysc/_validation/handler_validation.py
+apysc/_validation/matrix_data_validation.py
 apysc/_validation/number_validation.py
 apysc/_validation/parent_validation.py
 apysc/_validation/path_validation.py
 apysc/_validation/string_validation.py
+apysc/_validation/validation_common_utils.py
 apysc/_validation/variable_name_validation.py
```

