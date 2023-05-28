# Comparing `tmp/bigtree-0.9.2.tar.gz` & `tmp/bigtree-0.9.3.tar.gz`

## Comparing `bigtree-0.9.2.tar` & `bigtree-0.9.3.tar`

### file list

```diff
@@ -1,106 +1,107 @@
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bigtree-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 bigtree-0.9.2/.readthedocs.yaml
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bigtree-0.9.2/CHANGELOG.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bigtree-0.9.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bigtree-0.9.2/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bigtree-0.9.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bigtree-0.9.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bigtree-0.9.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   757076 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/DejaVuSans.ttf
--rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/binarytree.png
--rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/custom_tree.png
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/dag_construct.png
--rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo.png
--rw-r--r--   0        0        0    17554 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo_binarytree.png
--rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo_dag.png
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo_pillow.png
--rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/demo_tree.png
--rw-r--r--   0        0        0   313013 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/modify_advanced.png
--rw-r--r--   0        0        0   180588 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/modify_shift_and_copy.png
--rw-r--r--   0        0        0    67777 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/tree_construct.png
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 bigtree-0.9.2/assets/weighted_tree.png
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/py.typed
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/binarytree/construct.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/dag/__init__.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/dag/construct.py
--rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/dag/export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/__init__.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/basenode.py
--rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/binarynode.py
--rw-r--r--   0        0        0    18189 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/dagnode.py
--rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/node/node.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/__init__.py
--rw-r--r--   0        0        0    33732 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/construct.py
--rw-r--r--   0        0        0    30233 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/export.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/helper.py
--rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/modify.py
--rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/tree/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/utils/__init__.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/utils/exceptions.py
--rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/utils/iterators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/workflows/__init__.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/workflows/app_calendar.py
--rw-r--r--   0        0        0     8516 2020-02-02 00:00:00.000000 bigtree-0.9.2/bigtree/workflows/app_todo.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/make.bat
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/requirements.txt
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/binarytree.rst
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/conf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/dag.rst
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/node.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/tree.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/utils.rst
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/workflows.rst
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/_static/custom.css
--rw-r--r--   0        0        0    27138 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/_templates/layout.html
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/binarytree/construct.rst
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/dag/construct.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/dag/export.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/node/basenode.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/node/binarynode.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/node/dagnode.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/node/node.rst
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/construct.rst
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/export.rst
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/helper.rst
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/modify.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/tree/search.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/utils/iterators.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/bigtree/workflows/app_todo.rst
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/contributing.rst
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/list_dir.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/merging_trees.md
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/nodes.md
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/tips.rst
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bigtree-0.9.2/docs/source/others/weighted_trees.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/__init__.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/test_construct.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/test_export.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/test_helper.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/binarytree/test_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/dag/__init__.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/dag/test_construct.py
--rw-r--r--   0        0        0    13410 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/dag/test_export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/__init__.py
--rw-r--r--   0        0        0    31896 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/test_basenode.py
--rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/test_binarynode.py
--rw-r--r--   0        0        0    31052 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/test_dagnode.py
--rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/node/test_node.py
--rw-r--r--   0        0        0    57110 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_construct.py
--rw-r--r--   0        0        0    36938 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_export.py
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_helper.py
--rw-r--r--   0        0        0    67770 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_modify.py
--rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/tree/test_search.py
--rw-r--r--   0        0        0    13545 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/utils/test_iterators.py
--rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 bigtree-0.9.2/tests/workflows/test_todo.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bigtree-0.9.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bigtree-0.9.2/LICENSE
--rw-r--r--   0        0        0    25288 2020-02-02 00:00:00.000000 bigtree-0.9.2/README.md
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 bigtree-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    26396 2020-02-02 00:00:00.000000 bigtree-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bigtree-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 bigtree-0.9.3/.readthedocs.yaml
+-rw-r--r--   0        0        0    12475 2020-02-02 00:00:00.000000 bigtree-0.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bigtree-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bigtree-0.9.3/SECURITY.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bigtree-0.9.3/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bigtree-0.9.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bigtree-0.9.3/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bigtree-0.9.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   757076 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/DejaVuSans.ttf
+-rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/binarytree.png
+-rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/custom_tree.png
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/dag_construct.png
+-rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo.png
+-rw-r--r--   0        0        0    17554 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo_binarytree.png
+-rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo_dag.png
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo_pillow.png
+-rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo_tree.png
+-rw-r--r--   0        0        0   313013 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/modify_advanced.png
+-rw-r--r--   0        0        0   180588 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/modify_shift_and_copy.png
+-rw-r--r--   0        0        0    67777 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/tree_construct.png
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/weighted_tree.png
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/py.typed
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/binarytree/construct.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/dag/__init__.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/dag/construct.py
+-rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/dag/export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/__init__.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/basenode.py
+-rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/binarynode.py
+-rw-r--r--   0        0        0    18189 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/dagnode.py
+-rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/node.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/__init__.py
+-rw-r--r--   0        0        0    33748 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/construct.py
+-rw-r--r--   0        0        0    30233 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/export.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/helper.py
+-rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/modify.py
+-rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/utils/__init__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/utils/exceptions.py
+-rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/utils/iterators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/workflows/__init__.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/workflows/app_calendar.py
+-rw-r--r--   0        0        0     8516 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/workflows/app_todo.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/make.bat
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/requirements.txt
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/binarytree.rst
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/conf.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/dag.rst
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/node.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/tree.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/utils.rst
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/workflows.rst
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/_static/custom.css
+-rw-r--r--   0        0        0    27138 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/_templates/layout.html
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/binarytree/construct.rst
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/dag/construct.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/dag/export.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/node/basenode.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/node/binarynode.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/node/dagnode.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/node/node.rst
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/construct.rst
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/export.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/helper.rst
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/modify.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/search.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/utils/iterators.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/workflows/app_todo.rst
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/contributing.rst
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/list_dir.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/merging_trees.md
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/nodes.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/tips.rst
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/weighted_trees.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/__init__.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/test_construct.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/test_export.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/test_helper.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/test_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/dag/__init__.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/dag/test_construct.py
+-rw-r--r--   0        0        0    13410 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/dag/test_export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/__init__.py
+-rw-r--r--   0        0        0    31896 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/test_basenode.py
+-rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/test_binarynode.py
+-rw-r--r--   0        0        0    31052 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/test_dagnode.py
+-rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/test_node.py
+-rw-r--r--   0        0        0    57110 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_construct.py
+-rw-r--r--   0        0        0    36938 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_export.py
+-rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_helper.py
+-rw-r--r--   0        0        0    67770 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_modify.py
+-rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_search.py
+-rw-r--r--   0        0        0    13545 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/utils/test_iterators.py
+-rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/workflows/test_todo.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bigtree-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bigtree-0.9.3/LICENSE
+-rw-r--r--   0        0        0    25288 2020-02-02 00:00:00.000000 bigtree-0.9.3/README.md
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 bigtree-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    26396 2020-02-02 00:00:00.000000 bigtree-0.9.3/PKG-INFO
```

### Comparing `bigtree-0.9.2/.pre-commit-config.yaml` & `bigtree-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/CHANGELOG.md` & `bigtree-0.9.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.3] - 2023-05-28
+### Modified
+- Tree Constructor: Relax type hint to `Iterable` instead of `List` for `list_to_tree` and `list_to_tree_by_relation` methods.
+### Fixed
+- Node: Fix error message when trees have different `sep`.
+
 ## [0.9.2] - 2023-04-09
 ### Added
 - Node: Added `show` method to print tree to console.
 - Workflow Calendar: Tree use case with calendar implementation.
 
 ## [0.9.1] - 2023-03-30
 ### Changed
@@ -252,14 +258,15 @@
 - Tree Exporter: To list, nested dictionary, pandas DataFrame.
 - Tree Helper: Cloning, pruning trees, get difference between two trees.
 - Tree Modifier: Shift and copy nodes within tree and between trees.
 - Tree Search: Find single or multiple nodes based on name, attribute, or custom criteria.
 - Utility Iterator: Tree traversal methods.
 - Workflow To Do App: Tree use case with to-do list implementation.
 
+[0.9.3]: https://github.com/kayjan/bigtree/compare/v0.9.2...v0.9.3
 [0.9.2]: https://github.com/kayjan/bigtree/compare/v0.9.1...v0.9.2
 [0.9.1]: https://github.com/kayjan/bigtree/compare/v0.9.0...v0.9.1
 [0.9.0]: https://github.com/kayjan/bigtree/compare/v0.8.4...v0.9.0
 [0.8.4]: https://github.com/kayjan/bigtree/compare/v0.8.3...v0.8.4
 [0.8.3]: https://github.com/kayjan/bigtree/compare/v0.8.2...v0.8.3
 [0.8.2]: https://github.com/kayjan/bigtree/compare/v0.8.1...v0.8.2
 [0.8.1]: https://github.com/kayjan/bigtree/compare/v0.8.0...v0.8.1
```

### Comparing `bigtree-0.9.2/.github/workflows/codecov.yml` & `bigtree-0.9.3/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/.github/workflows/docs.yml` & `bigtree-0.9.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/.github/workflows/pytest.yml` & `bigtree-0.9.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/.github/workflows/python-publish.yml` & `bigtree-0.9.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/DejaVuSans.ttf` & `bigtree-0.9.3/assets/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/binarytree.png` & `bigtree-0.9.3/assets/binarytree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/custom_tree.png` & `bigtree-0.9.3/assets/custom_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/dag_construct.png` & `bigtree-0.9.3/assets/dag_construct.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/demo.png` & `bigtree-0.9.3/assets/demo.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/demo_binarytree.png` & `bigtree-0.9.3/assets/demo_binarytree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/demo_dag.png` & `bigtree-0.9.3/assets/demo_dag.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/demo_pillow.png` & `bigtree-0.9.3/assets/demo_pillow.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/demo_tree.png` & `bigtree-0.9.3/assets/demo_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/modify_advanced.png` & `bigtree-0.9.3/assets/modify_advanced.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/modify_shift_and_copy.png` & `bigtree-0.9.3/assets/modify_shift_and_copy.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/tree_construct.png` & `bigtree-0.9.3/assets/tree_construct.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/assets/weighted_tree.png` & `bigtree-0.9.3/assets/weighted_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/__init__.py` & `bigtree-0.9.3/bigtree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 from bigtree.binarytree.construct import list_to_binarytree
 from bigtree.dag.construct import dataframe_to_dag, dict_to_dag, list_to_dag
 from bigtree.dag.export import dag_to_dataframe, dag_to_dict, dag_to_dot, dag_to_list
 from bigtree.node.basenode import BaseNode
 from bigtree.node.binarynode import BinaryNode
 from bigtree.node.dagnode import DAGNode
```

### Comparing `bigtree-0.9.2/bigtree/binarytree/construct.py` & `bigtree-0.9.3/bigtree/binarytree/construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/dag/construct.py` & `bigtree-0.9.3/bigtree/dag/construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/dag/export.py` & `bigtree-0.9.3/bigtree/dag/export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/node/basenode.py` & `bigtree-0.9.3/bigtree/node/basenode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/node/binarynode.py` & `bigtree-0.9.3/bigtree/node/binarynode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/node/dagnode.py` & `bigtree-0.9.3/bigtree/node/dagnode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/node/node.py` & `bigtree-0.9.3/bigtree/node/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         if new_parent is not None:
             if any(
                 child.node_name == self.node_name and child is not self
                 for child in new_parent.children
             ):
                 raise TreeError(
                     f"Error: Duplicate node with same path\n"
-                    f"There exist a node with same path {new_parent.path_name}{self.sep}{self.node_name}"
+                    f"There exist a node with same path {new_parent.path_name}{new_parent.sep}{self.node_name}"
                 )
 
     def _BaseNode__post_assign_parent(self: T, new_parent: T) -> None:
         """No rules
 
         Args:
             new_parent (Self): new parent to be added
```

### Comparing `bigtree-0.9.2/bigtree/tree/construct.py` & `bigtree-0.9.3/bigtree/tree/construct.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from collections import OrderedDict
-from typing import Any, Dict, List, Optional, Tuple, Type
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Type
 
 import pandas as pd
 
 from bigtree.node.node import Node
 from bigtree.tree.export import tree_to_dataframe
 from bigtree.tree.search import find_child_by_name, find_name
 from bigtree.utils.exceptions import DuplicatedNodeError, TreeError
@@ -476,15 +476,15 @@
         child_node.parent = cur_parent
         cur_parent = child_node
 
     return tree_root
 
 
 def list_to_tree(
-    paths: List[str],
+    paths: Iterable[str],
     sep: str = "/",
     duplicate_name_allowed: bool = True,
     node_type: Type[Node] = Node,
 ) -> Node:
     """Construct tree from list of path strings.
 
     Path should contain `Node` name, separated by `sep`.
@@ -506,23 +506,23 @@
     │   └── e
     │       ├── g
     │       └── h
     └── c
         └── f
 
     Args:
-        paths (List[str]): list containing path strings
+        paths (Iterable[str]): list containing path strings
         sep (str): path separator for input `paths` and created tree, defaults to `/`
         duplicate_name_allowed (bool): indicator if nodes with duplicated `Node` name is allowed, defaults to True
         node_type (Type[Node]): node type of tree to be created, defaults to Node
 
     Returns:
         (Node)
     """
-    if not len(paths):
+    if not paths:
         raise ValueError("Path list does not contain any data, check `paths`")
 
     # Remove duplicates
     paths = list(OrderedDict.fromkeys(paths))
 
     # Construct root node
     root_name = paths[0].lstrip(sep).split(sep)[0]
@@ -534,15 +534,15 @@
             root_node, path, sep=sep, duplicate_name_allowed=duplicate_name_allowed
         )
     root_node.sep = sep
     return root_node
 
 
 def list_to_tree_by_relation(
-    relations: List[Tuple[str, str]],
+    relations: Iterable[Tuple[str, str]],
     node_type: Type[Node] = Node,
 ) -> Node:
     """Construct tree from list of tuple containing parent-child names.
 
     Note that node names must be unique since tree is created from parent-child names,
     except for leaf nodes - names of leaf nodes may be repeated as there is no confusion.
 
@@ -556,21 +556,21 @@
     │   └── e
     │       ├── g
     │       └── h
     └── c
         └── f
 
     Args:
-        relations (List[Tuple[str, str]]): list containing tuple containing parent-child names
+        relations (Iterable[Tuple[str, str]]): list containing tuple containing parent-child names
         node_type (Type[Node]): node type of tree to be created, defaults to Node
 
     Returns:
         (Node)
     """
-    if not len(relations):
+    if not relations:
         raise ValueError("Path list does not contain any data, check `relations`")
 
     relation_data = pd.DataFrame(relations, columns=["parent", "child"])
     return dataframe_to_tree_by_relation(
         relation_data, child_col="child", parent_col="parent", node_type=node_type
     )
```

### Comparing `bigtree-0.9.2/bigtree/tree/export.py` & `bigtree-0.9.3/bigtree/tree/export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/tree/helper.py` & `bigtree-0.9.3/bigtree/tree/helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/tree/modify.py` & `bigtree-0.9.3/bigtree/tree/modify.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/tree/search.py` & `bigtree-0.9.3/bigtree/tree/search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/utils/iterators.py` & `bigtree-0.9.3/bigtree/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/workflows/app_calendar.py` & `bigtree-0.9.3/bigtree/workflows/app_calendar.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/bigtree/workflows/app_todo.py` & `bigtree-0.9.3/bigtree/workflows/app_todo.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/Makefile` & `bigtree-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/make.bat` & `bigtree-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/conf.py` & `bigtree-0.9.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/index.rst` & `bigtree-0.9.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/_static/custom.css` & `bigtree-0.9.3/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/_static/favicon.ico` & `bigtree-0.9.3/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/_templates/layout.html` & `bigtree-0.9.3/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/bigtree/dag/construct.rst` & `bigtree-0.9.3/docs/source/bigtree/dag/construct.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/bigtree/dag/export.rst` & `bigtree-0.9.3/docs/source/bigtree/dag/export.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/bigtree/tree/construct.rst` & `bigtree-0.9.3/docs/source/bigtree/tree/construct.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/bigtree/tree/export.rst` & `bigtree-0.9.3/docs/source/bigtree/tree/export.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/bigtree/tree/modify.rst` & `bigtree-0.9.3/docs/source/bigtree/tree/modify.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/bigtree/tree/search.rst` & `bigtree-0.9.3/docs/source/bigtree/tree/search.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/bigtree/utils/iterators.rst` & `bigtree-0.9.3/docs/source/bigtree/utils/iterators.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/others/contributing.rst` & `bigtree-0.9.3/docs/source/others/contributing.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/others/merging_trees.md` & `bigtree-0.9.3/docs/source/others/merging_trees.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/others/nodes.md` & `bigtree-0.9.3/docs/source/others/nodes.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/docs/source/others/weighted_trees.md` & `bigtree-0.9.3/docs/source/others/weighted_trees.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/conftest.py` & `bigtree-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/binarytree/test_construct.py` & `bigtree-0.9.3/tests/binarytree/test_construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/binarytree/test_export.py` & `bigtree-0.9.3/tests/binarytree/test_export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/binarytree/test_helper.py` & `bigtree-0.9.3/tests/binarytree/test_helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/binarytree/test_search.py` & `bigtree-0.9.3/tests/binarytree/test_search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/dag/test_construct.py` & `bigtree-0.9.3/tests/dag/test_construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/dag/test_export.py` & `bigtree-0.9.3/tests/dag/test_export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/node/test_basenode.py` & `bigtree-0.9.3/tests/node/test_basenode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/node/test_binarynode.py` & `bigtree-0.9.3/tests/node/test_binarynode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/node/test_dagnode.py` & `bigtree-0.9.3/tests/node/test_dagnode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/node/test_node.py` & `bigtree-0.9.3/tests/node/test_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,24 @@
         # Set parent again
         self.a = Node(name="a", age=90)
         self.b = Node(name="b", age=65, parent=self.a)
         self.b.parent = self.a
         assert list(self.a.children) == [self.b]
         assert self.b.parent == self.a
 
+    def test_set_parent_sep_different_error_message(self):
+        b = Node("b", sep="\\")
+        self.b.parent = self.a
+        with pytest.raises(TreeError) as exc_info:
+            b.parent = self.a
+        assert (
+            str(exc_info.value)
+            == "Error: Duplicate node with same path\nThere exist a node with same path /a/b"
+        )
+
     def test_set_parent_sep_root(self):
         self.b.parent = self.a
         self.c.parent = self.a
         self.d.parent = self.b
         self.e.parent = self.b
         self.f.parent = self.c
         self.g.parent = self.e
@@ -160,14 +170,23 @@
         self.a.children = [self.b]
 
     def test_set_children_duplicate_constructor(self):
         # Set child again
         self.a = Node("a", children=[self.b])
         self.a.children = [self.b]
 
+    def test_children_sep_different_error_message(self):
+        b = Node("b", sep="\\")
+        with pytest.raises(TreeError) as exc_info:
+            self.a.children = [self.b, b]
+        assert (
+            str(exc_info.value)
+            == "Error: Duplicate node with same path\nAttempting to add nodes same path /a/b"
+        )
+
     def test_error_set_parent_same_path(self):
         self.a = Node("a")
         self.b = Node("b", parent=self.a)
         self.c = Node("b")
         with pytest.raises(TreeError):
             self.c.parent = self.a
```

### Comparing `bigtree-0.9.2/tests/tree/test_construct.py` & `bigtree-0.9.3/tests/tree/test_construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/tree/test_export.py` & `bigtree-0.9.3/tests/tree/test_export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/tree/test_helper.py` & `bigtree-0.9.3/tests/tree/test_helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/tree/test_modify.py` & `bigtree-0.9.3/tests/tree/test_modify.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/tree/test_search.py` & `bigtree-0.9.3/tests/tree/test_search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/utils/test_iterators.py` & `bigtree-0.9.3/tests/utils/test_iterators.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/tests/workflows/test_todo.py` & `bigtree-0.9.3/tests/workflows/test_todo.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/LICENSE` & `bigtree-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/README.md` & `bigtree-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/pyproject.toml` & `bigtree-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.2/PKG-INFO` & `bigtree-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtree
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tree Implementation for Python, integrated with Python list, dictionary, and pandas DataFrame.
 Project-URL: Documentation, https://bigtree.readthedocs.io
 Project-URL: Issues, https://github.com/kayjan/bigtree/issues
 Project-URL: Source, https://github.com/kayjan/bigtree
 Author-email: Kay Jan <kayjanw@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bigtree Version: 0.9.2 Summary: Tree Implementation
+Metadata-Version: 2.1 Name: bigtree Version: 0.9.3 Summary: Tree Implementation
 for Python, integrated with Python list, dictionary, and pandas DataFrame.
 Project-URL: Documentation, https://bigtree.readthedocs.io Project-URL: Issues,
 https://github.com/kayjan/bigtree/issues Project-URL: Source, https://
 github.com/kayjan/bigtree Author-email: Kay Jan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: bigtree,tree
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.7 Classifier:
```

