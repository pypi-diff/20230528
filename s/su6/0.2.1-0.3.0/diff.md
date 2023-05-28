# Comparing `tmp/su6-0.2.1.tar.gz` & `tmp/su6-0.3.0.tar.gz`

## Comparing `su6-0.2.1.tar` & `su6-0.3.0.tar`

### file list

```diff
@@ -1,670 +1,690 @@
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/colorsys.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/colorsys.meta.json
--rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/linecache.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/linecache.meta.json
--rw-r--r--   0        0        0    32512 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/locale.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/locale.meta.json
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/pty.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/pty.meta.json
--rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/pydoc.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/pydoc.meta.json
--rw-r--r--   0        0        0    39910 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/zlib.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/zlib.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    45562 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   182278 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    27933 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/html/entities.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/html/entities.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    94562 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/main.data.json
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/main.meta.json
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/token.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/token.meta.json
--rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_format.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_format.meta.json
--rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_url.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/mdurl/_url.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/__init__.meta.json
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/__main__.data.json
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/__main__.meta.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_export_format.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_extension.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_extension.meta.json
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_fileno.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_fileno.meta.json
--rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_inspect.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_inspect.meta.json
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_log_render.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_log_render.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_loop.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_loop.meta.json
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_null_file.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_palettes.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_pick.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_pick.meta.json
--rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_ratio.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_spinners.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_spinners.meta.json
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_stack.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_stack.meta.json
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_timer.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_timer.meta.json
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_windows.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_windows.meta.json
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_wrap.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/_wrap.meta.json
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/abc.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/abc.meta.json
--rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/align.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/align.meta.json
--rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/ansi.data.json
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/ansi.meta.json
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/box.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/box.meta.json
--rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/cells.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/cells.meta.json
--rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/color.data.json
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/color.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/columns.data.json
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/columns.meta.json
--rw-r--r--   0        0        0   175685 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/console.data.json
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/console.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/constrain.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/constrain.meta.json
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/containers.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/containers.meta.json
--rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/control.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/control.meta.json
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/default_styles.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/emoji.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/emoji.meta.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/errors.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/errors.meta.json
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/highlighter.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/json.data.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/json.meta.json
--rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/jupyter.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/jupyter.meta.json
--rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/live.data.json
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/live.meta.json
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/live_render.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/live_render.meta.json
--rw-r--r--   0        0        0    66647 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/markdown.data.json
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/markdown.meta.json
--rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/markup.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/markup.meta.json
--rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/measure.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/measure.meta.json
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/padding.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/padding.meta.json
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/pager.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/pager.meta.json
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/palette.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/palette.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/panel.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/panel.meta.json
--rw-r--r--   0        0        0   112532 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/pretty.data.json
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/pretty.meta.json
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/protocol.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/protocol.meta.json
--rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/region.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/region.meta.json
--rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/repr.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/repr.meta.json
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/rule.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/rule.meta.json
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/scope.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/scope.meta.json
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/screen.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/screen.meta.json
--rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/segment.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/segment.meta.json
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/spinner.data.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/spinner.meta.json
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/status.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/status.meta.json
--rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/style.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/style.meta.json
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/styled.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/styled.meta.json
--rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/syntax.data.json
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/syntax.meta.json
--rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/table.data.json
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/table.meta.json
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/text.data.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/text.meta.json
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/theme.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/theme.meta.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/themes.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/themes.meta.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/traceback.data.json
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/rich/traceback.meta.json
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6/__about__.data.json
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6/__about__.meta.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6/__init__.data.json
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6/__init__.meta.json
--rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6/cli.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6/cli.meta.json
--rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6/core.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6/core.meta.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6_checker/__about__.data.json
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6_checker/__about__.meta.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6_checker/__init__.data.json
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6_checker/__init__.meta.json
--rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6_checker/cli.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6_checker/cli.meta.json
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6_checker/core.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/su6_checker/core.meta.json
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/tests/__init__.data.json
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/tests/__init__.meta.json
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_completion_click7.data.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_completion_click7.meta.json
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_completion_click8.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_completion_click8.meta.json
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    59399 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    33728 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 su6-0.2.1/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/1dcbdc62e66ccf0e
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/1f88fbdfcbf2d8d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/1fbfdffa4078f509
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/23da3e9165a5513d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/25d9504d2b6847d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/2a630c7d6d7faa40
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/2b0cdebce71424f0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/35ab5ee4981cdf8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/380a13ecd1a2af25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/3c9bb20c3b57bae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/3cf13d9d13babf93
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/47ca38fe0242f05d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/4d5914600f7e99c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/4f75816f4078d31b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/4f8371badac33c92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/54637ff0aaaaf6b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/552fa1eb2057eecc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/55c947c0fa59929
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/5a6dc8ef65620223
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/5b7183ee842066de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/6550bbd98b1711bd
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/684d0841c18787fb
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/68c4553df91c1f5e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/6a74d0efd6350f1e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/6c989c6e4eea10bd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/7cc3783d00621498
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/7cf495b196c50222
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/7dc27d897f910c11
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/80844117d21fe12b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/80ded2016f4f413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/835f19fb8c240dbe
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/881c84062ed51136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/8a437c05421c6cb5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/8d2f83aae152de29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/902eb6f99ee41131
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/9080aaa3f2416b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/922bfc03482db456
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/93fed7ae4120c88e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/97a72bc70808d2f9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/9e915e4e576201bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/a0572377dc282cac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/a24edf91b0bcff12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/a3b201bbf3062966
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/a943564382aec90a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/aa2551751b9adb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/abc8db1325696a17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/acecedeb9f4dd91a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/aff288abf6945582
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/b03db5008e4f8099
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/b8d965aa2b8fd993
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/b990e7d90d89db2a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/bae3ebdf4629f324
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/be4a1815dbb4c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/beb37e84505d7dd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/c0d14d0162a80714
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/c250dc207334d18
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/c293dd30723003b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/c6dc2ffa42b39365
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/c766d7d105d53e92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/c9d297807d108576
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/cb0e3b769b6a1727
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/cbb8b9fccd8c8746
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/ccc4c37cd56e46e5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/d1c81941e3ef2e1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/d1d63b74d8d929b9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/d3a20b1509715554
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/d9cd4c2a9ad4580d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/e8ab3d919ff04fd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/e8cd5143f259cdce
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/f1af1d1ebb07ad61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.2.1/.ruff_cache/content/f58e778cbde5b210
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 su6-0.2.1/src/su6/__about__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 su6-0.2.1/src/su6/__init__.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 su6-0.2.1/src/su6/cli.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 su6-0.2.1/src/su6/core.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6-0.2.1/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 su6-0.2.1/README.md
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 su6-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/colorsys.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/colorsys.meta.json
+-rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/linecache.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/linecache.meta.json
+-rw-r--r--   0        0        0    32512 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/locale.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/locale.meta.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/pty.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/pty.meta.json
+-rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/pydoc.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/pydoc.meta.json
+-rw-r--r--   0        0        0    39910 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/zlib.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/zlib.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    45562 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   182278 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27933 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/html/entities.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/html/entities.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    94562 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/mdurl/_url.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/__main__.data.json
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_extension.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_fileno.meta.json
+-rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_inspect.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_inspect.meta.json
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_loop.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_loop.meta.json
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_pick.data.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_stack.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_timer.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_timer.meta.json
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_windows.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/abc.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/abc.meta.json
+-rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/align.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/align.meta.json
+-rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/ansi.data.json
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/ansi.meta.json
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/box.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/box.meta.json
+-rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/cells.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/cells.meta.json
+-rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/color.data.json
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/color.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/columns.data.json
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/columns.meta.json
+-rw-r--r--   0        0        0   175685 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/console.data.json
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/console.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/constrain.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/constrain.meta.json
+-rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/containers.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/containers.meta.json
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/control.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/control.meta.json
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/default_styles.data.json
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/emoji.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/errors.data.json
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/errors.meta.json
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/json.data.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/json.meta.json
+-rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/live.data.json
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/live.meta.json
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/live_render.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/live_render.meta.json
+-rw-r--r--   0        0        0    66647 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/markdown.data.json
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/markdown.meta.json
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/markup.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/markup.meta.json
+-rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/measure.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/measure.meta.json
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/padding.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/padding.meta.json
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/pager.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/pager.meta.json
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/palette.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/palette.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/panel.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/panel.meta.json
+-rw-r--r--   0        0        0   112532 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/pretty.data.json
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/protocol.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/protocol.meta.json
+-rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/region.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/region.meta.json
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/repr.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/repr.meta.json
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/rule.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/rule.meta.json
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/scope.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/scope.meta.json
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/screen.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/screen.meta.json
+-rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/segment.data.json
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/segment.meta.json
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/spinner.data.json
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/spinner.meta.json
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/status.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/status.meta.json
+-rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/style.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/style.meta.json
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/styled.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/styled.meta.json
+-rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/syntax.data.json
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/syntax.meta.json
+-rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/table.data.json
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/table.meta.json
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/text.data.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/text.meta.json
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/theme.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/theme.meta.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/themes.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/themes.meta.json
+-rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/traceback.data.json
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/rich/traceback.meta.json
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6/__about__.data.json
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6/__about__.meta.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6/__init__.data.json
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6/__init__.meta.json
+-rw-r--r--   0        0        0    18332 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6/cli.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6/cli.meta.json
+-rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6/core.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6/core.meta.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6_checker/__about__.data.json
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6_checker/__about__.meta.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6_checker/__init__.data.json
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6_checker/__init__.meta.json
+-rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6_checker/cli.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6_checker/cli.meta.json
+-rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6_checker/core.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/su6_checker/core.meta.json
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/tests/__init__.data.json
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/tests/__init__.meta.json
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    59399 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    33728 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 su6-0.3.0/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/10595a931c3c881e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/11f25cfda4e2f210
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/13985ae090677282
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/1cfd31ba4b0b7ef9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/1dcbdc62e66ccf0e
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/1f88fbdfcbf2d8d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/1fbfdffa4078f509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/23da3e9165a5513d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/25d9504d2b6847d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/2a630c7d6d7faa40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/2b0cdebce71424f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/2e4746b83d2d1cf8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/3271e344462a0ee3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/34e1109d49bf09f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/35ab5ee4981cdf8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/380a13ecd1a2af25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/3c6b70c96e832bc1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/3c9bb20c3b57bae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/3cf13d9d13babf93
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/47ca38fe0242f05d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/4d5914600f7e99c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/4f75816f4078d31b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/4f8371badac33c92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/54637ff0aaaaf6b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/552fa1eb2057eecc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/55c947c0fa59929
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/5a6dc8ef65620223
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/5b7183ee842066de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/6550bbd98b1711bd
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/684d0841c18787fb
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/68c4553df91c1f5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/6a74d0efd6350f1e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/6c989c6e4eea10bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/6db20c27780d4a5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/76d56794deeb084d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/7cc3783d00621498
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/7cf495b196c50222
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/7dc27d897f910c11
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/7f75cbd11ebac70a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/80844117d21fe12b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/80ded2016f4f413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/835f19fb8c240dbe
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/881c84062ed51136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/8a437c05421c6cb5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/8d2f83aae152de29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/902eb6f99ee41131
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/9080aaa3f2416b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/922bfc03482db456
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/93fed7ae4120c88e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/945994955724de24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/94ffcc82bc7ee370
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/968b32ac9319cc53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/97a72bc70808d2f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/9e915e4e576201bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/a0572377dc282cac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/a24edf91b0bcff12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/a3b201bbf3062966
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/a943564382aec90a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/aa2551751b9adb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/abc8db1325696a17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/acecedeb9f4dd91a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/aff288abf6945582
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/b03db5008e4f8099
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/b2d26e3968f3c218
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/b8d965aa2b8fd993
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/b990e7d90d89db2a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/bae3ebdf4629f324
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/bdeb811362915192
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/be4a1815dbb4c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/beb37e84505d7dd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/c0d14d0162a80714
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/c250dc207334d18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/c293dd30723003b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/c6dc2ffa42b39365
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/c766d7d105d53e92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/c9d297807d108576
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/cb0e3b769b6a1727
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/cbb8b9fccd8c8746
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/ccc4c37cd56e46e5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/d1c81941e3ef2e1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/d1d63b74d8d929b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/d3a20b1509715554
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/d9cd4c2a9ad4580d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/da4aff17737df0c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/de1238012a6853f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/dfc2e498a5736fb3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/e8ab3d919ff04fd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/e8cd5143f259cdce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/f1af1d1ebb07ad61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/f41987c18d73e01d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.3.0/.ruff_cache/content/f58e778cbde5b210
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-0.3.0/src/su6/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 su6-0.3.0/src/su6/__init__.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 su6-0.3.0/src/su6/cli.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 su6-0.3.0/src/su6/core.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 su6-0.3.0/README.md
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 su6-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 su6-0.3.0/PKG-INFO
```

### Comparing `su6-0.2.1/CHANGELOG.md` & `su6-0.3.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.0 (2023-05-28)
+### Feature
+* **all:** Allow running `su6 all --ignore-uninstalled` so missing checking tools don't affect the final exit code of 'all' ([`35ad498`](https://github.com/robinvandernoord/su6-checker/commit/35ad498983bd651d66bfa3e773b9a1e1e7d94e6c))
+* **pydocstyle:** Added docstring checker (and docstrings) ([`4ad2c29`](https://github.com/robinvandernoord/su6-checker/commit/4ad2c29c88a840dd01640a8d9bcf4695834e37a5))
+
+### Documentation
+* **readme:** Added list of supported tools ([`02fb7a8`](https://github.com/robinvandernoord/su6-checker/commit/02fb7a86673f64e4ab937b6f5a7b45543ab86aa1))
+
 ## v0.2.1 (2023-05-27)
 ### Fix
 * **exit codes:** They now actually work™ ([`503c69c`](https://github.com/robinvandernoord/su6-checker/commit/503c69ccf5d4d91847fd4f0580511d6a89800fd6))
 
 ## v0.2.0 (2023-05-27)
 ### Feature
 * **shell:** Introduce @with_exit_code decorator to generate an exit code based on the return value of a command method ([`7d6d4e2`](https://github.com/robinvandernoord/su6-checker/commit/7d6d4e27c2226538b79f63b972c90045517cbe46))
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/__future__.data.json` & `su6-0.3.0/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/__future__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/linecache.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7587301587301588%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 2), (2, 3)]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (1, 'typing'), (4, '_typeshed')], delete: [3]}",*

 * * "'hash'": "'1f773c204e1f7123a2f3cafec9d8bb3cf43479274b225843f556667e1908bca1'",*

 * * "'id'": "'linecache'",*

 * * "'interface_hash'": "'a394a279efd903e56d257cc3537d959bb52b584529de0c2b3aa60e3456eaba5d'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/lin […]*

```diff
@@ -1,32 +1,38 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
+        2,
+        3,
         1,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
+        "sys",
+        "typing",
         "typing_extensions",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "a88c160e68dac375c28ae94a628281401fde2632f1c1e7ac50ac017699204245",
-    "id": "__future__",
+    "hash": "1f773c204e1f7123a2f3cafec9d8bb3cf43479274b225843f556667e1908bca1",
+    "id": "linecache",
     "ignore_all": true,
-    "interface_hash": "785a6eda02f10c252e25c75d49899c617f4a50f56ab17aa5d128094494bb6647",
-    "mtime": 1685143295,
+    "interface_hash": "a394a279efd903e56d257cc3537d959bb52b584529de0c2b3aa60e3456eaba5d",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/__future__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/linecache.pyi",
     "plugin_data": null,
-    "size": 915,
+    "size": 945,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_ast.data.json` & `su6-0.3.0/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_ast.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_spinners.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7428571428571428%*

 * *Differences: {"'dep_lines'": '{delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(2, 'typing')], delete: [4, 2, 1, 0]}",*

 * * "'hash'": "'536af5fe0ff5cd28ec8e251d00449cda200c7378b8ae2fd2f0f60fea4439cf52'",*

 * * "'id'": "'rich._spinners'",*

 * * "'interface_hash'": "'f558f1ab7e7f9f21e444f7e168b8db6631e82ff78cd9044f5868b920441ad001'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_spinners.py'",*

 * * "'size'": '19919'}*

```diff
@@ -1,38 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        2,
-        3,
-        1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
-        5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "sys",
-        "typing",
-        "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "189ca9e5f979d2fafddf0fde549a04c4da5840422b279c427ac3b84df670b646",
-    "id": "_ast",
+    "hash": "536af5fe0ff5cd28ec8e251d00449cda200c7378b8ae2fd2f0f60fea4439cf52",
+    "id": "rich._spinners",
     "ignore_all": true,
-    "interface_hash": "7aaf7eb03088c4a732c70e702b755199cfa669aed9dbaf9b63d04ceb2f07d568",
-    "mtime": 1685143295,
+    "interface_hash": "f558f1ab7e7f9f21e444f7e168b8db6631e82ff78cd9044f5868b920441ad001",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_ast.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_spinners.py",
     "plugin_data": null,
-    "size": 14752,
+    "size": 19919,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_codecs.data.json` & `su6-0.3.0/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_codecs.meta.json` & `su6-0.3.0/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7475748194014448%*

 * *Differences: {"'dep_lines'": '{insert: [(6, 7), (7, 8), (8, 9), (9, 10), (10, 11)], delete: [8, 7, 6]}',*

 * * "'dep_prios'": '{insert: [(7, 5), (8, 5), (9, 5), (10, 5), (11, 5)], delete: [9, 8, 7]}',*

 * * "'dependencies'": "{insert: [(2, 'threading'), (4, 'io'), (5, 're'), (6, 'string'), (7, 'time'), "*

 * *                   "(8, 'types'), (13, 'os')], delete: [11, 10, 9, 8, 1]}",*

 * * "'hash'": "'efc0ae6530114eeb664869aab1a543a7e88f59df3c5c479d47e85dff0c989728'",*

 * * "'id'": "'logging'",*

 * * "'interface_hash'": "'6cbb4e8d90f49e871cd2109526d […]*

```diff
@@ -3,54 +3,60 @@
     "dep_lines": [
         4,
         1,
         2,
         3,
         5,
         6,
-        1,
-        1,
-        1,
+        7,
+        8,
+        9,
+        10,
+        11,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         10,
         5,
         5,
         5,
         5,
-        30,
-        30,
-        30,
+        5,
+        5,
+        5,
+        5,
+        5,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "codecs",
         "sys",
+        "threading",
         "_typeshed",
+        "io",
+        "re",
+        "string",
+        "time",
+        "types",
         "typing",
         "typing_extensions",
         "builtins",
         "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle"
+        "os"
     ],
-    "hash": "70e3defc1875bd08c24cbe869d9c14280401dc8b591637db091aad6a71684e1d",
-    "id": "_codecs",
+    "hash": "efc0ae6530114eeb664869aab1a543a7e88f59df3c5c479d47e85dff0c989728",
+    "id": "logging",
     "ignore_all": true,
-    "interface_hash": "b46b35bd03ec1cc9344093253180c85f42512ae908969e157e6619fb188b42f0",
-    "mtime": 1685143295,
+    "interface_hash": "6cbb4e8d90f49e871cd2109526db7296823c495b45acf5b495d714a78376aa50",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -84,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_codecs.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/logging/__init__.pyi",
     "plugin_data": null,
-    "size": 7280,
+    "size": 27004,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_collections_abc.data.json` & `su6-0.3.0/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -24,15 +24,15 @@
         "builtins",
         "abc"
     ],
     "hash": "a1242071aa8e060f1cb055c8d542467362f026499a9139fbcf15943f854ffcf5",
     "id": "_collections_abc",
     "ignore_all": true,
     "interface_hash": "021275b69c7711fa3770e4c0f14fc6f1bb88360b67da9800e3d413a3cfdd8b11",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_csv.data.json` & `su6-0.3.0/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_csv.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_csv.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -36,15 +36,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "ade13cca8f205a4385a4fe07742cfafb93aa2a37ba4ab8cfb4e2d5540c2a2b74",
     "id": "_csv",
     "ignore_all": true,
     "interface_hash": "1421c2d6ce5d771ba6ed757d6e9517d416d3bd151acdfb508fb3a0b21b5531ce",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_ctypes.data.json` & `su6-0.3.0/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_ctypes.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -27,15 +27,15 @@
         "abc",
         "typing"
     ],
     "hash": "f3f569576a38ac44f7351d80826ca0da2673c3895b9278a10d671615e6388fc9",
     "id": "_ctypes",
     "ignore_all": true,
     "interface_hash": "7d8346b18f5469b335c487cef9085c18fcd2dd06b78e2d61aef6b4bc1b48905f",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_decimal.data.json` & `su6-0.3.0/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_decimal.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_decimal.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -33,15 +33,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "48f8deddc79e8ef4fb7dfd0456d1de03d7cd794ec47739eea4b21ccef910976c",
     "id": "_decimal",
     "ignore_all": true,
     "interface_hash": "79bccc35c512a3b8d3061901e6a903ceee81e5adc7515d0e4790353e3135cbe7",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_operator.data.json` & `su6-0.3.0/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_operator.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_random.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7375%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 1)], delete: [4, 3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(3, 'typing')], delete: [3, 2, 1, 0]}",*

 * * "'hash'": "'fdcf346a4f5cf1e59ed16298d1a44114f183d1641e67553a52691ba2bd17c788'",*

 * * "'id'": "'_random'",*

 * * "'interface_hash'": "'8b34aaa585fc566099f20141576a0ac969bf0b7e9ecd4766f929651ee0fe8599'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdli […]*

```diff
@@ -1,41 +1,32 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        3,
         1,
-        2,
-        4,
-        5,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
-        5,
         5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
-        "_typeshed",
-        "typing",
         "typing_extensions",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "6af6cdd45bab26f05bd668e6a9adf75595caa87cbfb531af9addb4e0dd18636a",
-    "id": "_operator",
+    "hash": "fdcf346a4f5cf1e59ed16298d1a44114f183d1641e67553a52691ba2bd17c788",
+    "id": "_random",
     "ignore_all": true,
-    "interface_hash": "f1d7d99b1fca61d4b596b68f2c83c01e2a71cc79a0beede674ee626f73a36f3d",
-    "mtime": 1685143295,
+    "interface_hash": "8b34aaa585fc566099f20141576a0ac969bf0b7e9ecd4766f929651ee0fe8599",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_operator.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_random.pyi",
     "plugin_data": null,
-    "size": 6585,
+    "size": 405,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_random.data.json` & `su6-0.3.0/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_random.meta.json` & `su6-0.3.0/.mypy_cache/3.11/string.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7396296296296296%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 3), (2, 2), (3, 4), (4, 5), (5, 6)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5), (3, 5), (4, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, '_typeshed'), (3, 're'), (4, "*

 * *                   "'typing'), (8, 'enum')], delete: [3]}",*

 * * "'hash'": "'cc44bbe664dd2094229250b9499117bb258740f154f72d04a08d32edb54ad646'",*

 * * "'id'": "'string'",*

 * * "'interface_hash'": "'5bb98aba794ab5988f1bfd88b7f0e191c9464bf62d9d67e4378a3a6f7bcb5e84'",*

 * * "'mtime'": '1685 […]*

```diff
@@ -1,32 +1,47 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        3,
         1,
+        2,
+        4,
+        5,
+        6,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
+        5,
+        5,
         5,
         30,
         30
     ],
     "dependencies": [
+        "collections.abc",
+        "sys",
+        "_typeshed",
+        "re",
+        "typing",
         "typing_extensions",
         "builtins",
         "abc",
-        "typing"
+        "enum"
     ],
-    "hash": "fdcf346a4f5cf1e59ed16298d1a44114f183d1641e67553a52691ba2bd17c788",
-    "id": "_random",
+    "hash": "cc44bbe664dd2094229250b9499117bb258740f154f72d04a08d32edb54ad646",
+    "id": "string",
     "ignore_all": true,
-    "interface_hash": "8b34aaa585fc566099f20141576a0ac969bf0b7e9ecd4766f929651ee0fe8599",
-    "mtime": 1685143295,
+    "interface_hash": "5bb98aba794ab5988f1bfd88b7f0e191c9464bf62d9d67e4378a3a6f7bcb5e84",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_random.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/string.pyi",
     "plugin_data": null,
-    "size": 405,
+    "size": 3097,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_stat.data.json` & `su6-0.3.0/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_stat.meta.json` & `su6-0.3.0/.mypy_cache/3.11/reprlib.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7503703703703705%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 4), (3, 3), (4, 5), (5, 6)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (2, 5), (3, 5), (4, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (2, 'array'), (3, 'collections'), (4, "*

 * *                   "'typing'), (7, '_typeshed')], delete: [4]}",*

 * * "'hash'": "'bac2ab52145c08d78e55d632dd2e88f278d13915c843dad7ac699ed34b8625de'",*

 * * "'id'": "'reprlib'",*

 * * "'interface_hash'": "'2eb446a6a81cfec3b4a0186b8ae767f2e8cd8c96d9e9e750fefe61aa857d5260'",*

 * * "'mtime'": '1685283590',*

 * * "'path'" […]*

```diff
@@ -1,35 +1,47 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        4,
         1,
         2,
+        3,
+        5,
+        6,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
         10,
         5,
         5,
+        5,
+        5,
+        5,
         30,
         30
     ],
     "dependencies": [
+        "collections.abc",
         "sys",
+        "array",
+        "collections",
+        "typing",
         "typing_extensions",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "4545d9f4011bbe91db363d9537e5d852b7ba1d7bb73b7bda9b540122a7cac958",
-    "id": "_stat",
+    "hash": "bac2ab52145c08d78e55d632dd2e88f278d13915c843dad7ac699ed34b8625de",
+    "id": "reprlib",
     "ignore_all": true,
-    "interface_hash": "a61aa73892cc82b90287425ecfc03dac292e910c9ec04af03c2cfc83c8a85db4",
-    "mtime": 1685143295,
+    "interface_hash": "2eb446a6a81cfec3b4a0186b8ae767f2e8cd8c96d9e9e750fefe61aa857d5260",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_stat.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/reprlib.pyi",
     "plugin_data": null,
-    "size": 2944,
+    "size": 1986,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_thread.data.json` & `su6-0.3.0/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_thread.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_thread.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -33,15 +33,15 @@
         "builtins",
         "abc"
     ],
     "hash": "1dd9af47a90f2cba023502a65ef81a3126f4c5a0299b3b749b8a738dab49754f",
     "id": "_thread",
     "ignore_all": true,
     "interface_hash": "0d5cc4e4dc7dd5e40c1cb3a31c0455fd4b5a6096a1b531c79b5b7587b146d932",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_warnings.data.json` & `su6-0.3.0/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_warnings.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/cells.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7375%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 5), (1, 1), (2, 2), (3, 3), (4, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5), (5, 30), (6, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich._cell_widths'), (1, 're'), (2, 'functools'), (5, "*

 * *                   "'_typeshed'), (7, 'typing_extensions')]}",*

 * * "'hash'": "'eb6ef3b49b3dcce2fedfc1c9ee45c17ab47e813f0a05f602f14cc4c0c243618a'",*

 * * "'id'": "'rich.cells'",*

 * * "'interface_hash'": "'172e16952ab394c6ff692362a0d695ea8e0835948ad5846a9a454987745962e0'",*

 * * "'mtime'": '16851 […]*

```diff
@@ -1,29 +1,44 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        5,
+        1,
+        2,
+        3,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
         5,
+        30,
+        30,
         30
     ],
     "dependencies": [
+        "rich._cell_widths",
+        "re",
+        "functools",
         "typing",
         "builtins",
-        "abc"
+        "_typeshed",
+        "abc",
+        "typing_extensions"
     ],
-    "hash": "12ca327a8db64a2d4a7ce3e48dec89640981b34dbc8f6485f78899f6bd7625bc",
-    "id": "_warnings",
+    "hash": "eb6ef3b49b3dcce2fedfc1c9ee45c17ab47e813f0a05f602f14cc4c0c243618a",
+    "id": "rich.cells",
     "ignore_all": true,
-    "interface_hash": "d82c2fe96f249f6c67c9f318da861954091d569054e5678599df9778edc8c3ee",
-    "mtime": 1685143295,
+    "interface_hash": "172e16952ab394c6ff692362a0d695ea8e0835948ad5846a9a454987745962e0",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_warnings.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/cells.py",
     "plugin_data": null,
-    "size": 1026,
+    "size": 4509,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_weakref.data.json` & `su6-0.3.0/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_weakref.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_weakref.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -30,15 +30,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "bc440d5501e9ede6acdd4bab5144475ec983f6eecd62e3dc9f71b0c29506a02e",
     "id": "_weakref",
     "ignore_all": true,
     "interface_hash": "8b5dbc2c5adfca3ceb92f87748ab7f89694e25a28b282e22ea33b6831489006b",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_weakrefset.data.json` & `su6-0.3.0/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_weakrefset.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/screen.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7154364154364153%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(2, 5), (3, 9), (4, 1)], delete: [4, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 20)], delete: [1]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.segment'), (1, 'rich.style'), (2, 'rich._loop'), (3, "*

 * *                   "'rich.console'), (7, 'enum')], delete: [6, 4, 3, 1, 0]}",*

 * * "'hash'": "'acbfe3db05fee127ae20e236a0e95ce35f103fd100bc3e7d1889d4984004ea34'",*

 * * "'id'": "'rich.screen'",*

 * * "'interface_hash'": "'8db842986b5cbf3353da698ac5ce0831e10b1b74953434b144367 […]*

```diff
@@ -1,44 +1,44 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        2,
-        1,
         3,
         4,
-        7,
+        5,
+        9,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
         5,
         5,
+        20,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
+        "rich.segment",
+        "rich.style",
+        "rich._loop",
+        "rich.console",
         "typing",
-        "typing_extensions",
-        "types",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "enum"
     ],
-    "hash": "a95feb712aa1ad0440aa1c3ff081329b8a7a976bf976c7cdcd39b1c5d227ea57",
-    "id": "_weakrefset",
+    "hash": "acbfe3db05fee127ae20e236a0e95ce35f103fd100bc3e7d1889d4984004ea34",
+    "id": "rich.screen",
     "ignore_all": true,
-    "interface_hash": "b235dadc5fe23ff0afd8bfe6f1ee02cb171d77545e4c45adbd244eca1a7f68eb",
-    "mtime": 1685143295,
+    "interface_hash": "8db842986b5cbf3353da698ac5ce0831e10b1b74953434b144367bdd7fa15210",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/screen.py",
     "plugin_data": null,
-    "size": 2383,
+    "size": 1579,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/abc.data.json` & `su6-0.3.0/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/abc.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_loop.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.725%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 1), (2, 1)], delete: [4, 3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 30), (3, 30)], delete: [3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(2, '_typeshed'), (3, 'abc')], delete: [4, 2, 1, 0]}",*

 * * "'hash'": "'855ffa08b7683e6d2f6b6d96a70e332aa334458b33dd36715e3d0fa12fbd7834'",*

 * * "'id'": "'rich._loop'",*

 * * "'interface_hash'": "'b76fc611635bcba78ac86d56ecdf76df5d52e4165957022fabc6fe38e4bba5bf'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.1 […]*

```diff
@@ -1,38 +1,32 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        4,
         1,
-        2,
-        5,
-        6,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        10,
-        5,
-        5,
-        5
+        30,
+        30
     ],
     "dependencies": [
-        "collections.abc",
-        "_typeshed",
-        "sys",
         "typing",
-        "typing_extensions",
-        "builtins"
+        "builtins",
+        "_typeshed",
+        "abc"
     ],
-    "hash": "ceadae3f72efc214373499b073a01a7026c2fbec852c488327ec4bad5cb23b67",
-    "id": "abc",
+    "hash": "855ffa08b7683e6d2f6b6d96a70e332aa334458b33dd36715e3d0fa12fbd7834",
+    "id": "rich._loop",
     "ignore_all": true,
-    "interface_hash": "0eec2da7f77546f50f6e9328b32cd2abdc0038afe86d0a726dfd6d2bcfcee607",
-    "mtime": 1685143295,
+    "interface_hash": "b76fc611635bcba78ac86d56ecdf76df5d52e4165957022fabc6fe38e4bba5bf",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/abc.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_loop.py",
     "plugin_data": null,
-    "size": 1773,
+    "size": 1236,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/argparse.data.json` & `su6-0.3.0/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/argparse.meta.json` & `su6-0.3.0/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7825925925925926%*

 * *Differences: {"'dep_lines'": '{insert: [(4, 6), (5, 7)], delete: [4]}',*

 * * "'dep_prios'": '{insert: [(2, 5)]}',*

 * * "'dependencies'": "{insert: [(3, 'sre_constants')]}",*

 * * "'hash'": "'38b6a819e544b584ec71b7040293fae6a77f2447fc14e9bc70e752ec237c8022'",*

 * * "'id'": "'sre_parse'",*

 * * "'interface_hash'": "'14e54a4df7b7598ae3ed25a7fa48a5aee75f5efef703f80ea55a22acfed7f287'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_parse.pyi'",*

 * * "'size'": '4069'}*

```diff
@@ -1,44 +1,47 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         2,
         1,
         3,
         4,
-        5,
+        6,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
         5,
+        5,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
         "re",
+        "sre_constants",
         "typing",
         "typing_extensions",
         "builtins",
         "_typeshed",
         "abc"
     ],
-    "hash": "618be6b2698dc6ca55699bc25bcfe656b87890132abbe027335919112c82a99a",
-    "id": "argparse",
+    "hash": "38b6a819e544b584ec71b7040293fae6a77f2447fc14e9bc70e752ec237c8022",
+    "id": "sre_parse",
     "ignore_all": true,
-    "interface_hash": "950573db8ee28c2bd1dfeb5a32951017483df0332cbdfe95a31faf381ebb5cd5",
-    "mtime": 1685143295,
+    "interface_hash": "14e54a4df7b7598ae3ed25a7fa48a5aee75f5efef703f80ea55a22acfed7f287",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/argparse.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_parse.pyi",
     "plugin_data": null,
-    "size": 19942,
+    "size": 4069,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/array.data.json` & `su6-0.3.0/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/array.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_win32_console.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7026581605528973%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 16), (1, 19), (2, 20), (3, 579), (4, 5), (7, 15), (8, 1), (9, 1), '*

 * *                '(10, 1), (11, 1), (12, 1)], delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 5), (2, 5), (5, 10), (7, 10), (9, 30), (10, 30), (11, 30), (12, '*

 * *                '30), (13, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'ctypes.wintypes'), (1, 'rich.color'), (2, 'rich.style'), (3, "*

 * *                   "'rich.console'), (4, 'ctypes'), (7, 'time'), (9, '_ty […]*

```diff
@@ -1,50 +1,74 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        3,
-        1,
-        2,
+        16,
+        19,
+        20,
+        579,
+        5,
         6,
         7,
+        15,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
         10,
         5,
         5,
         5,
         5,
+        10,
+        5,
+        10,
+        5,
+        30,
+        30,
+        30,
+        30,
+        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
+        "ctypes.wintypes",
+        "rich.color",
+        "rich.style",
+        "rich.console",
+        "ctypes",
         "sys",
-        "_typeshed",
         "typing",
-        "typing_extensions",
+        "time",
         "builtins",
+        "_typeshed",
         "abc",
-        "ctypes",
+        "array",
+        "enum",
+        "functools",
         "mmap",
-        "pickle"
+        "pickle",
+        "rich.color_triplet",
+        "typing_extensions"
     ],
-    "hash": "857e937ecf94979d69f776505b3837900fb0898aee25681aec6aecea918cecf7",
-    "id": "array",
+    "hash": "f8db5e6a5b105d0e79f1efb3a49b64c21f31fdda82f928e500603cef674613a5",
+    "id": "rich._win32_console",
     "ignore_all": true,
-    "interface_hash": "e74f43bcf6812ded0e30399199d4635c9bc9566bf7e4a36c46596db0efe00fdd",
-    "mtime": 1685143295,
+    "interface_hash": "4f75d220b2446d31efd07881418ba81ada3c0c96c6cd26363ae6f0a214580e8e",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -78,13 +102,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/array.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_win32_console.py",
     "plugin_data": null,
-    "size": 3717,
+    "size": 22784,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/ast.data.json` & `su6-0.3.0/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/ast.meta.json` & `su6-0.3.0/.mypy_cache/3.11/ast.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -45,15 +45,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "9c9e46f14b4a591961817f550985f69228acfe5cd12cc83b39dcc143acbb798e",
     "id": "ast",
     "ignore_all": true,
     "interface_hash": "e5c60e38dc2db9261f0af7147b7d365cc9f7056831c602e2c55e5fc901d849f6",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/builtins.data.json` & `su6-0.3.0/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/builtins.meta.json` & `su6-0.3.0/.mypy_cache/3.11/builtins.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -51,15 +51,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "c40d372b9738999cc202708777b2205bbb3a183ed81fd5bb2814e1527ca6bbe1",
     "id": "builtins",
     "ignore_all": true,
     "interface_hash": "15f9ce52026184585df9055fa8dd98cc4a7227a20dc0a648ba67143efda8eb29",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/codecs.data.json` & `su6-0.3.0/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/codecs.meta.json` & `su6-0.3.0/.mypy_cache/3.11/codecs.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -45,15 +45,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "abcdbf8e98a1d1dcc78b663b26b2c59e461cc46b1fc60fda37f079266e35df68",
     "id": "codecs",
     "ignore_all": true,
     "interface_hash": "d28f2525cd97a74da3f27dd2f29dee3427468790c4ae1b17dcad5000d2b882ac",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/colorsys.data.json` & `su6-0.3.0/.mypy_cache/3.11/colorsys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/colorsys.meta.json` & `su6-0.3.0/.mypy_cache/3.11/colorsys.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -15,15 +15,15 @@
         "abc",
         "typing"
     ],
     "hash": "a359a986bd38d55896d08c3e762608dfa737c133f60fcc77299f688b6fd23e80",
     "id": "colorsys",
     "ignore_all": true,
     "interface_hash": "f497588ae10d265ac425ec335a3f20125846f3d5dd70e896e13f23379da19950",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/configparser.data.json` & `su6-0.3.0/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/configparser.meta.json` & `su6-0.3.0/.mypy_cache/3.11/configparser.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -33,15 +33,15 @@
         "abc",
         "os"
     ],
     "hash": "fe331b4b387055ec377ff100800899afa3534646dabd7cda11379590ab7c0b0b",
     "id": "configparser",
     "ignore_all": true,
     "interface_hash": "b31e83e5097e4682674d09b460655966cc62863839ad37a99b7562e921ff3cb9",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/contextlib.data.json` & `su6-0.3.0/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/contextlib.meta.json` & `su6-0.3.0/.mypy_cache/3.11/warnings.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7517715617715618%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 3), (3, 4), (4, 5), (6, 1), (7, 1)], delete: [6, 5, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(7, 30), (8, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(2, '_warnings'), (7, '_typeshed'), (8, 'abc')], delete: [3, 1]}",*

 * * "'hash'": "'9a991da6c7cb550f45efd87385ec22f61a45c69511ab3af2594b6d1ce0487343'",*

 * * "'id'": "'warnings'",*

 * * "'interface_hash'": "'a2c670fd5bdd0dedfd8034ac63ff7a45aefb3014858e5188b2f96cec862ca4ac'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-c […]*

```diff
@@ -1,44 +1,47 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        5,
+        3,
         1,
         2,
-        3,
+        4,
+        5,
         6,
-        7,
-        8,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
-        5,
         10,
         5,
         5,
         5,
         5,
-        5
+        5,
+        30,
+        30
     ],
     "dependencies": [
         "collections.abc",
-        "abc",
         "sys",
-        "_typeshed",
+        "_warnings",
         "types",
         "typing",
         "typing_extensions",
-        "builtins"
+        "builtins",
+        "_typeshed",
+        "abc"
     ],
-    "hash": "c4656ab0b855c3aed90b09036223336af2d28ce8f7b002882c0cd4971d758511",
-    "id": "contextlib",
+    "hash": "9a991da6c7cb550f45efd87385ec22f61a45c69511ab3af2594b6d1ce0487343",
+    "id": "warnings",
     "ignore_all": true,
-    "interface_hash": "089d84d23bdd14c45d68f871f8d4896a74017a2ad540b58c2fdf81c057f81142",
-    "mtime": 1685143295,
+    "interface_hash": "a2c670fd5bdd0dedfd8034ac63ff7a45aefb3014858e5188b2f96cec862ca4ac",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/contextlib.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/warnings.pyi",
     "plugin_data": null,
-    "size": 8986,
+    "size": 3682,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/copy.data.json` & `su6-0.3.0/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/copy.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_timer.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 6), (1, 8), (2, 9)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (4, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'time'), (1, 'contextlib'), (4, '_typeshed')]}",*

 * * "'hash'": "'cde9716d3ea83c566736bc163e973592d51e013f957387ee15c4592d018bb4c2'",*

 * * "'id'": "'rich._timer'",*

 * * "'interface_hash'": "'bfdd6c20b7ecfcd57c73148117aefe0872f821c646cd5582579b33fad184e569'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_timer.p […]*

```diff
@@ -1,29 +1,38 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        6,
+        8,
+        9,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
         5,
+        5,
+        30,
         30
     ],
     "dependencies": [
+        "time",
+        "contextlib",
         "typing",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "891dbbc4965fc233e2f13e2c8f79729c2bfce84a3f6f841f77ab43efd675ee7d",
-    "id": "copy",
+    "hash": "cde9716d3ea83c566736bc163e973592d51e013f957387ee15c4592d018bb4c2",
+    "id": "rich._timer",
     "ignore_all": true,
-    "interface_hash": "475ff08feca909613d4745917797bea89365cd187492138f8a470792b5b8cb58",
-    "mtime": 1685143295,
+    "interface_hash": "bfdd6c20b7ecfcd57c73148117aefe0872f821c646cd5582579b33fad184e569",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/copy.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_timer.py",
     "plugin_data": null,
-    "size": 350,
+    "size": 417,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/csv.data.json` & `su6-0.3.0/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/csv.meta.json` & `su6-0.3.0/.mypy_cache/3.11/csv.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -30,15 +30,15 @@
         "builtins",
         "abc"
     ],
     "hash": "9d8fca202e5ddcea1a8240fe3e17fcbf6ce5841f1661689bca55abe3200192ca",
     "id": "csv",
     "ignore_all": true,
     "interface_hash": "052057dc8e5145a786530cf0cb849d2c9ac8e25894c07e5aa312c538e1e214d2",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/dataclasses.data.json` & `su6-0.3.0/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/dataclasses.meta.json` & `su6-0.3.0/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -33,15 +33,15 @@
         "typing_extensions",
         "abc"
     ],
     "hash": "3c60aa626a823ecffdf68a8e1856506b8ebdd4c073cff06364b4f619e489b5a9",
     "id": "dataclasses",
     "ignore_all": true,
     "interface_hash": "954bae89e71c06ea0a24fa150501b5f9a6382f08dc8c8d3c27912d3db47b2c9c",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/datetime.data.json` & `su6-0.3.0/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/datetime.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.730952380952381%*

 * *Differences: {"'dep_lines'": '{delete: [4, 3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(1, 30)], delete: [4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'builtins')], delete: [6, 5, 4, 2, 0]}",*

 * * "'hash'": "'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'",*

 * * "'id'": "'markdown_it.common'",*

 * * "'interface_hash'": "'025d277b435885d2ab21746beda078a54170d7202b39271c651ced3c454e2915'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/common […]*

```diff
@@ -1,41 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        2,
-        3,
-        4,
-        5,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
-        5,
-        5,
-        5,
         5,
+        30,
         30
     ],
     "dependencies": [
-        "sys",
-        "abc",
-        "time",
-        "typing",
-        "typing_extensions",
         "builtins",
-        "_typeshed"
+        "abc",
+        "typing"
     ],
-    "hash": "0c60f43831b1f7d0abcfb453bf4fcc2d42dc7a37ad8ffe0d7344f047a6ecb87e",
-    "id": "datetime",
+    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
+    "id": "markdown_it.common",
     "ignore_all": true,
-    "interface_hash": "528f62badeb1a9d3c4aa6851fbf55bccea9c5a718ce08b5cd4d3cf20efd41ffd",
-    "mtime": 1685143295,
+    "interface_hash": "025d277b435885d2ab21746beda078a54170d7202b39271c651ced3c454e2915",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/datetime.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/common/__init__.py",
     "plugin_data": null,
-    "size": 11534,
+    "size": 0,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/decimal.data.json` & `su6-0.3.0/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/decimal.meta.json` & `su6-0.3.0/.mypy_cache/3.11/email/charset.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7533333333333334%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc')], delete: [0]}",*

 * * "'hash'": "'7eb946e66f91d483704797cfcbe5603351fd555cb7655a0e5444e653fcd491d7'",*

 * * "'id'": "'email.charset'",*

 * * "'interface_hash'": "'2de97f403307003b2dcb8e652f6e41c2bb8efe58ff05e6839a0b41b5a4720686'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/charset.pyi'",*

 * * "'size'": '1077'}*

```diff
@@ -1,32 +1,32 @@
 {
-    "data_mtime": 1685143684,
+    "data_mtime": 1685143683,
     "dep_lines": [
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "_decimal",
+        "collections.abc",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "3af726e9b7292d9cb1396aeb99d9d991d615541e03459cf2265298543cb29e69",
-    "id": "decimal",
+    "hash": "7eb946e66f91d483704797cfcbe5603351fd555cb7655a0e5444e653fcd491d7",
+    "id": "email.charset",
     "ignore_all": true,
-    "interface_hash": "2247da24f493604d4e8f80d6685ea905f459273fef13c22011cdd98f6b12cc55",
-    "mtime": 1685143295,
+    "interface_hash": "2de97f403307003b2dcb8e652f6e41c2bb8efe58ff05e6839a0b41b5a4720686",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/decimal.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/charset.pyi",
     "plugin_data": null,
-    "size": 117,
+    "size": 1077,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/difflib.data.json` & `su6-0.3.0/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/difflib.meta.json` & `su6-0.3.0/.mypy_cache/3.11/difflib.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -27,15 +27,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "5d9e951886d13fa0360b66b47c9ecbe97aa42d246e795301f9926abf344bc305",
     "id": "difflib",
     "ignore_all": true,
     "interface_hash": "682e520d6ab811e598a750b2685cdf582ec5aed3c1cbeb801f960110e0af53e4",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/dis.data.json` & `su6-0.3.0/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/dis.meta.json` & `su6-0.3.0/.mypy_cache/3.11/dis.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -33,15 +33,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "d29f5fee5fb560e7554e8bdc2cc65a05992e94838554fa808ee3838971c37085",
     "id": "dis",
     "ignore_all": true,
     "interface_hash": "adc9915ec35ef8a18847d99e038f4e4f7bce077c9ba55861ca157ec2dc17be1f",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/enum.data.json` & `su6-0.3.0/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/enum.meta.json` & `su6-0.3.0/.mypy_cache/3.11/enum.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -30,15 +30,15 @@
         "typing",
         "typing_extensions"
     ],
     "hash": "ed43c787e02aed02cae5cca660012347f2c99e5ea96f4fd79d96d060f4aa5685",
     "id": "enum",
     "ignore_all": true,
     "interface_hash": "118aaa1bd26678e4764f55bc8aeba4f06c06a463d184eb1ee9b2cad9b9f7eee7",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/errno.data.json` & `su6-0.3.0/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/errno.meta.json` & `su6-0.3.0/.mypy_cache/3.11/html/entities.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.76%*

 * *Differences: {"'dep_lines'": '{delete: [1, 0]}',*

 * * "'dep_prios'": '{delete: [1, 0]}',*

 * * "'dependencies'": '{delete: [1, 0]}',*

 * * "'hash'": "'87ee8abb57e93a192d86d8d53172d3915c0a99cfb26706388593771a468b68c8'",*

 * * "'id'": "'html.entities'",*

 * * "'interface_hash'": "'ffd23da68d18ff16bd92ee261d7c3c0a03e5bddad2981e2594a938c17a7f1b68'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/html/entities.pyi'",*

 * * "'size'": '182'}*

```diff
@@ -1,35 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        2,
-        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "bd0401f598c4a64b36aec1483018fe5d595ea6c95bdead83dc5e75db0925a27c",
-    "id": "errno",
+    "hash": "87ee8abb57e93a192d86d8d53172d3915c0a99cfb26706388593771a468b68c8",
+    "id": "html.entities",
     "ignore_all": true,
-    "interface_hash": "e1e65cfbee39cc37932c3082a2d6faa8252a44c9a46d46fbf725ed1021d90fb4",
-    "mtime": 1685143295,
+    "interface_hash": "ffd23da68d18ff16bd92ee261d7c3c0a03e5bddad2981e2594a938c17a7f1b68",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/errno.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/html/entities.pyi",
     "plugin_data": null,
-    "size": 3911,
+    "size": 182,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/fractions.data.json` & `su6-0.3.0/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/fractions.meta.json` & `su6-0.3.0/.mypy_cache/3.11/fractions.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -39,15 +39,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "8920640aa1ef26e4093747df64e273af50a65c28cef9cb693e6feaff46bdfe88",
     "id": "fractions",
     "ignore_all": true,
     "interface_hash": "dca99cd4bb227f0db86a6c78c1b2ffb30f5939ee2a558e9e82680c0deb2c6946",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/functools.data.json` & `su6-0.3.0/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/functools.meta.json` & `su6-0.3.0/.mypy_cache/3.11/shlex.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7565656565656566%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 1), (3, 4), (4, 1)], delete: [5, 4, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 30)], delete: [3, 2]}',*

 * * "'dependencies'": "{insert: [(5, '_typeshed')], delete: [3, 2]}",*

 * * "'hash'": "'b6068708c447c5be5cab55e6b0d9ea628424eac94864658817eaff5f659ce914'",*

 * * "'id'": "'shlex'",*

 * * "'interface_hash'": "'67902f856c36ac4c1bc55d2943b31a004e5ee887f7f237ee716a0d467ac42f48'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/ […]*

```diff
@@ -1,44 +1,41 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        4,
-        1,
         2,
+        1,
         3,
-        5,
-        6,
+        4,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
-        5,
-        5,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "types",
-        "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "a55fc5249be5a8cc7802223683191b924150d000994f1beac88c3134361db0ee",
-    "id": "functools",
+    "hash": "b6068708c447c5be5cab55e6b0d9ea628424eac94864658817eaff5f659ce914",
+    "id": "shlex",
     "ignore_all": true,
-    "interface_hash": "a2e9817a8cb7e0ce65d43b881f11fe770f7d2593f597ff6287e8ca2c06282fb0",
-    "mtime": 1685143295,
+    "interface_hash": "67902f856c36ac4c1bc55d2943b31a004e5ee887f7f237ee716a0d467ac42f48",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/functools.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/shlex.pyi",
     "plugin_data": null,
-    "size": 6712,
+    "size": 1502,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/genericpath.data.json` & `su6-0.3.0/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/genericpath.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_palettes.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6990740740740741%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(1, 1)], delete: [4, 3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.palette'), (3, 'typing')], delete: [4, 3, 2, 1, 0]}",*

 * * "'hash'": "'71d7afd4940a67426f960b95f62a478339d3767be52335050c16f422dd8fce32'",*

 * * "'id'": "'rich._palettes'",*

 * * "'interface_hash'": "'a9a7e508b3c4f8a548b09a97bc8e59ccb7d1c8d4c6301a06adc2593a7b4b12de'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6 […]*

```diff
@@ -1,41 +1,32 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        3,
         1,
-        2,
-        4,
-        5,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
-        5,
         5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "os",
-        "_typeshed",
-        "typing",
-        "typing_extensions",
+        "rich.palette",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "50d45ab3fd6f6adc2a69a00ae4885e0c123e9e773ee3d3366768e99b9e6e8fbd",
-    "id": "genericpath",
+    "hash": "71d7afd4940a67426f960b95f62a478339d3767be52335050c16f422dd8fce32",
+    "id": "rich._palettes",
     "ignore_all": true,
-    "interface_hash": "592081edf3b264e91eeb7bf8e751aaf367fa3108b344596ac367b31465b846dc",
-    "mtime": 1685143295,
+    "interface_hash": "a9a7e508b3c4f8a548b09a97bc8e59ccb7d1c8d4c6301a06adc2593a7b4b12de",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/genericpath.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_palettes.py",
     "plugin_data": null,
-    "size": 1756,
+    "size": 7063,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/getpass.data.json` & `su6-0.3.0/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/getpass.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_windows.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6955555555555556%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 25), (1, 1), (2, 2), (3, 16), (4, 66), (5, 69)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5), (3, 5), (4, 10), (7, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich._win32_console'), (1, 'sys'), (2, 'dataclasses'), (3, "*

 * *                   "'ctypes'), (4, 'platform'), (5, 'rich'), (8, 'typing')], delete: [0]}",*

 * * "'hash'": "'27fae1687ec73377f95ef1f96ec02b18aaa84e88da57c1deb4d2d4275497f48e'",*

 * * "'id'": "'rich._windows'",*

 * * "'interface_hash'":  […]*

```diff
@@ -1,29 +1,47 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
+        25,
+        1,
+        2,
+        16,
+        66,
+        69,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
+        10,
+        5,
         5,
+        30,
         30
     ],
     "dependencies": [
-        "typing",
+        "rich._win32_console",
+        "sys",
+        "dataclasses",
+        "ctypes",
+        "platform",
+        "rich",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "1c755308b5f630e123566d4785ff25d521e2d12de4014056713d1d1f2dbbc19f",
-    "id": "getpass",
+    "hash": "27fae1687ec73377f95ef1f96ec02b18aaa84e88da57c1deb4d2d4275497f48e",
+    "id": "rich._windows",
     "ignore_all": true,
-    "interface_hash": "846d32fa7d3f0ba4c3a00aaa237cf1e4a0e4916fe3c05ebbf1459c9ddef5c98a",
-    "mtime": 1685143295,
+    "interface_hash": "974e41661a343e129a1f46290e766656bdf10299e6f66d27c26a6d0da8c1cabf",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/getpass.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_windows.py",
     "plugin_data": null,
-    "size": 227,
+    "size": 1902,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/gettext.data.json` & `su6-0.3.0/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/gettext.meta.json` & `su6-0.3.0/.mypy_cache/3.11/gettext.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -30,15 +30,15 @@
         "builtins",
         "abc"
     ],
     "hash": "05bcfbfe3e5ba3e16560a69ffaeba02e1e3b810e78532bd08cc44617306fc579",
     "id": "gettext",
     "ignore_all": true,
     "interface_hash": "809447e1d9a1b1061202eac0f3802ad6c09c388b327b0603fd143483d16d3787",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/glob.data.json` & `su6-0.3.0/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/glob.meta.json` & `su6-0.3.0/.mypy_cache/3.11/math.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7642195767195769%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 1), (2, 3), (4, 1)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 30)]}',*

 * * "'dependencies'": "{insert: [(3, 'typing_extensions'), (5, '_typeshed')], delete: [2]}",*

 * * "'hash'": "'7383fb2c7e3a74ef80504a0d82a06ed95c4c7754272c54e89a64f1319ab87732'",*

 * * "'id'": "'math'",*

 * * "'interface_hash'": "'2c3de2e9d8a8d90d40a4e6b21c41d8cfe42421af18310f55a76c4666a70bfd34'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/ […]*

```diff
@@ -1,38 +1,41 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        3,
-        1,
         2,
+        1,
+        3,
         4,
         1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "_typeshed",
         "typing",
+        "typing_extensions",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "b23877cf7cc743ec86f6a87b449a4cc1a92ad72e573a19c7a17a82c3fc3507a2",
-    "id": "glob",
+    "hash": "7383fb2c7e3a74ef80504a0d82a06ed95c4c7754272c54e89a64f1319ab87732",
+    "id": "math",
     "ignore_all": true,
-    "interface_hash": "0b54d93d4031a2a78bad77ffdb5e562a1953657395d23eb1249760d4eff0837f",
-    "mtime": 1685143295,
+    "interface_hash": "2c3de2e9d8a8d90d40a4e6b21c41d8cfe42421af18310f55a76c4666a70bfd34",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/glob.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/math.pyi",
     "plugin_data": null,
-    "size": 1421,
+    "size": 5025,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/inspect.data.json` & `su6-0.3.0/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/inspect.meta.json` & `su6-0.3.0/.mypy_cache/3.11/inspect.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -39,15 +39,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "9b9bc26634b9323492d1abe333418ad1bb84b2bd41bf161b538d0202abb34d8f",
     "id": "inspect",
     "ignore_all": true,
     "interface_hash": "ef7caeaf025c2cf678f25021ea693e52978b499d7c931782f2cca3f12b14eda2",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/io.data.json` & `su6-0.3.0/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/io.meta.json` & `su6-0.3.0/.mypy_cache/3.11/marshal.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7566666666666666%*

 * *Differences: {"'dep_lines'": '{insert: [(5, 1)], delete: [9, 8, 7, 6, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 30)], delete: [6, 5, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(2, '_typeshed'), (5, 'abc')], delete: [6, 5, 4, 3, 1, 0]}",*

 * * "'hash'": "'be1b42745d0d382d1a16406d8a070b3df1507eeb46b26eff9f7ebb3ce528a33e'",*

 * * "'id'": "'marshal'",*

 * * "'interface_hash'": "'87b6f47763c79a3349a3f3e62669dd7bf6de1a0c47a00441a44d77b044426ad3'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-p […]*

```diff
@@ -1,62 +1,50 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        6,
         1,
         2,
         3,
         4,
         5,
-        7,
-        8,
-        9,
-        10,
+        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
         10,
         10,
-        10,
-        10,
-        5,
-        5,
         5,
         5,
         5,
         30,
         30,
         30,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "abc",
         "builtins",
-        "codecs",
-        "sys",
-        "_typeshed",
-        "os",
         "types",
+        "_typeshed",
         "typing",
         "typing_extensions",
+        "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle"
     ],
-    "hash": "0b41ad24faa49ac20e0c8c0d0bf223ff7de8ce8ea44fe01e3a4a2cb1f363054d",
-    "id": "io",
+    "hash": "be1b42745d0d382d1a16406d8a070b3df1507eeb46b26eff9f7ebb3ce528a33e",
+    "id": "marshal",
     "ignore_all": true,
-    "interface_hash": "f9869284f2a5be1f4215bfc4c458a1220d04288cfd924c5156bc82dfd3c84906",
-    "mtime": 1685143295,
+    "interface_hash": "87b6f47763c79a3349a3f3e62669dd7bf6de1a0c47a00441a44d77b044426ad3",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -90,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/io.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/marshal.pyi",
     "plugin_data": null,
-    "size": 7875,
+    "size": 841,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/itertools.data.json` & `su6-0.3.0/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/itertools.meta.json` & `su6-0.3.0/.mypy_cache/3.11/itertools.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -30,15 +30,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "8d452d6d11a70ac8cf92f7f8ca2f0ec391f06ffd520b0a5e9c6083b3efe75b5d",
     "id": "itertools",
     "ignore_all": true,
     "interface_hash": "e17449f9c56774e8827dea124b7d272bdd79086ca33c6199ee6509f6fe37510b",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/linecache.data.json` & `su6-0.3.0/.mypy_cache/3.11/linecache.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/linecache.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/errors.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7428571428571428%*

 * *Differences: {"'dep_lines'": '{delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(2, 'typing')], delete: [4, 2, 1, 0]}",*

 * * "'hash'": "'e693f729ce5de1027f734285b31adfca18e23d57bb275ccea9215b140cdc57e6'",*

 * * "'id'": "'rich.errors'",*

 * * "'interface_hash'": "'534ee3082dbc4ad481e7299060952717c174935b937136d76df876eaf8407f10'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/errors.py'",*

 * * "'size'": '642'}*

```diff
@@ -1,38 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        2,
-        3,
-        1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
-        5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "sys",
-        "typing",
-        "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "1f773c204e1f7123a2f3cafec9d8bb3cf43479274b225843f556667e1908bca1",
-    "id": "linecache",
+    "hash": "e693f729ce5de1027f734285b31adfca18e23d57bb275ccea9215b140cdc57e6",
+    "id": "rich.errors",
     "ignore_all": true,
-    "interface_hash": "a394a279efd903e56d257cc3537d959bb52b584529de0c2b3aa60e3456eaba5d",
-    "mtime": 1685143295,
+    "interface_hash": "534ee3082dbc4ad481e7299060952717c174935b937136d76df876eaf8407f10",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/linecache.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/errors.py",
     "plugin_data": null,
-    "size": 945,
+    "size": 642,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/locale.data.json` & `su6-0.3.0/.mypy_cache/3.11/locale.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/locale.meta.json` & `su6-0.3.0/.mypy_cache/3.11/locale.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/marshal.data.json` & `su6-0.3.0/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/marshal.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_codecs.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7699023199023199%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 4), (5, 6), (6, 1)], delete: [3]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (3, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'codecs'), (2, 'sys'), (6, 'builtins')], "*

 * *                   'delete: [1, 0]}',*

 * * "'hash'": "'70e3defc1875bd08c24cbe869d9c14280401dc8b591637db091aad6a71684e1d'",*

 * * "'id'": "'_codecs'",*

 * * "'interface_hash'": "'b46b35bd03ec1cc9344093253180c85f42512ae908969e157e6619fb188b42f0'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6- […]*

```diff
@@ -1,50 +1,56 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        4,
         1,
         2,
         3,
-        4,
         5,
+        6,
+        1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
         10,
         10,
         5,
         5,
         5,
+        5,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "builtins",
-        "types",
+        "collections.abc",
+        "codecs",
+        "sys",
         "_typeshed",
         "typing",
         "typing_extensions",
+        "builtins",
         "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle"
     ],
-    "hash": "be1b42745d0d382d1a16406d8a070b3df1507eeb46b26eff9f7ebb3ce528a33e",
-    "id": "marshal",
+    "hash": "70e3defc1875bd08c24cbe869d9c14280401dc8b591637db091aad6a71684e1d",
+    "id": "_codecs",
     "ignore_all": true,
-    "interface_hash": "87b6f47763c79a3349a3f3e62669dd7bf6de1a0c47a00441a44d77b044426ad3",
-    "mtime": 1685143295,
+    "interface_hash": "b46b35bd03ec1cc9344093253180c85f42512ae908969e157e6619fb188b42f0",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -78,13 +84,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/marshal.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_codecs.pyi",
     "plugin_data": null,
-    "size": 841,
+    "size": 7280,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/math.data.json` & `su6-0.3.0/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/math.meta.json` & `su6-0.3.0/.mypy_cache/3.11/pickle.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7554040404040404%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 1), (2, 2), (4, 5), (5, 1), (6, 1)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 5), (6, 30), (7, 30)]}',*

 * * "'dependencies'": "{insert: [(2, '_typeshed'), (7, 'array'), (8, 'ctypes'), (9, 'mmap')], delete: "*

 * *                   '[5]}',*

 * * "'hash'": "'01215def75497e54bbe02f50a7b531a9884a9939582b42a2ddf2348b7c8e9d94'",*

 * * "'id'": "'pickle'",*

 * * "'interface_hash'": "'cfbe426adb1182a1f1e9c4585ad054bb30bd9ba84b029df30a91851fb63ee5a6'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robi […]*

```diff
@@ -1,41 +1,50 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        2,
-        1,
         3,
+        1,
+        2,
         4,
+        5,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
+        5,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
+        "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "array",
+        "ctypes",
+        "mmap"
     ],
-    "hash": "7383fb2c7e3a74ef80504a0d82a06ed95c4c7754272c54e89a64f1319ab87732",
-    "id": "math",
+    "hash": "01215def75497e54bbe02f50a7b531a9884a9939582b42a2ddf2348b7c8e9d94",
+    "id": "pickle",
     "ignore_all": true,
-    "interface_hash": "2c3de2e9d8a8d90d40a4e6b21c41d8cfe42421af18310f55a76c4666a70bfd34",
-    "mtime": 1685143295,
+    "interface_hash": "cfbe426adb1182a1f1e9c4585ad054bb30bd9ba84b029df30a91851fb63ee5a6",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/math.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/pickle.pyi",
     "plugin_data": null,
-    "size": 5025,
+    "size": 6764,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/mmap.data.json` & `su6-0.3.0/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/mmap.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/globals.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7373737373737373%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 6)], delete: [7, 6, 5, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 25), (3, 25)], delete: [8, 7, 6, 3, 2, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'click.core'), (2, 'threading')], delete: [9, 8, 7, 2, 1, 0]}",*

 * * "'hash'": "'4cffaa33cf124f373b7f5dbb877e530ffbfddb41607ce0f6130cea034a04f175'",*

 * * "'id'": "'click.globals'",*

 * * "'interface_hash'": "'ea4004205ca0c1c53556d83cbdae280ff0dd68081faaeeb251669dbd6fa04017'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-chec […]*

```diff
@@ -1,49 +1,37 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        3,
+        6,
         1,
         2,
-        4,
         5,
         1,
-        1,
-        1,
-        1,
         1
     ],
     "dep_prios": [
-        5,
+        25,
         10,
         5,
+        25,
         5,
-        5,
-        5,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
-        "_typeshed",
+        "click.core",
         "typing",
+        "threading",
         "typing_extensions",
         "builtins",
-        "abc",
-        "array",
-        "ctypes",
-        "pickle"
+        "abc"
     ],
-    "hash": "d9e78f0946bc6297002b245e9d85b5be1bcfe36b9a503843f57923c1574200ea",
-    "id": "mmap",
+    "hash": "4cffaa33cf124f373b7f5dbb877e530ffbfddb41607ce0f6130cea034a04f175",
+    "id": "click.globals",
     "ignore_all": true,
-    "interface_hash": "4826eca11c6294e24662f5d0ea3aeb5050023b4d7584ca360d81eca7a5d7a39d",
+    "interface_hash": "ea4004205ca0c1c53556d83cbdae280ff0dd68081faaeeb251669dbd6fa04017",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -78,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/mmap.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/click/globals.py",
     "plugin_data": null,
-    "size": 4009,
+    "size": 1961,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/msvcrt.data.json` & `su6-0.3.0/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/msvcrt.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/utils.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7396296296296296%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 3), (2, 4), (3, 1), (4, 1)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (4, 30), (5, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, '__future__'), (2, 'pathlib'), (5, "*

 * *                   "'os'), (7, 'typing_extensions')], delete: [1, 0]}",*

 * * "'hash'": "'7e50fb1929681b26c48175d5684df528a9b00250704a6177e5de131a67febabf'",*

 * * "'id'": "'markdown_it.utils'",*

 * * "'interface_hash'": "'8335636d49a8bfa20d8496a08427c175714de0547c045ada302dee9e3 […]*

```diff
@@ -1,35 +1,44 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        3,
+        1,
+        4,
+        1,
         1,
-        2,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
         5,
         5,
+        5,
+        5,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "sys",
-        "typing_extensions",
+        "collections.abc",
+        "__future__",
+        "pathlib",
         "builtins",
         "abc",
-        "typing"
+        "os",
+        "typing",
+        "typing_extensions"
     ],
-    "hash": "d4a762dc87ddb7286da0abdb399dec04efb82a19579a4ef11af621851da7b598",
-    "id": "msvcrt",
+    "hash": "7e50fb1929681b26c48175d5684df528a9b00250704a6177e5de131a67febabf",
+    "id": "markdown_it.utils",
     "ignore_all": true,
-    "interface_hash": "9c3d3ffaec1b81ce2404515a91e464cc85aa699821a8db83958c5e1a7001082c",
-    "mtime": 1685143295,
+    "interface_hash": "8335636d49a8bfa20d8496a08427c175714de0547c045ada302dee9e385bebc9",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/msvcrt.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/utils.py",
     "plugin_data": null,
-    "size": 995,
+    "size": 3262,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/numbers.data.json` & `su6-0.3.0/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/numbers.meta.json` & `su6-0.3.0/.mypy_cache/3.11/__future__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7322222222222223%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 1), (1, 1), (2, 1)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 30), (3, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'typing_extensions'), (1, 'builtins')], delete: [2]}",*

 * * "'hash'": "'a88c160e68dac375c28ae94a628281401fde2632f1c1e7ac50ac017699204245'",*

 * * "'id'": "'__future__'",*

 * * "'interface_hash'": "'785a6eda02f10c252e25c75d49899c617f4a50f56ab17aa5d128094494bb6647'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/s […]*

```diff
@@ -1,29 +1,32 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        4,
-        5,
+        1,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5
+        30,
+        30
     ],
     "dependencies": [
+        "typing_extensions",
+        "builtins",
         "abc",
-        "typing",
-        "builtins"
+        "typing"
     ],
-    "hash": "aa29ea52bc87c75f589211fa38294e2cc1bc735c97f4fa331ebaff28e5f2cb84",
-    "id": "numbers",
+    "hash": "a88c160e68dac375c28ae94a628281401fde2632f1c1e7ac50ac017699204245",
+    "id": "__future__",
     "ignore_all": true,
-    "interface_hash": "73479f60f40dd74ecc1b17ddb3686ec0848505c1e59ff61c46c3c55a1919cf16",
-    "mtime": 1685143295,
+    "interface_hash": "785a6eda02f10c252e25c75d49899c617f4a50f56ab17aa5d128094494bb6647",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/numbers.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/__future__.pyi",
     "plugin_data": null,
-    "size": 3914,
+    "size": 915,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/opcode.data.json` & `su6-0.3.0/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/opcode.meta.json` & `su6-0.3.0/.mypy_cache/3.11/opcode.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -24,15 +24,15 @@
         "abc",
         "typing"
     ],
     "hash": "59c0a8b72408537be5d42d12987309aac4a2d17dc740d1d3c2d88732320749e1",
     "id": "opcode",
     "ignore_all": true,
     "interface_hash": "b76c7988f1431faf887cccd5df7e17f46b561f99be1ddf1e6d6e0f94151bf422",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/operator.data.json` & `su6-0.3.0/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/operator.meta.json` & `su6-0.3.0/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7564814814814814%*

 * *Differences: {"'dep_lines'": '{insert: [(2, 3)], delete: [3, 2]}',*

 * * "'dep_prios'": '{insert: [(3, 5)], delete: [4, 3]}',*

 * * "'dependencies'": "{insert: [(1, 'typing'), (2, 'typing_extensions')], delete: [6, 5, 1]}",*

 * * "'hash'": "'cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c'",*

 * * "'id'": "'sre_constants'",*

 * * "'interface_hash'": "'9712b3c3ae06b67272c232e1379bf306d8606ccbd5bb6d332f741942b043edb8'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/myp […]*

```diff
@@ -1,41 +1,38 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
         2,
-        1,
-        1,
+        3,
         1,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
         5,
-        30,
-        30,
+        5,
         30,
         30
     ],
     "dependencies": [
         "sys",
-        "_operator",
+        "typing",
+        "typing_extensions",
         "builtins",
         "_typeshed",
-        "abc",
-        "typing",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "b5874dad84073d6251c60f2da6aded0683c8cf18d7369e3f606cd1787d383625",
-    "id": "operator",
+    "hash": "cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c",
+    "id": "sre_constants",
     "ignore_all": true,
-    "interface_hash": "971937d4b9dd70d103f8fc675639a947014d5791ef8704d631c2b61d235e4bf3",
-    "mtime": 1685143295,
+    "interface_hash": "9712b3c3ae06b67272c232e1379bf306d8606ccbd5bb6d332f741942b043edb8",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/operator.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_constants.pyi",
     "plugin_data": null,
-    "size": 1644,
+    "size": 3986,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/pathlib.data.json` & `su6-0.3.0/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/pathlib.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/parser.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7389328063241106%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 29), (1, 36), (2, 24), (3, 25), (4, 26), (5, 35), (6, 140), (7, '*

 * *                '395), (9, 1)], delete: [7, 6, 5, 4, 3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 25), (5, 25), (6, 20), (7, 20), (9, 30), (10, 30)], delete: [5, 4, '*

 * *                '3, 2]}',*

 * * "'dependencies'": "{insert: [(0, 'click.exceptions'), (1, 'click.core'), (3, 'collections'), (4, "*

 * *                   "'gettext'), (6, 'shlex'), (7, 'difflib'), (9, '_typeshed'), (15, 'types') […]*

```diff
@@ -1,61 +1,67 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        12,
+        29,
+        36,
+        24,
+        25,
+        26,
+        35,
+        140,
+        395,
+        1,
         1,
-        2,
-        13,
-        14,
-        15,
-        16,
-        17,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        25,
         10,
         5,
         5,
-        5,
-        5,
-        5,
-        5,
+        25,
+        20,
+        20,
         5,
         30,
         30,
         30,
         30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
-        "_typeshed",
-        "io",
-        "os",
-        "types",
+        "click.exceptions",
+        "click.core",
         "typing",
+        "collections",
+        "gettext",
         "typing_extensions",
+        "shlex",
+        "difflib",
         "builtins",
+        "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
-        "pickle"
+        "pickle",
+        "types"
     ],
-    "hash": "af5d9944e5c7afe3dd4c99f5d83d4950e1d88bbcaba5db66ac57f946b5d10f41",
-    "id": "pathlib",
+    "hash": "70012dd6e411f20ab7f92f72b2a6d553e7dd01936f8a5c70e11789fd3d4e40c9",
+    "id": "click.parser",
     "ignore_all": true,
-    "interface_hash": "bd4e7f6edf566926f7480e2946c15d13f167e2f912a9a794c2f7c1067a8fad80",
+    "interface_hash": "7d71318c773f103c9de02366cb3b6ad6aa171a08f00d26c380488086111d7e4a",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -90,13 +96,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/pathlib.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/click/parser.py",
     "plugin_data": null,
-    "size": 7949,
+    "size": 19044,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/pickle.data.json` & `su6-0.3.0/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/pickle.meta.json` & `su6-0.3.0/.mypy_cache/3.11/threading.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7583333333333333%*

 * *Differences: {"'dep_lines'": '{insert: [(5, 6), (6, 51)], delete: [7, 6, 5]}',*

 * * "'dep_prios'": '{insert: [(6, 5), (7, 5)], delete: [8, 7, 6]}',*

 * * "'dependencies'": "{insert: [(3, 'types'), (6, '_thread')], delete: [9, 8, 7]}",*

 * * "'hash'": "'f2c4bdcb0b9cbdadb0c49fa600420d90019d83e6854d3a5a5aafd988fe3cd378'",*

 * * "'id'": "'threading'",*

 * * "'interface_hash'": "'aa82688d3c03b586c022cf1142ca5632a48efc591fa0b627211e885f1fd85f23'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-pack […]*

```diff
@@ -2,49 +2,46 @@
     "data_mtime": 1685143683,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
-        1,
-        1,
-        1,
+        6,
+        51,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
         5,
-        30,
-        30,
-        30,
+        5,
+        5,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
         "_typeshed",
+        "types",
         "typing",
         "typing_extensions",
+        "_thread",
         "builtins",
-        "abc",
-        "array",
-        "ctypes",
-        "mmap"
+        "abc"
     ],
-    "hash": "01215def75497e54bbe02f50a7b531a9884a9939582b42a2ddf2348b7c8e9d94",
-    "id": "pickle",
+    "hash": "f2c4bdcb0b9cbdadb0c49fa600420d90019d83e6854d3a5a5aafd988fe3cd378",
+    "id": "threading",
     "ignore_all": true,
-    "interface_hash": "cfbe426adb1182a1f1e9c4585ad054bb30bd9ba84b029df30a91851fb63ee5a6",
-    "mtime": 1685143295,
+    "interface_hash": "aa82688d3c03b586c022cf1142ca5632a48efc591fa0b627211e885f1fd85f23",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -78,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/pickle.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/threading.pyi",
     "plugin_data": null,
-    "size": 6764,
+    "size": 6028,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/platform.data.json` & `su6-0.3.0/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/platform.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7904761904761906%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 2), (2, 3), (3, 1)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (4, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'textwrap'), (2, 'contextlib'), (6, 'typing_extensions')], "*

 * *                   'delete: [0]}',*

 * * "'hash'": "'d747d0eb839c05432e2bb985be1f37eb7feea0ec4f95122d64198acd12438286'",*

 * * "'id'": "'click._textwrap'",*

 * * "'interface_hash'": "'90f3db3ff0c60035a0c3f5c1fbeac280a4736bc3d493e18fe767f2cb7a77f86e'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3. […]*

```diff
@@ -1,34 +1,40 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        7,
+        2,
+        3,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         10,
+        10,
         5,
         5,
         30,
+        30,
         30
     ],
     "dependencies": [
-        "sys",
+        "textwrap",
         "typing",
+        "contextlib",
         "builtins",
         "_typeshed",
-        "abc"
+        "abc",
+        "typing_extensions"
     ],
-    "hash": "20e99509f6e765e56fea8ebf9375e15695f123fdc0af99ca50e323efd17ebc44",
-    "id": "platform",
+    "hash": "d747d0eb839c05432e2bb985be1f37eb7feea0ec4f95122d64198acd12438286",
+    "id": "click._textwrap",
     "ignore_all": true,
-    "interface_hash": "530d2c958c1822755594b66ea896cb0b8e7b2133dd9ea8d023129d8b044b0af7",
+    "interface_hash": "90f3db3ff0c60035a0c3f5c1fbeac280a4736bc3d493e18fe767f2cb7a77f86e",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -63,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/platform.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/click/_textwrap.py",
     "plugin_data": null,
-    "size": 2375,
+    "size": 1353,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/posixpath.data.json` & `su6-0.3.0/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/posixpath.meta.json` & `su6-0.3.0/.mypy_cache/3.11/posixpath.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -33,15 +33,15 @@
         "builtins",
         "abc"
     ],
     "hash": "e29af0b8d907ad14fb6a1be8ff951377d80ecca2f14c39f13e7d9b0b5727e530",
     "id": "posixpath",
     "ignore_all": true,
     "interface_hash": "c3eb6062528f32b8c6e747dd67a9572e9c6bfbf6c6bdda30d182323b4089e3f1",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/pty.data.json` & `su6-0.3.0/.mypy_cache/3.11/pty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/pty.meta.json` & `su6-0.3.0/.mypy_cache/3.11/pty.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -27,15 +27,15 @@
         "os",
         "typing"
     ],
     "hash": "a73e8c91fda30bffb85408395e397c4ad633ec0b265451febb9ace41ef26ae87",
     "id": "pty",
     "ignore_all": true,
     "interface_hash": "18bdacd7fc4bb09bf75854a8732014b9e1e1d0dca6f0f5b9bc1c2d3e6066fd01",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/pydoc.data.json` & `su6-0.3.0/.mypy_cache/3.11/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/pydoc.meta.json` & `su6-0.3.0/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.727979797979798%*

 * *Differences: {"'dep_lines'": '{insert: [(3, 1), (4, 1)], delete: [8, 7, 6, 5, 4, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 30)], delete: [4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 're'), (3, 'builtins'), (4, 'abc')], delete: [8, 6, 5, 4, 3, 2, "*

 * *                   '1]}',*

 * * "'hash'": "'0c53d66512d44e95d7981a43ef5d83801a9e12c6aaa65b05a35074fecb1ef07f'",*

 * * "'id'": "'json.encoder'",*

 * * "'interface_hash'": "'5e7ae11c6ee6936f28efa0e308818439ac6cd408e83858317d2b9037426bb289'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robi […]*

```diff
@@ -1,47 +1,35 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        5,
         1,
         2,
         3,
-        4,
-        6,
-        7,
-        8,
-        9
+        1,
+        1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
         5,
         5,
         5,
-        5,
-        5
+        30
     ],
     "dependencies": [
         "collections.abc",
-        "sys",
-        "_typeshed",
-        "abc",
-        "builtins",
-        "reprlib",
-        "types",
+        "re",
         "typing",
-        "typing_extensions"
+        "builtins",
+        "abc"
     ],
-    "hash": "a5b9fc8f7d48fde0a812a953344848dea1b6208d66a6982cd1bd378be309e395",
-    "id": "pydoc",
+    "hash": "0c53d66512d44e95d7981a43ef5d83801a9e12c6aaa65b05a35074fecb1ef07f",
+    "id": "json.encoder",
     "ignore_all": true,
-    "interface_hash": "4f9b07c1646cb983b9add257b6935f65c646ea35ed72fa25a6814a8113127759",
-    "mtime": 1685143295,
+    "interface_hash": "5e7ae11c6ee6936f28efa0e308818439ac6cd408e83858317d2b9037426bb289",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -75,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/pydoc.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/encoder.pyi",
     "plugin_data": null,
-    "size": 10392,
+    "size": 1073,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/random.data.json` & `su6-0.3.0/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/random.meta.json` & `su6-0.3.0/.mypy_cache/3.11/random.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -33,15 +33,15 @@
         "abc",
         "numbers"
     ],
     "hash": "cd0376273b30c0297134c77768237d572ecd19d309a415d628265d2a817b39e8",
     "id": "random",
     "ignore_all": true,
     "interface_hash": "bb0083b1cf5d7d23692a1075e6b97e7c47d955457f5f32afdd0ade4c6dc30440",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/re.data.json` & `su6-0.3.0/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/re.meta.json` & `su6-0.3.0/.mypy_cache/3.11/re.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -51,15 +51,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "6628a0287263a0a91b274aea7dce328361b557f6249454c8f92f79af56500fbe",
     "id": "re",
     "ignore_all": true,
     "interface_hash": "790255c3f35b5de88f7eb480b28d58dc0ccaec4619989ebe4474adf9a422c70c",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/reprlib.data.json` & `su6-0.3.0/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/reprlib.meta.json` & `su6-0.3.0/.mypy_cache/3.11/functools.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7774410774410775%*

 * *Differences: {"'dep_lines'": '{delete: [6]}',*

 * * "'dep_prios'": '{delete: [7]}',*

 * * "'dependencies'": "{insert: [(2, 'types'), (3, '_typeshed')], delete: [7, 3, 2]}",*

 * * "'hash'": "'a55fc5249be5a8cc7802223683191b924150d000994f1beac88c3134361db0ee'",*

 * * "'id'": "'functools'",*

 * * "'interface_hash'": "'a2e9817a8cb7e0ce65d43b881f11fe770f7d2593f597ff6287e8ca2c06282fb0'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/functools.pyi'",*

 * * "'size'": '6712'}*

```diff
@@ -4,44 +4,41 @@
         4,
         1,
         2,
         3,
         5,
         6,
         1,
-        1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "array",
-        "collections",
+        "types",
+        "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "bac2ab52145c08d78e55d632dd2e88f278d13915c843dad7ac699ed34b8625de",
-    "id": "reprlib",
+    "hash": "a55fc5249be5a8cc7802223683191b924150d000994f1beac88c3134361db0ee",
+    "id": "functools",
     "ignore_all": true,
-    "interface_hash": "2eb446a6a81cfec3b4a0186b8ae767f2e8cd8c96d9e9e750fefe61aa857d5260",
-    "mtime": 1685143295,
+    "interface_hash": "a2e9817a8cb7e0ce65d43b881f11fe770f7d2593f597ff6287e8ca2c06282fb0",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -75,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/reprlib.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/functools.pyi",
     "plugin_data": null,
-    "size": 1986,
+    "size": 6712,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/shlex.data.json` & `su6-0.3.0/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/shlex.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.736904761904762%*

 * *Differences: {"'dep_lines'": '{delete: [3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(2, 'typing')], delete: [5, 3, 2, 1, 0]}",*

 * * "'hash'": "'86ed552fd9db55da6926b5688a356c85195c4517bfbf7763bb7326776b0a65d6'",*

 * * "'id'": "'rich._emoji_codes'",*

 * * "'interface_hash'": "'3349b076d76c590dd6f9a7ca1c913093d5f7d0c64dc7590e5659121cc9b78246'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_emoji_codes.py'",*

 * * "'size'": '140235' […]*

```diff
@@ -1,41 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        2,
-        1,
-        3,
-        4,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
-        "typing",
-        "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "b6068708c447c5be5cab55e6b0d9ea628424eac94864658817eaff5f659ce914",
-    "id": "shlex",
+    "hash": "86ed552fd9db55da6926b5688a356c85195c4517bfbf7763bb7326776b0a65d6",
+    "id": "rich._emoji_codes",
     "ignore_all": true,
-    "interface_hash": "67902f856c36ac4c1bc55d2943b31a004e5ee887f7f237ee716a0d467ac42f48",
-    "mtime": 1685143295,
+    "interface_hash": "3349b076d76c590dd6f9a7ca1c913093d5f7d0c64dc7590e5659121cc9b78246",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/shlex.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_emoji_codes.py",
     "plugin_data": null,
-    "size": 1502,
+    "size": 140235,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/shutil.data.json` & `su6-0.3.0/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/shutil.meta.json` & `su6-0.3.0/.mypy_cache/3.11/operator.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7363636363636364%*

 * *Differences: {"'dep_lines'": '{insert: [(2, 1), (3, 1), (4, 1)], delete: [5, 4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 30), (4, 30), (5, 30)], delete: [4, 3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, '_operator'), (2, 'builtins'), (4, 'abc')], delete: [7, 6, 1, "*

 * *                   '0]}',*

 * * "'hash'": "'b5874dad84073d6251c60f2da6aded0683c8cf18d7369e3f606cd1787d383625'",*

 * * "'id'": "'operator'",*

 * * "'interface_hash'": "'971937d4b9dd70d103f8fc675639a947014d5791ef8704d631c2b61d235e4bf3'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": " […]*

```diff
@@ -1,44 +1,41 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        4,
         1,
         2,
-        3,
-        5,
-        6,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
-        5,
         10,
-        10,
-        5,
-        5,
         5,
         5,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "os",
         "sys",
+        "_operator",
+        "builtins",
         "_typeshed",
+        "abc",
         "typing",
-        "typing_extensions",
-        "builtins",
-        "abc"
+        "typing_extensions"
     ],
-    "hash": "14a2bb451d6170f6e211ac293eed7182c2d925a35b3c28b0bb5509c21bf1a000",
-    "id": "shutil",
+    "hash": "b5874dad84073d6251c60f2da6aded0683c8cf18d7369e3f606cd1787d383625",
+    "id": "operator",
     "ignore_all": true,
-    "interface_hash": "57656da15158dbdecfaa2bfd4ddccf69e5796d41dc9c0e81fc787cb985d96f80",
-    "mtime": 1685143295,
+    "interface_hash": "971937d4b9dd70d103f8fc675639a947014d5791ef8704d631c2b61d235e4bf3",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/shutil.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/operator.pyi",
     "plugin_data": null,
-    "size": 6658,
+    "size": 1644,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/sre_compile.data.json` & `su6-0.3.0/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/sre_compile.meta.json` & `su6-0.3.0/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -24,15 +24,15 @@
         "builtins",
         "abc"
     ],
     "hash": "c9cd67b263730096df01415a2933288a4f7d800e1380fc31f76bb1e39af65440",
     "id": "sre_compile",
     "ignore_all": true,
     "interface_hash": "0c5d3388f39ecbe1463dedac85f0a27794d3f1dd40107c3b29cb269058107429",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/sre_constants.data.json` & `su6-0.3.0/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/sre_constants.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_stat.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7746031746031746%*

 * *Differences: {"'dep_lines'": '{delete: [2]}',*

 * * "'dep_prios'": '{delete: [1]}',*

 * * "'dependencies'": "{insert: [(4, 'typing')], delete: [4, 1]}",*

 * * "'hash'": "'4545d9f4011bbe91db363d9537e5d852b7ba1d7bb73b7bda9b540122a7cac958'",*

 * * "'id'": "'_stat'",*

 * * "'interface_hash'": "'a61aa73892cc82b90287425ecfc03dac292e910c9ec04af03c2cfc83c8a85db4'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_stat.pyi'",*

 * * "'size'": '2944'}*

```diff
@@ -1,38 +1,35 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
         2,
-        3,
         1,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
         5,
-        5,
         30,
         30
     ],
     "dependencies": [
         "sys",
-        "typing",
         "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c",
-    "id": "sre_constants",
+    "hash": "4545d9f4011bbe91db363d9537e5d852b7ba1d7bb73b7bda9b540122a7cac958",
+    "id": "_stat",
     "ignore_all": true,
-    "interface_hash": "9712b3c3ae06b67272c232e1379bf306d8606ccbd5bb6d332f741942b043edb8",
-    "mtime": 1685143295,
+    "interface_hash": "a61aa73892cc82b90287425ecfc03dac292e910c9ec04af03c2cfc83c8a85db4",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_constants.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_stat.pyi",
     "plugin_data": null,
-    "size": 3986,
+    "size": 2944,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/sre_parse.data.json` & `su6-0.3.0/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/sre_parse.meta.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_format.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.769090909090909%*

 * *Differences: {"'dep_lines'": '{insert: [(2, 3)], delete: [5, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 25)], delete: [7, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'mdurl._url'), (1, '__future__')], delete: [7, 5, 3, 2, 1, 0]}",*

 * * "'hash'": "'c5972dd2675e3d70341f7900ab18c6b650793bce86df90c060c1a4038e02981e'",*

 * * "'id'": "'mdurl._format'",*

 * * "'interface_hash'": "'dba7009860e9aa1a455609dc3b1b29ec8f98225b3e3cd3619daa07d9eefa2086'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdur […]*

```diff
@@ -1,46 +1,34 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        2,
-        1,
-        3,
-        4,
         6,
-        7,
         1,
+        3,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        10,
-        5,
-        5,
+        25,
         5,
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
-        "re",
-        "sre_constants",
+        "mdurl._url",
+        "__future__",
         "typing",
-        "typing_extensions",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "38b6a819e544b584ec71b7040293fae6a77f2447fc14e9bc70e752ec237c8022",
-    "id": "sre_parse",
+    "hash": "c5972dd2675e3d70341f7900ab18c6b650793bce86df90c060c1a4038e02981e",
+    "id": "mdurl._format",
     "ignore_all": true,
-    "interface_hash": "14e54a4df7b7598ae3ed25a7fa48a5aee75f5efef703f80ea55a22acfed7f287",
+    "interface_hash": "dba7009860e9aa1a455609dc3b1b29ec8f98225b3e3cd3619daa07d9eefa2086",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -75,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_parse.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_format.py",
     "plugin_data": null,
-    "size": 4069,
+    "size": 626,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/stat.data.json` & `su6-0.3.0/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/stat.meta.json` & `su6-0.3.0/.mypy_cache/3.11/stat.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -18,15 +18,15 @@
         "abc",
         "typing"
     ],
     "hash": "1fd817ee6e4326df5c4f9878c64dc9c080c05437734adfdc1dfa1e546fc1d8aa",
     "id": "stat",
     "ignore_all": true,
     "interface_hash": "c6ff0f50154f0f201b18bb46176fc1c264df495fb049dd8a5e30e5d038165b65",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/string.data.json` & `su6-0.3.0/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/string.meta.json` & `su6-0.3.0/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7503703703703705%*

 * *Differences: {"'dep_lines'": '{delete: [5, 4, 3, 0]}',*

 * * "'dep_prios'": '{delete: [4, 3, 2, 0]}',*

 * * "'dependencies'": "{insert: [(4, 'typing')], delete: [8, 4, 3, 2, 0]}",*

 * * "'hash'": "'d4a762dc87ddb7286da0abdb399dec04efb82a19579a4ef11af621851da7b598'",*

 * * "'id'": "'msvcrt'",*

 * * "'interface_hash'": "'9c3d3ffaec1b81ce2404515a91e464cc85aa699821a8db83958c5e1a7001082c'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/msvcrt.pyi'",*

 * * "'size'": '995'}*

```diff
@@ -1,47 +1,35 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        3,
         1,
         2,
-        4,
-        5,
-        6,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
         10,
         5,
         5,
-        5,
-        5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
         "sys",
-        "_typeshed",
-        "re",
-        "typing",
         "typing_extensions",
         "builtins",
         "abc",
-        "enum"
+        "typing"
     ],
-    "hash": "cc44bbe664dd2094229250b9499117bb258740f154f72d04a08d32edb54ad646",
-    "id": "string",
+    "hash": "d4a762dc87ddb7286da0abdb399dec04efb82a19579a4ef11af621851da7b598",
+    "id": "msvcrt",
     "ignore_all": true,
-    "interface_hash": "5bb98aba794ab5988f1bfd88b7f0e191c9464bf62d9d67e4378a3a6f7bcb5e84",
-    "mtime": 1685143295,
+    "interface_hash": "9c3d3ffaec1b81ce2404515a91e464cc85aa699821a8db83958c5e1a7001082c",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -75,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/string.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/msvcrt.pyi",
     "plugin_data": null,
-    "size": 3097,
+    "size": 995,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/subprocess.data.json` & `su6-0.3.0/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/subprocess.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7404382284382284%*

 * *Differences: {"'data_mtime'": '1685143684',*

 * * "'dep_lines'": '{insert: [(2, 3), (6, 7), (7, 423), (8, 424), (9, 1), (10, 1), (11, 1), (12, 1), '*

 * *                '(13, 1)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (3, 10), (4, 10), (5, 10), (7, 20), (8, 20), (10, '*

 * *                '30), (11, 30), (12, 30), (13, 30), (14, 30)], delete: [4, 3, 2, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'codecs'), (1, 'io'), (2, 'os'), (3, 're'), (6, 'weakref'), (7, "*

 * *                   "'errno'), (8, 'random'), (10, '_cod […]*

```diff
@@ -1,58 +1,82 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143684,
     "dep_lines": [
-        3,
         1,
         2,
+        3,
         4,
         5,
         6,
+        7,
+        423,
+        424,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
+        10,
+        10,
+        10,
+        10,
+        10,
         10,
         5,
+        20,
+        20,
         5,
-        5,
-        5,
-        5,
+        30,
+        30,
+        30,
+        30,
+        30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
+        "codecs",
+        "io",
+        "os",
+        "re",
         "sys",
-        "_typeshed",
-        "types",
         "typing",
-        "typing_extensions",
+        "weakref",
+        "errno",
+        "random",
         "builtins",
+        "_codecs",
+        "_typeshed",
         "abc",
         "array",
         "ctypes",
+        "genericpath",
         "mmap",
-        "os",
-        "pickle"
+        "pickle",
+        "posixpath",
+        "types",
+        "typing_extensions"
     ],
-    "hash": "d4ba0d25f732153c8003c650e12155f803326ed0fac4281b27d871f56a50cd34",
-    "id": "subprocess",
+    "hash": "2481cb62cec9cf3e0a4fdb7e76ce28e230732e39f00a22502aababfb98b008a2",
+    "id": "click._compat",
     "ignore_all": true,
-    "interface_hash": "5ae7ed6dca59aec33fec130abf5d53e13e5ac14c1cf73804d5046aaf8303bc28",
+    "interface_hash": "b6edd78bba746e6aa879f29be935595252217a360090570b3684c4e003b34434",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -87,13 +111,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/subprocess.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/click/_compat.py",
     "plugin_data": null,
-    "size": 91091,
+    "size": 18810,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/sys.data.json` & `su6-0.3.0/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/sys.meta.json` & `su6-0.3.0/.mypy_cache/3.11/sys.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -39,15 +39,15 @@
         "abc",
         "importlib"
     ],
     "hash": "bb33fcc38a16497298549aa7d67ceac363fdf6c670ea0baeed5f44f5a24e2b3b",
     "id": "sys",
     "ignore_all": true,
     "interface_hash": "c61b3585dc8c27d1eb5d96398fca5e03f21bbe305c599fc0c8fabb9d8d504ee6",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/tempfile.data.json` & `su6-0.3.0/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/tempfile.meta.json` & `su6-0.3.0/.mypy_cache/3.11/pathlib.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7633333333333333%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 12), (3, 13), (4, 14), (5, 15), (6, 16), (7, 17)], delete: [7, 6, '*

 * *                '5, 4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(7, 5), (8, 5)], delete: [8, 1]}',*

 * * "'dependencies'": "{insert: [(3, 'io'), (4, 'os')], delete: [12, 1]}",*

 * * "'hash'": "'af5d9944e5c7afe3dd4c99f5d83d4950e1d88bbcaba5db66ac57f946b5d10f41'",*

 * * "'id'": "'pathlib'",*

 * * "'interface_hash'": "'bd4e7f6edf566926f7480e2946c15d13f167e2f912a9a794c2f7c1067a8fad80'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/we […]*

```diff
@@ -1,62 +1,62 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        4,
+        12,
         1,
         2,
-        3,
-        5,
-        6,
-        7,
-        1,
+        13,
+        14,
+        15,
+        16,
+        17,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
-        10,
         5,
         5,
         5,
         5,
         5,
-        30,
+        5,
+        5,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "io",
         "sys",
         "_typeshed",
+        "io",
+        "os",
         "types",
         "typing",
         "typing_extensions",
         "builtins",
         "abc",
         "array",
         "ctypes",
         "mmap",
-        "os",
         "pickle"
     ],
-    "hash": "7907cc70476aaeb3c54da28bb94a0ee3b8183cedae5975862c489f6c4a25678b",
-    "id": "tempfile",
+    "hash": "af5d9944e5c7afe3dd4c99f5d83d4950e1d88bbcaba5db66ac57f946b5d10f41",
+    "id": "pathlib",
     "ignore_all": true,
-    "interface_hash": "fa62afc141aeeac2ddbe8b72a3826ec37f24ae28caa6e475b5b8e3dad4284a22",
-    "mtime": 1685143295,
+    "interface_hash": "bd4e7f6edf566926f7480e2946c15d13f167e2f912a9a794c2f7c1067a8fad80",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -90,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/tempfile.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/pathlib.pyi",
     "plugin_data": null,
-    "size": 17269,
+    "size": 7949,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/termios.data.json` & `su6-0.3.0/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/termios.meta.json` & `su6-0.3.0/.mypy_cache/3.11/platform.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7505952380952381%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 7), (2, 1)], delete: [3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(3, 30)], delete: [2, 1]}',*

 * * "'dependencies'": "{insert: [(3, '_typeshed')], delete: [3, 1]}",*

 * * "'hash'": "'20e99509f6e765e56fea8ebf9375e15695f123fdc0af99ca50e323efd17ebc44'",*

 * * "'id'": "'platform'",*

 * * "'interface_hash'": "'530d2c958c1822755594b66ea896cb0b8e7b2133dd9ea8d023129d8b044b0af7'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/p […]*

```diff
@@ -1,38 +1,35 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        2,
-        3,
-        4,
+        7,
+        1,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
         5,
-        5,
-        5,
+        30,
         30
     ],
     "dependencies": [
         "sys",
-        "_typeshed",
         "typing",
-        "typing_extensions",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "2f0f08844c903b2aa786d04a8a488242c21b5912f570b5db810e5afc7ec29ba9",
-    "id": "termios",
+    "hash": "20e99509f6e765e56fea8ebf9375e15695f123fdc0af99ca50e323efd17ebc44",
+    "id": "platform",
     "ignore_all": true,
-    "interface_hash": "6949464470ae855c517f57f5cd7944fe547de71b372e20a351af08f190f9884f",
-    "mtime": 1685143295,
+    "interface_hash": "530d2c958c1822755594b66ea896cb0b8e7b2133dd9ea8d023129d8b044b0af7",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/termios.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/platform.pyi",
     "plugin_data": null,
-    "size": 5095,
+    "size": 2375,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/textwrap.data.json` & `su6-0.3.0/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/textwrap.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_null_file.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.775%*

 * *Differences: {"'dependencies'": "{insert: [(0, 'types'), (1, 'typing'), (3, '_typeshed')], delete: [4, 1, 0]}",*

 * * "'hash'": "'b4649793fbfe21999b8f5180cc78adf00de460840c882a55b0215fb02fbf289e'",*

 * * "'id'": "'rich._null_file'",*

 * * "'interface_hash'": "'879597e4b2f8671f49bd21f5497de7289f9fb377c45b9bd8140b4301219ab3ab'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_null_file.py'",*

 * * "'size'": '1387'}*

```diff
@@ -11,25 +11,25 @@
         5,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "re",
+        "types",
+        "typing",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "e9e1065949260d153ff9f03e68e2165ac7bdfb5188abc4fcf52e1569ff5a27b6",
-    "id": "textwrap",
+    "hash": "b4649793fbfe21999b8f5180cc78adf00de460840c882a55b0215fb02fbf289e",
+    "id": "rich._null_file",
     "ignore_all": true,
-    "interface_hash": "29232ba58f8215dd6357b76e6f62c44a51e72d89c8e61f20e5095cce0c3941c6",
-    "mtime": 1685143295,
+    "interface_hash": "879597e4b2f8671f49bd21f5497de7289f9fb377c45b9bd8140b4301219ab3ab",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/textwrap.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_null_file.py",
     "plugin_data": null,
-    "size": 3233,
+    "size": 1387,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/threading.data.json` & `su6-0.3.0/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/threading.meta.json` & `su6-0.3.0/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7610774410774411%*

 * *Differences: {"'dep_lines'": '{insert: [(2, 3)], delete: [6, 5, 0]}',*

 * * "'dep_prios'": '{delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'email.message'), (2, 'email.policy')], delete: [6, 3, 2, 1]}",*

 * * "'hash'": "'6bef9c70cfca2efd38e18849f547603c1578043aabfa6e9ac44b019e9e2c323b'",*

 * * "'id'": "'email'",*

 * * "'interface_hash'": "'2e646e239ef025bcfe7280473c83a79ac7db26c13d93528e2a15010efdbfac7d'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/ […]*

```diff
@@ -1,47 +1,41 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        3,
         1,
         2,
+        3,
         4,
         5,
-        6,
-        51,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
         5,
         5,
         5,
         5,
         5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "sys",
-        "_typeshed",
-        "types",
+        "email.message",
+        "email.policy",
         "typing",
         "typing_extensions",
-        "_thread",
         "builtins",
         "abc"
     ],
-    "hash": "f2c4bdcb0b9cbdadb0c49fa600420d90019d83e6854d3a5a5aafd988fe3cd378",
-    "id": "threading",
+    "hash": "6bef9c70cfca2efd38e18849f547603c1578043aabfa6e9ac44b019e9e2c323b",
+    "id": "email",
     "ignore_all": true,
-    "interface_hash": "aa82688d3c03b586c022cf1142ca5632a48efc591fa0b627211e885f1fd85f23",
-    "mtime": 1685143295,
+    "interface_hash": "2e646e239ef025bcfe7280473c83a79ac7db26c13d93528e2a15010efdbfac7d",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -75,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/threading.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/__init__.pyi",
     "plugin_data": null,
-    "size": 6028,
+    "size": 1054,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/time.data.json` & `su6-0.3.0/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/time.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6880952380952381%*

 * *Differences: {"'data_mtime'": '1685143879',*

 * * "'dep_lines'": '{insert: [(1, 1), (2, 1), (3, 1), (4, 1), (5, 1), (6, 1), (7, 1), (8, 1)], '*

 * *                'delete: [3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(2, 30), (3, 30), (4, 30), (5, 30), (6, 30), (7, 30), (8, 30), (9, '*

 * *                '30)], delete: [2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'itertools'), (1, 'builtins'), (3, 'abc'), (4, 'array'), (5, "*

 * *                   "'ctypes'), (6, 'mmap'), (7, 'pickle'), (8, 'types')], delete: [5, 4, 0]}",*

 * * "'hash'": "'72fa […]*

```diff
@@ -1,38 +1,53 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143879,
     "dep_lines": [
         1,
-        2,
-        3,
-        4,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
-        5,
         5,
         5,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "sys",
+        "itertools",
+        "builtins",
         "_typeshed",
+        "abc",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle",
+        "types",
         "typing",
-        "typing_extensions",
-        "builtins",
-        "abc"
+        "typing_extensions"
     ],
-    "hash": "81ee1e52c98cc1cd26d7a6aa6d5a9c23d100b4e14cdd725b405a720187e41f8c",
-    "id": "time",
+    "hash": "72faffdaff0145bc5c225e71e6575fa9d1e3848f188bcb3cca4e741bf9e6ea34",
+    "id": "importlib_metadata._itertools",
     "ignore_all": true,
-    "interface_hash": "7816257c61ae61d9828ffbe5f5b912a849465f4aabae1d902ea98aeb326bea5b",
-    "mtime": 1685143295,
+    "interface_hash": "0114264fde6d441302d2262cdcbb0b41b39f317fed176a8394f9ec4163612f2b",
+    "mtime": 1685143799,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +81,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/time.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/importlib_metadata/_itertools.py",
     "plugin_data": null,
-    "size": 3663,
+    "size": 2068,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/traceback.data.json` & `su6-0.3.0/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/traceback.meta.json` & `su6-0.3.0/.mypy_cache/3.11/traceback.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -30,15 +30,15 @@
         "builtins",
         "abc"
     ],
     "hash": "2497208e6ba2109935f781184e0161660605078966bace07775dd17c03e462aa",
     "id": "traceback",
     "ignore_all": true,
     "interface_hash": "f4d3d8a7f1efd5d131aa94ee8a536f454d35f48d95f0ae21b6981bfbc2c1cd20",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/tty.data.json` & `su6-0.3.0/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/tty.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7288888888888889%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 23), (1, 24), (3, 1), (4, 1)], delete: [2, 1]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (3, 30), (4, 30), (5, 30)], delete: [2, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'codecs'), (1, 're'), (3, '_codecs'), (5, 'typing'), (6, "*

 * *                   "'typing_extensions')], delete: [2, 1, 0]}",*

 * * "'hash'": "'04ea0e61e6345da5e1b63e6614e7c6539aec3956e4a744ae896763dd95a2f758'",*

 * * "'id'": "'markdown_it._punycode'",*

 * * "'interface_hash'": "'c00c6f578fc55ea1557781a8ed60305791b12208a2c8b08fb8cb4 […]*

```diff
@@ -1,35 +1,41 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        23,
+        24,
+        1,
+        1,
         1,
-        2,
-        3,
         1,
         1
     ],
     "dep_prios": [
         10,
+        10,
         5,
-        5,
-        5,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "sys",
-        "typing",
-        "typing_extensions",
+        "codecs",
+        "re",
         "builtins",
-        "abc"
+        "_codecs",
+        "abc",
+        "typing",
+        "typing_extensions"
     ],
-    "hash": "93eadd2f4010b8e595f7f4af4efc698bd6d7a8fe571bfad7e90078f8fdaf26f8",
-    "id": "tty",
+    "hash": "04ea0e61e6345da5e1b63e6614e7c6539aec3956e4a744ae896763dd95a2f758",
+    "id": "markdown_it._punycode",
     "ignore_all": true,
-    "interface_hash": "a9d1399e812eae7c01ab1ab2863f3d2eac3ae027bcc24c004a75d36506742307",
-    "mtime": 1685143295,
+    "interface_hash": "c00c6f578fc55ea1557781a8ed60305791b12208a2c8b08fb8cb4547d1d11c78",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/tty.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/_punycode.py",
     "plugin_data": null,
-    "size": 430,
+    "size": 2317,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/types.data.json` & `su6-0.3.0/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/types.meta.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_decode.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7591331269349845%*

 * *Differences: {"'dep_lines'": '{insert: [(2, 4), (3, 5), (4, 1), (5, 1), (6, 1), (7, 1), (8, 1), (9, 1), (10, '*

 * *                '1), (11, 1)], delete: [6, 5, 4, 3, 1]}',*

 * * "'dep_prios'": '{insert: [(3, 10), (5, 30), (6, 30), (7, 30), (8, 30), (9, 30), (10, 30), (11, '*

 * *                '30)], delete: [5, 4, 3]}',*

 * * "'dependencies'": "{insert: [(1, '__future__'), (2, 'functools'), (3, 're'), (4, 'builtins'), (6, "*

 * *                   "'abc'), (7, 'array'), (8, 'ctypes'), (9, 'enum'), (10, 'mmap'), (11, "*

 * *                   "'p […]*

```diff
@@ -1,46 +1,61 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         3,
-        16,
         1,
-        2,
-        19,
-        20,
-        607,
+        4,
+        5,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         10,
+        10,
         5,
-        5,
-        5,
-        5,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "importlib.machinery",
-        "sys",
-        "_typeshed",
-        "typing",
-        "typing_extensions",
+        "__future__",
+        "functools",
+        "re",
         "builtins",
+        "_typeshed",
         "abc",
-        "importlib"
+        "array",
+        "ctypes",
+        "enum",
+        "mmap",
+        "pickle",
+        "typing",
+        "typing_extensions"
     ],
-    "hash": "bb1594589ec5ca09736286838e17153b5f7c33e7eaa783ab884856ab9bbd8f04",
-    "id": "types",
+    "hash": "dd0fe00d0a94fff4ef0dbbbbc7e6fd2e36d5978416cb983fa85c258dcbaf37f6",
+    "id": "mdurl._decode",
     "ignore_all": true,
-    "interface_hash": "fea64d1cb455db2f23e925fb7c8aed26dd9823e8395482957e120518d869eabb",
+    "interface_hash": "6f5f83a6622ef21ad6e3b0383c8cc478e08bbed44b5e5ee6513bf696f36b56d8",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -75,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/types.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_decode.py",
     "plugin_data": null,
-    "size": 20809,
+    "size": 3004,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typing.data.json` & `su6-0.3.0/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typing.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typing.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -48,15 +48,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "78c5d7fda12b38e4f9c30cdbdfbb1dec5e28302fca1d3e1b86d0f48b9cecbb0f",
     "id": "typing",
     "ignore_all": true,
     "interface_hash": "25c24cf7f8fe29920a845b1c025dbbe469fe1cf916feec7cfd63af7530f538f3",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typing_extensions.data.json` & `su6-0.3.0/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -33,15 +33,15 @@
         "types",
         "builtins"
     ],
     "hash": "44b4201aff73a621deda9aa2be5ee1f0260fb30c6bda0dbefc887a3c65a04119",
     "id": "typing_extensions",
     "ignore_all": true,
     "interface_hash": "97a64b9296f7cd7e33606259f5b17e600995b040b31b5c94570b5369924712e9",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/uuid.data.json` & `su6-0.3.0/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/uuid.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.753250773993808%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 14), (1, 15), (6, 13), (7, 16), (8, 17), (9, 18)], delete: [4]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 10), (3, 10), (9, 5), (10, 5)], delete: [5]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'importlib.machinery'), (2, '_ast'), (4, "*

 * *                   "'types'), (6, 'abc'), (7, 'io'), (8, 'typing'), (14, 'os')], delete: [10, 5, "*

 * *                   '2]}',*

 * * "'hash'": "'2ef3e7cd4f57d7730ef462502b680809572a49eb21b9555784a5744ab4e70c3f'",*

 * * "'id'": "'imp […]*

```diff
@@ -1,53 +1,68 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        14,
+        15,
         1,
         2,
         3,
         4,
-        1,
+        13,
+        16,
+        17,
+        18,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
+        5,
+        10,
+        10,
         10,
         5,
         5,
         5,
         5,
-        30,
+        5,
+        5,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
+        "collections.abc",
+        "importlib.machinery",
+        "_ast",
         "sys",
+        "types",
         "_typeshed",
-        "enum",
+        "abc",
+        "io",
+        "typing",
         "typing_extensions",
         "builtins",
-        "abc",
         "array",
         "ctypes",
         "mmap",
-        "pickle",
-        "typing"
+        "os",
+        "pickle"
     ],
-    "hash": "8c28006bde3a41ef255422bf6626035a62a8e9edaf430622e7f05e329a3c422e",
-    "id": "uuid",
+    "hash": "2ef3e7cd4f57d7730ef462502b680809572a49eb21b9555784a5744ab4e70c3f",
+    "id": "importlib.abc",
     "ignore_all": true,
-    "interface_hash": "68be08b7157d0b400fe2a32ba2ffd7e27aaf1bf6bcd798739b799c9e5dc737c6",
-    "mtime": 1685143295,
+    "interface_hash": "1f812316c4a5826c77daf23351cd0e6b42734c58b14468c8acb270ede33d5d9c",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -81,13 +96,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/uuid.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi",
     "plugin_data": null,
-    "size": 2558,
+    "size": 7380,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/warnings.data.json` & `su6-0.3.0/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/warnings.meta.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_encode.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7778787878787878%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 5), (4, 1), (5, 1)], delete: [5, 4, 2]}',*

 * * "'dep_prios'": '{insert: [(5, 30), (6, 30)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'urllib.parse'), (2, '__future__'), (3, 'string'), (6, "*

 * *                   "'typing'), (7, 'typing_extensions'), (8, 'urllib')], delete: [7, 5, 4, 3, 2, "*

 * *                   '1]}',*

 * * "'hash'": "'82824b505b75878ad564daaa9bdb75e4dc365be6c55d8404cb7691d352265afb'",*

 * * "'id'": "'mdurl._encode'",*

 * * "'interface_hash'": "'c46a8178501394440815b21cce0 […]*

```diff
@@ -1,46 +1,46 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         3,
+        5,
         1,
-        2,
         4,
-        5,
-        6,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
         5,
         5,
         5,
         5,
         30,
+        30,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "sys",
-        "_warnings",
-        "types",
+        "urllib.parse",
+        "__future__",
+        "string",
+        "builtins",
+        "abc",
         "typing",
         "typing_extensions",
-        "builtins",
-        "_typeshed",
-        "abc"
+        "urllib"
     ],
-    "hash": "9a991da6c7cb550f45efd87385ec22f61a45c69511ab3af2594b6d1ce0487343",
-    "id": "warnings",
+    "hash": "82824b505b75878ad564daaa9bdb75e4dc365be6c55d8404cb7691d352265afb",
+    "id": "mdurl._encode",
     "ignore_all": true,
-    "interface_hash": "a2c670fd5bdd0dedfd8034ac63ff7a45aefb3014858e5188b2f96cec862ca4ac",
+    "interface_hash": "c46a8178501394440815b21cce0bea6c32abcb1c9cad344caff69c21789a1940",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -75,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/warnings.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_encode.py",
     "plugin_data": null,
-    "size": 3682,
+    "size": 2602,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/weakref.data.json` & `su6-0.3.0/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/weakref.meta.json` & `su6-0.3.0/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7444444444444446%*

 * *Differences: {"'dep_lines'": '{delete: [6, 5, 4, 3, 0]}',*

 * * "'dep_prios'": '{delete: [4, 3, 2, 1, 0]}',*

 * * "'dependencies'": '{delete: [6, 4, 3, 2, 1]}',*

 * * "'hash'": "'5dd5349e16128655996d25e9c4676c82eaed3374bf9740bd98360257d4df6a29'",*

 * * "'id'": "'json.decoder'",*

 * * "'interface_hash'": "'fc463b2e147ff6395c1c12cef7cd5d5aa5d3e10f5c41b66aa1dddc135ae77e51'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/decoder.pyi'",*

 * * "'size'": '1117'}*

```diff
@@ -1,47 +1,32 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        13,
         1,
         2,
-        3,
-        12,
-        14,
-        15,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
-        5,
-        5,
         5,
         5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "sys",
-        "_typeshed",
-        "_weakref",
-        "_weakrefset",
         "typing",
-        "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "2f4d35940e2c4b0c2eb1bf2a5ba693d7594eb77431269f2de4e9683bb3f3d9e2",
-    "id": "weakref",
+    "hash": "5dd5349e16128655996d25e9c4676c82eaed3374bf9740bd98360257d4df6a29",
+    "id": "json.decoder",
     "ignore_all": true,
-    "interface_hash": "13b7e4e6a79b3335dcdeae4b8f3f06a016f46d17c1fa6f02850816d065481b1a",
-    "mtime": 1685143295,
+    "interface_hash": "fc463b2e147ff6395c1c12cef7cd5d5aa5d3e10f5c41b66aa1dddc135ae77e51",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -75,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/weakref.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/decoder.pyi",
     "plugin_data": null,
-    "size": 6020,
+    "size": 1117,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/webbrowser.data.json` & `su6-0.3.0/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/webbrowser.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.769047619047619%*

 * *Differences: {"'dep_lines'": '{delete: [3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 30)], delete: [3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'abc')], delete: [3, 2, 1, 0]}",*

 * * "'hash'": "'7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f'",*

 * * "'id'": "'typer.colors'",*

 * * "'interface_hash'": "'27b284b26e724e12cf37260c1baa2dfb8b4eacd2f12a30cc5a22b69d7b95ad25'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/colors.py'",*

 * * "'size'": '430'}*

```diff
@@ -1,37 +1,28 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        3,
         1,
-        2,
-        4,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
-        "abc",
-        "typing_extensions",
         "builtins",
+        "abc",
         "typing"
     ],
-    "hash": "5eafef06c53dd8b7d5ef6d7ece9ac1448f3f153c6061af7e9701fdf92f9e307c",
-    "id": "webbrowser",
+    "hash": "7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f",
+    "id": "typer.colors",
     "ignore_all": true,
-    "interface_hash": "713ac81ceecef86d02bf81125c771c8657aa61761f3ce7d997ad5d0eb8f736ca",
+    "interface_hash": "27b284b26e724e12cf37260c1baa2dfb8b4eacd2f12a30cc5a22b69d7b95ad25",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -66,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/webbrowser.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/colors.py",
     "plugin_data": null,
-    "size": 2527,
+    "size": 430,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/zlib.data.json` & `su6-0.3.0/.mypy_cache/3.11/zlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/zlib.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_ratio.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7222222222222222%*

 * *Differences: {"'data_mtime'": '1685143684',*

 * * "'dep_lines'": '{insert: [(3, 4), (4, 150)], delete: [3]}',*

 * * "'dep_prios'": '{insert: [(4, 5), (5, 5)], delete: [4]}',*

 * * "'dependencies'": "{insert: [(1, 'fractions'), (2, 'math'), (3, 'typing'), (4, 'dataclasses'), "*

 * *                   "(6, '_decimal'), (7, '_typeshed'), (9, 'numbers'), (10, 'typing_extensions')], "*

 * *                   'delete: [9, 8, 7, 6, 5, 2, 1]}',*

 * * "'hash'": "'e9d047c62c3f49835145d719f600ca2391a701e1d9f16be64e072d36972eb665'",*

 * * "'id'": "'rich._ratio'",*

 * * " […]*

```diff
@@ -1,50 +1,53 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143684,
     "dep_lines": [
         1,
         2,
         3,
-        1,
+        4,
+        150,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
         5,
         5,
-        30,
+        5,
+        5,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
         "sys",
-        "_typeshed",
-        "typing_extensions",
+        "fractions",
+        "math",
+        "typing",
+        "dataclasses",
         "builtins",
+        "_decimal",
+        "_typeshed",
         "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle",
-        "typing"
+        "numbers",
+        "typing_extensions"
     ],
-    "hash": "5cfaadb83c98fbafc7b16f74eb5a6a88e32ad3912d1b9d89a788983ed3e6a8e3",
-    "id": "zlib",
+    "hash": "e9d047c62c3f49835145d719f600ca2391a701e1d9f16be64e072d36972eb665",
+    "id": "rich._ratio",
     "ignore_all": true,
-    "interface_hash": "bdf2de9a898fcc3adbcefd8746e9d3e9006aa3491765c1ac71dd5e4efa0dc516",
-    "mtime": 1685143295,
+    "interface_hash": "382f661f12b18379bc061ff96638f37c925dc21430a12725701db59da6db2d38",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -78,13 +81,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/zlib.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_ratio.py",
     "plugin_data": null,
-    "size": 1787,
+    "size": 5460,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -45,15 +45,15 @@
         "builtins",
         "abc"
     ],
     "hash": "b51d2b79a156278383c840da565bf3312ef8e715015d3a44096c0c5eac13393d",
     "id": "_typeshed",
     "ignore_all": true,
     "interface_hash": "4ef2d160516e285b420e0961365fda7f825237b733569e3b275106a350c80337",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/_compat.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/_compat.meta.json` & `su6-0.3.0/.mypy_cache/3.11/tempfile.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7112354312354313%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 4)], delete: [13, 12, 11, 10, 9, 8, 7, 3]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (5, 5), (6, 5), (7, 5)], delete: [14, 13, 12, 11, 10, 8, 7, 3, '*

 * *                '2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (3, '_typeshed'), (4, 'types'), (6, "*

 * *                   "'typing_extensions'), (12, 'os')], delete: [20, 19, 18, 15, 11, 10, 8, 7, 6, "*

 * *                   '3, 2, 0]}',*

 * * "'hash'": "'7907cc70476aaeb3c54da28bb94a0ee3b8183ced […]*

```diff
@@ -1,83 +1,62 @@
 {
-    "data_mtime": 1685143684,
+    "data_mtime": 1685143683,
     "dep_lines": [
+        4,
         1,
         2,
         3,
-        4,
         5,
         6,
         7,
-        423,
-        424,
-        1,
-        1,
-        1,
-        1,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        10,
-        10,
-        10,
+        5,
         10,
         10,
         5,
-        20,
-        20,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
+        5,
+        5,
+        5,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "codecs",
+        "collections.abc",
         "io",
-        "os",
-        "re",
         "sys",
+        "_typeshed",
+        "types",
         "typing",
-        "weakref",
-        "errno",
-        "random",
+        "typing_extensions",
         "builtins",
-        "_codecs",
-        "_typeshed",
         "abc",
         "array",
         "ctypes",
-        "genericpath",
         "mmap",
-        "pickle",
-        "posixpath",
-        "types",
-        "typing_extensions"
+        "os",
+        "pickle"
     ],
-    "hash": "2481cb62cec9cf3e0a4fdb7e76ce28e230732e39f00a22502aababfb98b008a2",
-    "id": "click._compat",
+    "hash": "7907cc70476aaeb3c54da28bb94a0ee3b8183cedae5975862c489f6c4a25678b",
+    "id": "tempfile",
     "ignore_all": true,
-    "interface_hash": "b6edd78bba746e6aa879f29be935595252217a360090570b3684c4e003b34434",
-    "mtime": 1685143295,
+    "interface_hash": "fa62afc141aeeac2ddbe8b72a3826ec37f24ae28caa6e475b5b8e3dad4284a22",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -111,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/click/_compat.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/tempfile.pyi",
     "plugin_data": null,
-    "size": 18810,
+    "size": 17269,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/_termui_impl.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/_termui_impl.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/_textwrap.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/_textwrap.meta.json` & `su6-0.3.0/.mypy_cache/3.11/getpass.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7428571428571428%*

 * *Differences: {"'dep_lines'": '{delete: [3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [5, 4, 1, 0]}',*

 * * "'dependencies'": '{delete: [6, 4, 2, 0]}',*

 * * "'hash'": "'1c755308b5f630e123566d4785ff25d521e2d12de4014056713d1d1f2dbbc19f'",*

 * * "'id'": "'getpass'",*

 * * "'interface_hash'": "'846d32fa7d3f0ba4c3a00aaa237cf1e4a0e4916fe3c05ebbf1459c9ddef5c98a'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/getpass.pyi'",*

 * * "'size'": '227'}*

```diff
@@ -1,41 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        2,
-        3,
-        1,
-        1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        10,
         5,
         5,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "textwrap",
         "typing",
-        "contextlib",
         "builtins",
-        "_typeshed",
-        "abc",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "d747d0eb839c05432e2bb985be1f37eb7feea0ec4f95122d64198acd12438286",
-    "id": "click._textwrap",
+    "hash": "1c755308b5f630e123566d4785ff25d521e2d12de4014056713d1d1f2dbbc19f",
+    "id": "getpass",
     "ignore_all": true,
-    "interface_hash": "90f3db3ff0c60035a0c3f5c1fbeac280a4736bc3d493e18fe767f2cb7a77f86e",
-    "mtime": 1685143295,
+    "interface_hash": "846d32fa7d3f0ba4c3a00aaa237cf1e4a0e4916fe3c05ebbf1459c9ddef5c98a",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/click/_textwrap.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/getpass.pyi",
     "plugin_data": null,
-    "size": 1353,
+    "size": 227,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/core.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/core.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/decorators.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/decorators.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/exceptions.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/exceptions.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/formatting.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/formatting.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/globals.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/globals.meta.json` & `su6-0.3.0/.mypy_cache/3.11/abc.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7055555555555555%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 4), (4, 6)], delete: [4, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (5, 5)], delete: [5, 3, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, '_typeshed'), (2, 'sys')], delete: [5, "*

 * *                   '2, 0]}',*

 * * "'hash'": "'ceadae3f72efc214373499b073a01a7026c2fbec852c488327ec4bad5cb23b67'",*

 * * "'id'": "'abc'",*

 * * "'interface_hash'": "'0eec2da7f77546f50f6e9328b32cd2abdc0038afe86d0a726dfd6d2bcfcee607'",*

 * * "'mtime'": '1685283590',*

 * * " […]*

```diff
@@ -1,38 +1,38 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        6,
+        4,
         1,
         2,
         5,
-        1,
+        6,
         1
     ],
     "dep_prios": [
-        25,
+        5,
+        5,
         10,
         5,
-        25,
         5,
-        30
+        5
     ],
     "dependencies": [
-        "click.core",
+        "collections.abc",
+        "_typeshed",
+        "sys",
         "typing",
-        "threading",
         "typing_extensions",
-        "builtins",
-        "abc"
+        "builtins"
     ],
-    "hash": "4cffaa33cf124f373b7f5dbb877e530ffbfddb41607ce0f6130cea034a04f175",
-    "id": "click.globals",
+    "hash": "ceadae3f72efc214373499b073a01a7026c2fbec852c488327ec4bad5cb23b67",
+    "id": "abc",
     "ignore_all": true,
-    "interface_hash": "ea4004205ca0c1c53556d83cbdae280ff0dd68081faaeeb251669dbd6fa04017",
-    "mtime": 1685143295,
+    "interface_hash": "0eec2da7f77546f50f6e9328b32cd2abdc0038afe86d0a726dfd6d2bcfcee607",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/click/globals.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/abc.pyi",
     "plugin_data": null,
-    "size": 1961,
+    "size": 1773,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/parser.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/parser.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7780759087260635%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 1), (1, 1)], delete: [7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [7, 6, 5, 4, 3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'click'), (8, 'typing'), (9, 'typing_extensions')], delete: [15, "*

 * *                   '7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'hash'": "'929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a'",*

 * * "'id'": "'typer._compat_utils'",*

 * * "'interface_hash'": "'f13939f83ff3c74c0b399e38a0f09049771195ed55e4e7d096d0f5225ca3996b'",*

 * * "'path' […]*

```diff
@@ -1,67 +1,49 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        29,
-        36,
-        24,
-        25,
-        26,
-        35,
-        140,
-        395,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        25,
         10,
         5,
-        5,
-        25,
-        20,
-        20,
-        5,
+        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "click.exceptions",
-        "click.core",
-        "typing",
-        "collections",
-        "gettext",
-        "typing_extensions",
-        "shlex",
-        "difflib",
+        "click",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle",
-        "types"
+        "typing",
+        "typing_extensions"
     ],
-    "hash": "70012dd6e411f20ab7f92f72b2a6d553e7dd01936f8a5c70e11789fd3d4e40c9",
-    "id": "click.parser",
+    "hash": "929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a",
+    "id": "typer._compat_utils",
     "ignore_all": true,
-    "interface_hash": "7d71318c773f103c9de02366cb3b6ad6aa171a08f00d26c380488086111d7e4a",
+    "interface_hash": "f13939f83ff3c74c0b399e38a0f09049771195ed55e4e7d096d0f5225ca3996b",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -96,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/click/parser.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_compat_utils.py",
     "plugin_data": null,
-    "size": 19044,
+    "size": 94,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/shell_completion.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/shell_completion.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/termui.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/termui.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/types.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/types.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/utils.data.json` & `su6-0.3.0/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/click/utils.meta.json` & `su6-0.3.0/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/collections/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -33,15 +33,15 @@
         "builtins",
         "abc"
     ],
     "hash": "f5e16c9ed8790956c54a074ea675d0ce3404db9e0e83a2d254e706d06290b724",
     "id": "collections",
     "ignore_all": true,
     "interface_hash": "02da07e0f9a70efabb774f32b47c3554ef92648b90c2082498e85987d25fdeb8",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/collections/abc.data.json` & `su6-0.3.0/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/collections/abc.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/themes.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7253968253968254%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 1), (1, 2)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (3, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.default_styles'), (1, 'rich.theme'), (4, 'rich.style')], "*

 * *                   'delete: [0]}',*

 * * "'hash'": "'d318132e8cdf69b79b62d709b43742e50917e4855411abe2a83509261e185459'",*

 * * "'id'": "'rich.themes'",*

 * * "'interface_hash'": "'c7645ea79e02f663c3e35494c3e38d3edbfed0d874cd39434350c8e598165d3a'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/ […]*

```diff
@@ -1,32 +1,38 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
         1,
+        2,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        5,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "_collections_abc",
+        "rich.default_styles",
+        "rich.theme",
         "builtins",
         "abc",
+        "rich.style",
         "typing"
     ],
-    "hash": "90189900dd153dff2aa642276e3a8a65145ed0f5eb67b8f1366086b38a3950e7",
-    "id": "collections.abc",
+    "hash": "d318132e8cdf69b79b62d709b43742e50917e4855411abe2a83509261e185459",
+    "id": "rich.themes",
     "ignore_all": true,
-    "interface_hash": "06bab035dfaa5f3ad1efba42299a607e80d44d225139ec1f803fdb074d7a9d93",
-    "mtime": 1685143295,
+    "interface_hash": "c7645ea79e02f663c3e35494c3e38d3edbfed0d874cd39434350c8e598165d3a",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/collections/abc.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/themes.py",
     "plugin_data": null,
-    "size": 79,
+    "size": 102,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/pydoc.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.755%*

 * *Differences: {"'dep_lines'": '{insert: [(7, 8), (8, 9)], delete: [11, 10, 9, 8, 7]}',*

 * * "'dep_prios'": '{delete: [11, 10, 9]}',*

 * * "'dependencies'": "{insert: [(4, 'builtins'), (5, 'reprlib'), (6, 'types')], delete: [11, 10, 9, "*

 * *                   '8, 7, 2]}',*

 * * "'hash'": "'a5b9fc8f7d48fde0a812a953344848dea1b6208d66a6982cd1bd378be309e395'",*

 * * "'id'": "'pydoc'",*

 * * "'interface_hash'": "'4f9b07c1646cb983b9add257b6935f65c646ea35ed72fa25a6814a8113127759'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/ […]*

```diff
@@ -4,53 +4,44 @@
         5,
         1,
         2,
         3,
         4,
         6,
         7,
-        10,
-        1,
-        1,
-        1,
-        1
+        8,
+        9
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
         5,
         5,
         5,
-        5,
-        30,
-        30,
-        30
+        5
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "_ctypes",
         "_typeshed",
         "abc",
-        "typing",
-        "typing_extensions",
-        "types",
         "builtins",
-        "array",
-        "mmap",
-        "pickle"
+        "reprlib",
+        "types",
+        "typing",
+        "typing_extensions"
     ],
-    "hash": "4e07f95e28e46e9d4c5eda8e3a693994b25ddc9e70955e59f569acc5472d3284",
-    "id": "ctypes",
+    "hash": "a5b9fc8f7d48fde0a812a953344848dea1b6208d66a6982cd1bd378be309e395",
+    "id": "pydoc",
     "ignore_all": true,
-    "interface_hash": "258d6db8de019fc835a41737c0c96359c2e8e1c006da708ce31c5b3846725a76",
-    "mtime": 1685143295,
+    "interface_hash": "4f9b07c1646cb983b9add257b6935f65c646ea35ed72fa25a6814a8113127759",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -84,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/pydoc.pyi",
     "plugin_data": null,
-    "size": 11646,
+    "size": 10392,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/ctypes/wintypes.data.json` & `su6-0.3.0/.mypy_cache/3.11/ctypes/wintypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/ctypes/wintypes.meta.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_url.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7861904761904762%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 3)], delete: [1, 0]}',*

 * * "'dep_prios'": '{delete: [3]}',*

 * * "'dependencies'": "{insert: [(0, '__future__'), (1, 'typing')], delete: [4, 1, 0]}",*

 * * "'hash'": "'e6442745037603f1b8b2f2e747365c1b46dfa03f406c1ad80d7a2eb031d9df3d'",*

 * * "'id'": "'mdurl._url'",*

 * * "'interface_hash'": "'2a514ad3dcf650747db692ff0fa23e44a0203118f1fbd0b2df0c38e4c5100970'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_url.py'",*

 * * "'size'": '284'}*

```diff
@@ -1,34 +1,31 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        23,
-        1,
+        3,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
-        "ctypes",
-        "typing_extensions",
+        "__future__",
+        "typing",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "defeeb073c43c6345deb22a8d25df81981445c4754febdceecfffcf2ad494435",
-    "id": "ctypes.wintypes",
+    "hash": "e6442745037603f1b8b2f2e747365c1b46dfa03f406c1ad80d7a2eb031d9df3d",
+    "id": "mdurl._url",
     "ignore_all": true,
-    "interface_hash": "9096eb2cb1b060b28548100a7e883a3d72ab90d909c4cd3fdbc685aefeda3c80",
+    "interface_hash": "2a514ad3dcf650747db692ff0fa23e44a0203118f1fbd0b2df0c38e4c5100970",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -63,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/ctypes/wintypes.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_url.py",
     "plugin_data": null,
-    "size": 5284,
+    "size": 284,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7320454545454546%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 7), (1, 10), (2, 22), (3, 29), (4, 30), (5, 32), (6, 38), (8, 1)], '*

 * *                'delete: [3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (3, 10), (9, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'click.exceptions'), (1, 'click.termui'), (2, 'click.utils'), "*

 * *                   "(3, 'typer.colors'), (4, 'typer.main'), (5, 'typer.models'), (6, "*

 * *                   "'typer.params'), (7, 'shutil'), (10, 'typing')], delete: [4, 3, 2, 1, 0 […]*

```diff
@@ -1,40 +1,52 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        1,
-        2,
-        3,
-        4,
+        7,
+        10,
+        22,
+        29,
+        30,
+        32,
+        38,
         5,
         1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
+        10,
+        5,
+        5,
         5,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "email.message",
-        "email.policy",
-        "typing",
-        "typing_extensions",
+        "click.exceptions",
+        "click.termui",
+        "click.utils",
+        "typer.colors",
+        "typer.main",
+        "typer.models",
+        "typer.params",
+        "shutil",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "6bef9c70cfca2efd38e18849f547603c1578043aabfa6e9ac44b019e9e2c323b",
-    "id": "email",
+    "hash": "c5ff549135bc942c56bd006b25e9430d11aca40c240e6d2f7762a28e11ea3f28",
+    "id": "typer",
     "ignore_all": true,
-    "interface_hash": "2e646e239ef025bcfe7280473c83a79ac7db26c13d93528e2a15010efdbfac7d",
+    "interface_hash": "77eb44dfcf25f13187d20d29aaf6cb48eded4dc38ac76aa831bd663abd45a61b",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -69,13 +81,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/__init__.py",
     "plugin_data": null,
-    "size": 1054,
+    "size": 1602,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/charset.data.json` & `su6-0.3.0/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/charset.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_cell_widths.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.775%*

 * *Differences: {"'dep_lines'": '{delete: [0]}',*

 * * "'dep_prios'": '{delete: [0]}',*

 * * "'dependencies'": '{delete: [0]}',*

 * * "'hash'": "'da7e048898b75fdb2a22ad0ed7a91467fcf2e9460c777c457c286529f9d6d477'",*

 * * "'id'": "'rich._cell_widths'",*

 * * "'interface_hash'": "'51626b8163420906cde6caed792b590188b485e282bfdfe06cf073271dd588bd'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_cell_widths.py'",*

 * * "'size'": '10096'}*

```diff
@@ -1,32 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
         1,
-        1,
         1
     ],
     "dep_prios": [
         5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "7eb946e66f91d483704797cfcbe5603351fd555cb7655a0e5444e653fcd491d7",
-    "id": "email.charset",
+    "hash": "da7e048898b75fdb2a22ad0ed7a91467fcf2e9460c777c457c286529f9d6d477",
+    "id": "rich._cell_widths",
     "ignore_all": true,
-    "interface_hash": "2de97f403307003b2dcb8e652f6e41c2bb8efe58ff05e6839a0b41b5a4720686",
-    "mtime": 1685143295,
+    "interface_hash": "51626b8163420906cde6caed792b590188b485e282bfdfe06cf073271dd588bd",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/charset.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_cell_widths.py",
     "plugin_data": null,
-    "size": 1077,
+    "size": 10096,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-0.3.0/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-0.3.0/.mypy_cache/3.11/decimal.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7095238095238094%*

 * *Differences: {"'data_mtime'": '1685143684',*

 * * "'dep_lines'": '{insert: [(1, 1)], delete: [2, 1]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(0, '_decimal'), (3, 'typing')], delete: [2, 1, 0]}",*

 * * "'hash'": "'3af726e9b7292d9cb1396aeb99d9d991d615541e03459cf2265298543cb29e69'",*

 * * "'id'": "'decimal'",*

 * * "'interface_hash'": "'2247da24f493604d4e8f80d6685ea905f459273fef13c22011cdd98f6b12cc55'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/ […]*

```diff
@@ -1,35 +1,32 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143684,
     "dep_lines": [
         1,
-        2,
-        3,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "email.message",
-        "typing",
+        "_decimal",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf",
-    "id": "email.contentmanager",
+    "hash": "3af726e9b7292d9cb1396aeb99d9d991d615541e03459cf2265298543cb29e69",
+    "id": "decimal",
     "ignore_all": true,
-    "interface_hash": "86a7db72494c58ed2d0e5e9f95b2906da6e78e83aa31e5d85859dcbc0d594fad",
-    "mtime": 1685143295,
+    "interface_hash": "2247da24f493604d4e8f80d6685ea905f459273fef13c22011cdd98f6b12cc55",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/decimal.pyi",
     "plugin_data": null,
-    "size": 480,
+    "size": 117,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/errors.data.json` & `su6-0.3.0/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/errors.meta.json` & `su6-0.3.0/.mypy_cache/3.11/email/errors.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -21,15 +21,15 @@
         "abc",
         "typing"
     ],
     "hash": "ca7498bfe12fcf0148a719c9bfa9f40ff037ddb6e1308f6101d338a8b9a859b9",
     "id": "email.errors",
     "ignore_all": true,
     "interface_hash": "16c9ae8529ab35377883b11b2bc711f7d621d66d3f1352d74195a597037f24bb",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/header.data.json` & `su6-0.3.0/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/header.meta.json` & `su6-0.3.0/.mypy_cache/3.11/email/header.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -21,15 +21,15 @@
         "builtins",
         "abc"
     ],
     "hash": "d98ef62919eee52c902ba572fe572fc3a54622a5e630532cf09aa7f12374562d",
     "id": "email.header",
     "ignore_all": true,
     "interface_hash": "01187afc6a997ff0cfa6678d65f39b1f905eaae0cb55b51ac4ef0e366430347f",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/message.data.json` & `su6-0.3.0/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/message.meta.json` & `su6-0.3.0/.mypy_cache/3.11/email/message.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -36,15 +36,15 @@
         "builtins",
         "abc"
     ],
     "hash": "762e166d09e139961a402ba13a8aaabb0c5cbd010af7cd6f562150d86b3d6f4f",
     "id": "email.message",
     "ignore_all": true,
     "interface_hash": "e872437a0f57176c79a86b9d69089a4c48dbd1fc6907f65e4dda936c6d14b79f",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/policy.data.json` & `su6-0.3.0/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/email/policy.meta.json` & `su6-0.3.0/.mypy_cache/3.11/email/policy.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -30,15 +30,15 @@
         "typing",
         "builtins"
     ],
     "hash": "2122e2c085231b4505c48fb54f55b2fb36ead76660699bc3d800fffbd4f0c6f4",
     "id": "email.policy",
     "ignore_all": true,
     "interface_hash": "6dcefb20f7ebc6d81fba80753edb4f9695c0e5e1f9e4195cfb5fbc1b9e26f5ef",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/html/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/html/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -15,15 +15,15 @@
         "builtins",
         "abc"
     ],
     "hash": "4ca36dd8af43fa802f0939adf7f12d8119dd7296fefbcadac3160530f1d3482d",
     "id": "html",
     "ignore_all": true,
     "interface_hash": "f5a489fb30320ac11c544fa5068367117c3cb88c3c76e70fc9a0536f4261bcb3",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/html/entities.data.json` & `su6-0.3.0/.mypy_cache/3.11/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/html/entities.meta.json` & `su6-0.3.0/.mypy_cache/3.11/copy.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7666666666666667%*

 * *Differences: {"'dep_prios'": '{insert: [(1, 5)], delete: [1]}',*

 * * "'dependencies'": "{insert: [(0, 'typing')], delete: [2]}",*

 * * "'hash'": "'891dbbc4965fc233e2f13e2c8f79729c2bfce84a3f6f841f77ab43efd675ee7d'",*

 * * "'id'": "'copy'",*

 * * "'interface_hash'": "'475ff08feca909613d4745917797bea89365cd187492138f8a470792b5b8cb58'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/copy.pyi'",*

 * * "'size'": '350'}*

```diff
@@ -3,27 +3,27 @@
     "dep_lines": [
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        30,
+        5,
         30
     ],
     "dependencies": [
+        "typing",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "87ee8abb57e93a192d86d8d53172d3915c0a99cfb26706388593771a468b68c8",
-    "id": "html.entities",
+    "hash": "891dbbc4965fc233e2f13e2c8f79729c2bfce84a3f6f841f77ab43efd675ee7d",
+    "id": "copy",
     "ignore_all": true,
-    "interface_hash": "ffd23da68d18ff16bd92ee261d7c3c0a03e5bddad2981e2594a938c17a7f1b68",
-    "mtime": 1685143295,
+    "interface_hash": "475ff08feca909613d4745917797bea89365cd187492138f8a470792b5b8cb58",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/html/entities.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/copy.pyi",
     "plugin_data": null,
-    "size": 182,
+    "size": 350,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7431818181818183%*

 * *Differences: {"'data_mtime'": '1685143684',*

 * * "'dep_lines'": '{insert: [(0, 14), (1, 15), (2, 16), (3, 17), (4, 18)], delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'mdurl._decode'), (1, 'mdurl._encode'), (2, 'mdurl._format'), "*

 * *                   "(3, 'mdurl._parse'), (4, 'mdurl._url')], delete: [2, 1, 0]}",*

 * * "'hash'": "'d6fa44f3d3725e7888459342ff87fa04f9b751be1b3e7b637f2ca12d147ba295'",*

 * * "'id'": "'mdurl'",*

 * * "'interface_hash'": "'68709c75b089acb3978892b0b110795b20192 […]*

```diff
@@ -1,37 +1,43 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143684,
     "dep_lines": [
-        1,
-        2,
-        3,
+        14,
+        15,
+        16,
+        17,
+        18,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
+        5,
+        5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "importlib.abc",
-        "types",
+        "mdurl._decode",
+        "mdurl._encode",
+        "mdurl._format",
+        "mdurl._parse",
+        "mdurl._url",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914",
-    "id": "importlib",
+    "hash": "d6fa44f3d3725e7888459342ff87fa04f9b751be1b3e7b637f2ca12d147ba295",
+    "id": "mdurl",
     "ignore_all": true,
-    "interface_hash": "5f92435a83c8d015c7f5083f731f4b7db32ae1cd81d45c2986fdcbc6fcba52a3",
+    "interface_hash": "68709c75b089acb3978892b0b110795b2019253d8373e4bf42394bea8f0b2753",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -66,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/__init__.py",
     "plugin_data": null,
-    "size": 801,
+    "size": 547,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/abc.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/padding.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7054700854700855%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(1, 10), (2, 11), (3, 12), (5, 1), (6, 139), (7, 1), (8, 1), (9, 1)], '*

 * *                'delete: [9, 8, 7, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 25), (8, 30), (9, 30), (10, 30)], delete: [4, 3, 2, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.console'), (1, 'rich.jupyter'), (2, 'rich.measure'), (3, "*

 * *                   "'rich.style'), (4, 'rich.segment'), (6, 'rich'), (8, '_typeshed'), (9, 'abc'), "*

 * *                   "(12, 'enum'), (15, ' […]*

```diff
@@ -1,68 +1,68 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        14,
-        15,
-        1,
-        2,
-        3,
         4,
+        10,
+        11,
+        12,
         13,
-        16,
-        17,
-        18,
+        1,
+        139,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
+        25,
         5,
         5,
-        10,
-        10,
-        10,
-        5,
         5,
         5,
         5,
         5,
         5,
         30,
         30,
         30,
         30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "importlib.machinery",
-        "_ast",
-        "sys",
-        "types",
-        "_typeshed",
-        "abc",
-        "io",
+        "rich.console",
+        "rich.jupyter",
+        "rich.measure",
+        "rich.style",
+        "rich.segment",
         "typing",
-        "typing_extensions",
+        "rich",
         "builtins",
+        "_typeshed",
+        "abc",
         "array",
         "ctypes",
+        "enum",
         "mmap",
-        "os",
-        "pickle"
+        "pickle",
+        "typing_extensions"
     ],
-    "hash": "2ef3e7cd4f57d7730ef462502b680809572a49eb21b9555784a5744ab4e70c3f",
-    "id": "importlib.abc",
+    "hash": "f08d5d40d4102b58828c7b46043127efc911a77a76ec6633979511dea07b7b61",
+    "id": "rich.padding",
     "ignore_all": true,
-    "interface_hash": "1f812316c4a5826c77daf23351cd0e6b42734c58b14468c8acb270ede33d5d9c",
-    "mtime": 1685143295,
+    "interface_hash": "bc537bd6ac0e6faddeca536a672e1b6bf709b52f24ab1303bcb5841a890d3cca",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -96,13 +96,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/padding.py",
     "plugin_data": null,
-    "size": 7380,
+    "size": 4958,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -48,15 +48,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "d8d65c367ab0b794c41c101e2200e4171d0d147dfa49385be91cdd958db6fc1d",
     "id": "importlib.machinery",
     "ignore_all": true,
     "interface_hash": "ed787cd1b044afa8da6ba8ca65b83b98da626a56aeff0e387d41c80562131742",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -45,15 +45,15 @@
         "typing_extensions",
         "builtins"
     ],
     "hash": "ae422af81eff03dc03edf2ef5f854e32c69b6b23ebb6d7415e1165121041a540",
     "id": "importlib.metadata",
     "ignore_all": true,
     "interface_hash": "21a4b9857190f7893fd1d564e25c567d7f4777614d1a6990ac158bb2835a9eab",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -18,15 +18,15 @@
         "builtins",
         "abc"
     ],
     "hash": "2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4",
     "id": "importlib.metadata._meta",
     "ignore_all": true,
     "interface_hash": "c88463ed7df95bf0015736581082e5a7cd111fdf7879efce7252e1872cba96cd",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 3)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10)], delete: [3, 2]}',*

 * * "'dependencies'": "{insert: [(0, 'importlib_metadata._functools'), (1, 're'), (6, 'enum')], "*

 * *                   'delete: [10, 8, 2, 0]}',*

 * * "'hash'": "'1c2b0592c66924b7933f734493f9e0ac079755146d4ebb7287d78e001a113f80'",*

 * * "'id'": "'importlib_metadata._text'",*

 * * "'interface_hash'": "'80a1151f6ae59be2ef7bd25798341a5440572e4d5358ebb1270a6edba965ab68'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv […]*

```diff
@@ -1,52 +1,49 @@
 {
     "data_mtime": 1685143879,
     "dep_lines": [
-        1,
-        1,
+        3,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "itertools",
+        "importlib_metadata._functools",
+        "re",
         "builtins",
-        "_typeshed",
         "abc",
         "array",
         "ctypes",
+        "enum",
         "mmap",
         "pickle",
-        "types",
-        "typing",
-        "typing_extensions"
+        "typing"
     ],
-    "hash": "72faffdaff0145bc5c225e71e6575fa9d1e3848f188bcb3cca4e741bf9e6ea34",
-    "id": "importlib_metadata._itertools",
+    "hash": "1c2b0592c66924b7933f734493f9e0ac079755146d4ebb7287d78e001a113f80",
+    "id": "importlib_metadata._text",
     "ignore_all": true,
-    "interface_hash": "0114264fde6d441302d2262cdcbb0b41b39f317fed176a8394f9ec4163612f2b",
+    "interface_hash": "80a1151f6ae59be2ef7bd25798341a5440572e4d5358ebb1270a6edba965ab68",
     "mtime": 1685143799,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -81,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/importlib_metadata/_itertools.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/importlib_metadata/_text.py",
     "plugin_data": null,
-    "size": 2068,
+    "size": 2166,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_text.data.json` & `su6-0.3.0/.mypy_cache/3.11/importlib_metadata/_text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/pager.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7096969696969696%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 29), (1, 30), (2, 1), (3, 2), (4, 1)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(1, 5), (2, 5), (3, 5), (5, 30), (6, 30)], delete: [1]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.__main__'), (1, 'rich.console'), (4, 'builtins'), (5, "*

 * *                   "'_random'), (6, 'datetime'), (7, 'importlib'), (8, 'rich.jupyter'), (9, "*

 * *                   "'rich.style'), (10, 'rich.table'), (11, 'rich.text'), (12, 'rich.theme'), (13, "*

 * *                   " […]*

```diff
@@ -1,50 +1,62 @@
 {
-    "data_mtime": 1685143879,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        3,
+        29,
+        30,
+        1,
+        2,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
         5,
+        5,
+        5,
+        5,
+        30,
+        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "importlib_metadata._functools",
-        "re",
-        "builtins",
+        "rich.__main__",
+        "rich.console",
         "abc",
-        "array",
-        "ctypes",
-        "enum",
-        "mmap",
-        "pickle",
-        "typing"
+        "typing",
+        "builtins",
+        "_random",
+        "datetime",
+        "importlib",
+        "rich.jupyter",
+        "rich.style",
+        "rich.table",
+        "rich.text",
+        "rich.theme",
+        "types"
     ],
-    "hash": "1c2b0592c66924b7933f734493f9e0ac079755146d4ebb7287d78e001a113f80",
-    "id": "importlib_metadata._text",
+    "hash": "48efc44c114a6e0de7fc080ecd79b8d52bf7e98c57032237fd1f8a398dbfb927",
+    "id": "rich.pager",
     "ignore_all": true,
-    "interface_hash": "80a1151f6ae59be2ef7bd25798341a5440572e4d5358ebb1270a6edba965ab68",
-    "mtime": 1685143799,
+    "interface_hash": "459e2e84034139b55dbab928e42d39aeaa0e874ccc261e1c24a435dd20953020",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -78,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/importlib_metadata/_text.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/pager.py",
     "plugin_data": null,
-    "size": 2166,
+    "size": 828,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/json/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/json/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685283590'}*

```diff
@@ -27,15 +27,15 @@
         "builtins",
         "abc"
     ],
     "hash": "5e17291feef29d72276962727f64c6d0328ab777c2ff53b0be7dace84e9a79f6",
     "id": "json",
     "ignore_all": true,
     "interface_hash": "bf18996540bc47e1664c9a0a23332b42adf07134cb6c4ef19f5da4cc1b42a273",
-    "mtime": 1685143295,
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/json/decoder.data.json` & `su6-0.3.0/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/json/decoder.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7422222222222222%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 4)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (2, 30)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 're'), (3, 'typing')], delete: [1, 0]}",*

 * * "'hash'": "'d2ae501644a75ff97b39bdfb3034a3d94613d289c23f3ff4ee15287762be6ba0'",*

 * * "'id'": "'markdown_it.common.html_re'",*

 * * "'interface_hash'": "'9142291d0a031fd3e87c9e711b279902080af901c30f34c8f274c9599aa462df'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/m […]*

```diff
@@ -1,32 +1,32 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        4,
         1,
-        2,
         1,
         1
     ],
     "dep_prios": [
+        10,
         5,
-        5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "typing",
+        "re",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "5dd5349e16128655996d25e9c4676c82eaed3374bf9740bd98360257d4df6a29",
-    "id": "json.decoder",
+    "hash": "d2ae501644a75ff97b39bdfb3034a3d94613d289c23f3ff4ee15287762be6ba0",
+    "id": "markdown_it.common.html_re",
     "ignore_all": true,
-    "interface_hash": "fc463b2e147ff6395c1c12cef7cd5d5aa5d3e10f5c41b66aa1dddc135ae77e51",
-    "mtime": 1685143295,
+    "interface_hash": "9142291d0a031fd3e87c9e711b279902080af901c30f34c8f274c9599aa462df",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/decoder.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/common/html_re.py",
     "plugin_data": null,
-    "size": 1117,
+    "size": 929,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/json/encoder.data.json` & `su6-0.3.0/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/json/encoder.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/_compat.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7515873015873016%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 1), (2, 4), (3, 5), (4, 1)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 10), (5, 30)]}',*

 * * "'dependencies'": "{insert: [(1, '__future__'), (2, 'sys'), (5, '_typeshed')], delete: [1]}",*

 * * "'hash'": "'9f8672df4cc31cc5e3d66a63bca292db2596c039fce1816a2a311089b7371c99'",*

 * * "'id'": "'markdown_it._compat'",*

 * * "'interface_hash'": "'2dce51e6de3b6e5d526407624bf715b722ef736235e2727a592ff1d462244581'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/py […]*

```diff
@@ -1,35 +1,41 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        1,
-        2,
         3,
         1,
+        4,
+        5,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        10,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "re",
+        "__future__",
+        "sys",
         "typing",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "0c53d66512d44e95d7981a43ef5d83801a9e12c6aaa65b05a35074fecb1ef07f",
-    "id": "json.encoder",
+    "hash": "9f8672df4cc31cc5e3d66a63bca292db2596c039fce1816a2a311089b7371c99",
+    "id": "markdown_it._compat",
     "ignore_all": true,
-    "interface_hash": "5e7ae11c6ee6936f28efa0e308818439ac6cd408e83858317d2b9037426bb289",
-    "mtime": 1685143295,
+    "interface_hash": "2dce51e6de3b6e5d526407624bf715b722ef736235e2727a592ff1d462244581",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/encoder.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/_compat.py",
     "plugin_data": null,
-    "size": 1073,
+    "size": 248,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/logging/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/logging/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7314988558352403%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 7), (1, 8), (6, 1), (7, 1), (8, 1), (9, 1)], delete: [10, 9, 8, 7, '*

 * *                '6, 5, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 10), (7, 30), (8, 30), (9, 30), (10, 30)], delete: [5, 4, 3, 2, 1, '*

 * *                '0]}',*

 * * "'dependencies'": "{insert: [(0, 'typer._typing'), (1, 'typer.models'), (2, 'inspect'), (3, "*

 * *                   "'copy'), (8, 'click'), (9, 'click.core'), (10, 'click.shell_completion'), (11, "*

 * *                   "'click.types' […]*

```diff
@@ -1,61 +1,58 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        4,
+        7,
+        8,
         1,
         2,
         3,
         5,
-        6,
-        7,
-        8,
-        9,
-        10,
-        11,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        10,
-        5,
-        5,
-        5,
-        5,
         5,
+        10,
         5,
         5,
         5,
         5,
         30,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
-        "threading",
-        "_typeshed",
-        "io",
-        "re",
-        "string",
-        "time",
-        "types",
+        "typer._typing",
+        "typer.models",
+        "inspect",
+        "copy",
         "typing",
         "typing_extensions",
         "builtins",
         "abc",
-        "os"
+        "click",
+        "click.core",
+        "click.shell_completion",
+        "click.types",
+        "types"
     ],
-    "hash": "efc0ae6530114eeb664869aab1a543a7e88f59df3c5c479d47e85dff0c989728",
-    "id": "logging",
+    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
+    "id": "typer.utils",
     "ignore_all": true,
-    "interface_hash": "6cbb4e8d90f49e871cd2109526db7296823c495b45acf5b495d714a78376aa50",
+    "interface_hash": "a2a85c807b26672ed4a26c19c9b4e841141ca67ec475f5c25733d86efba2979d",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -90,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/logging/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/utils.py",
     "plugin_data": null,
-    "size": 27004,
+    "size": 7293,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/_compat.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/_compat.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7471428571428571%*

 * *Differences: {"'data_mtime'": '1685143684',*

 * * "'dep_lines'": '{delete: [3, 2]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'markdown_it.rules_inline.state_inline'), (3, "*

 * *                   "'markdown_it.ruler'), (4, 'typing')], delete: [5, 3, 2, 1, 0]}",*

 * * "'hash'": "'6a172951d7fed25d31359ef48be6e1e05be0a118eb9e4a17272c11eeac4ed6bc'",*

 * * "'id'": "'markdown_it.rules_inline.balance_pairs'",*

 * * "'interface_hash'": "'d5318932ca6787d6f7ffbef89f6ca21d3595bec0713dcd65d5253a829d7b242 […]*

```diff
@@ -1,40 +1,34 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143684,
     "dep_lines": [
         3,
         1,
-        4,
-        5,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        10,
-        5,
-        5,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "__future__",
-        "sys",
-        "typing",
+        "markdown_it.rules_inline.state_inline",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "markdown_it.ruler",
+        "typing"
     ],
-    "hash": "9f8672df4cc31cc5e3d66a63bca292db2596c039fce1816a2a311089b7371c99",
-    "id": "markdown_it._compat",
+    "hash": "6a172951d7fed25d31359ef48be6e1e05be0a118eb9e4a17272c11eeac4ed6bc",
+    "id": "markdown_it.rules_inline.balance_pairs",
     "ignore_all": true,
-    "interface_hash": "2dce51e6de3b6e5d526407624bf715b722ef736235e2727a592ff1d462244581",
+    "interface_hash": "d5318932ca6787d6f7ffbef89f6ca21d3595bec0713dcd65d5253a829d7b242f",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -69,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/_compat.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py",
     "plugin_data": null,
-    "size": 248,
+    "size": 4062,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/_punycode.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/_punycode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7761904761904762%*

 * *Differences: {"'dep_lines'": '{delete: [3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [4, 3, 1, 0]}',*

 * * "'dependencies'": '{delete: [6, 3, 1, 0]}',*

 * * "'hash'": "'957fcd985ea46df550b39a124d8b07aae239c2a9074d38ca93e352c5c0879f8a'",*

 * * "'id'": "'markdown_it.presets.default'",*

 * * "'interface_hash'": "'1fcfb104c14c57a8624b9f624302872a6c8822ec1854ba5ea6a7f1279fbe4f99'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/presets/default.py'",*

 * * "'size'": '1765'}*

```diff
@@ -1,40 +1,28 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        23,
-        24,
-        1,
-        1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        10,
         5,
         30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "codecs",
-        "re",
         "builtins",
-        "_codecs",
         "abc",
-        "typing",
-        "typing_extensions"
+        "typing"
     ],
-    "hash": "04ea0e61e6345da5e1b63e6614e7c6539aec3956e4a744ae896763dd95a2f758",
-    "id": "markdown_it._punycode",
+    "hash": "957fcd985ea46df550b39a124d8b07aae239c2a9074d38ca93e352c5c0879f8a",
+    "id": "markdown_it.presets.default",
     "ignore_all": true,
-    "interface_hash": "c00c6f578fc55ea1557781a8ed60305791b12208a2c8b08fb8cb4547d1d11c78",
+    "interface_hash": "1fcfb104c14c57a8624b9f624302872a6c8822ec1854ba5ea6a7f1279fbe4f99",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -69,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/_punycode.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/presets/default.py",
     "plugin_data": null,
-    "size": 2317,
+    "size": 1765,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/main.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/main.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_block.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_core.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/renderer.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/renderer.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/ruler.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/ruler.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/ruler.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/ruler.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/token.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/token.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/utils.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/utils.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7708333333333334%*

 * *Differences: {"'dep_lines'": '{delete: [4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [5, 4, 2, 1, 0]}',*

 * * "'dependencies'": '{delete: [7, 5, 2, 1, 0]}',*

 * * "'hash'": "'cbf3e0a7955accd025114614677df007b2b0c269e3c70674156c890306115139'",*

 * * "'id'": "'markdown_it.presets.zero'",*

 * * "'interface_hash'": "'bfc58c2b73c1b4a7f676b45d0a45cae9f79f5041a38d88ee925c3045cca6c2b7'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/presets/zero.py'",*

 * * "'size'": '2006'}*

```diff
@@ -1,43 +1,28 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        3,
-        1,
-        4,
-        1,
-        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
-        5,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "__future__",
-        "pathlib",
         "builtins",
         "abc",
-        "os",
-        "typing",
-        "typing_extensions"
+        "typing"
     ],
-    "hash": "7e50fb1929681b26c48175d5684df528a9b00250704a6177e5de131a67febabf",
-    "id": "markdown_it.utils",
+    "hash": "cbf3e0a7955accd025114614677df007b2b0c269e3c70674156c890306115139",
+    "id": "markdown_it.presets.zero",
     "ignore_all": true,
-    "interface_hash": "8335636d49a8bfa20d8496a08427c175714de0547c045ada302dee9e385bebc9",
+    "interface_hash": "bfc58c2b73c1b4a7f676b45d0a45cae9f79f5041a38d88ee925c3045cca6c2b7",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/presets/zero.py",
     "plugin_data": null,
-    "size": 3262,
+    "size": 2006,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.76%*

 * *Differences: {"'data_mtime'": '1685143684',*

 * * "'dep_lines'": '{insert: [(0, 3), (1, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (2, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'markdown_it.common.utils'), (3, 'markdown_it.common')]}",*

 * * "'hash'": "'c27f6b0a1925685bb19785121ee77536618a7df357cb6307fb5c6adcaf366d8a'",*

 * * "'id'": "'markdown_it.helpers.parse_link_title'",*

 * * "'interface_hash'": "'76b204d20f42cff8ce2106b155e3329779299085797dce9983b3dbf875fa9df8'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site […]*

```diff
@@ -1,28 +1,34 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143684,
     "dep_lines": [
+        3,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        30,
         30,
         30
     ],
     "dependencies": [
+        "markdown_it.common.utils",
         "builtins",
         "abc",
+        "markdown_it.common",
         "typing"
     ],
-    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
-    "id": "markdown_it.common",
+    "hash": "c27f6b0a1925685bb19785121ee77536618a7df357cb6307fb5c6adcaf366d8a",
+    "id": "markdown_it.helpers.parse_link_title",
     "ignore_all": true,
-    "interface_hash": "025d277b435885d2ab21746beda078a54170d7202b39271c651ced3c454e2915",
+    "interface_hash": "76b204d20f42cff8ce2106b155e3329779299085797dce9983b3dbf875fa9df8",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -57,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/common/__init__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py",
     "plugin_data": null,
-    "size": 0,
+    "size": 1410,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/entities.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.76%*

 * *Differences: {"'data_mtime'": '1685143684',*

 * * "'dep_lines'": '{insert: [(1, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (2, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'markdown_it.rules_inline.state_inline'), (3, "*

 * *                   "'markdown_it.ruler')], delete: [0]}",*

 * * "'hash'": "'65b2fc0b43b5b825472278dfb8aa548c5a515c57b97b5e6ba9289d845da16db1'",*

 * * "'id'": "'markdown_it.rules_inline.text'",*

 * * "'interface_hash'": "'86ef54d7833c704c55a5f05b276d95a6dccf83eee446e767d6090b8a90f188ae'",*

 * * "'path'": "'/home/robin/we […]*

```diff
@@ -1,31 +1,34 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143684,
     "dep_lines": [
         4,
         1,
         1,
+        1,
         1
     ],
     "dep_prios": [
-        10,
         5,
+        5,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "re",
+        "markdown_it.rules_inline.state_inline",
         "builtins",
         "abc",
+        "markdown_it.ruler",
         "typing"
     ],
-    "hash": "d2ae501644a75ff97b39bdfb3034a3d94613d289c23f3ff4ee15287762be6ba0",
-    "id": "markdown_it.common.html_re",
+    "hash": "65b2fc0b43b5b825472278dfb8aa548c5a515c57b97b5e6ba9289d845da16db1",
+    "id": "markdown_it.rules_inline.text",
     "ignore_all": true,
-    "interface_hash": "9142291d0a031fd3e87c9e711b279902080af901c30f34c8f274c9599aa462df",
+    "interface_hash": "86ef54d7833c704c55a5f05b276d95a6dccf83eee446e767d6090b8a90f188ae",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -60,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/common/html_re.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py",
     "plugin_data": null,
-    "size": 929,
+    "size": 1427,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/utils.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7898148148148147%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 4), (1, 5), (2, 1), (3, 1)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (3, 30), (4, 30)]}',*

 * * "'dependencies'": "{insert: [(1, 'markdown_it.rules_inline.state_inline'), (5, "*

 * *                   "'markdown_it.ruler'), (7, 'typing_extensions')]}",*

 * * "'hash'": "'be4c18f47bf69666ad7fa13820fb2cee4a1b7a49de7c519cc470d4b05c323ded'",*

 * * "'id'": "'markdown_it.rules_inline.escape'",*

 * * "'interface_hash'": "'4d41fab364a12e6c62f3bfaad7ea40964d1959b1793e7ad7a61788f72655c34b'",*

 * * "'path'": […]*

```diff
@@ -1,34 +1,43 @@
 {
     "data_mtime": 1685143684,
     "dep_lines": [
-        3,
+        4,
+        5,
+        1,
+        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        5,
+        30,
+        30,
         30,
         30,
         30
     ],
     "dependencies": [
         "markdown_it.common.utils",
+        "markdown_it.rules_inline.state_inline",
         "builtins",
         "abc",
         "markdown_it.common",
-        "typing"
+        "markdown_it.ruler",
+        "typing",
+        "typing_extensions"
     ],
-    "hash": "c27f6b0a1925685bb19785121ee77536618a7df357cb6307fb5c6adcaf366d8a",
-    "id": "markdown_it.helpers.parse_link_title",
+    "hash": "be4c18f47bf69666ad7fa13820fb2cee4a1b7a49de7c519cc470d4b05c323ded",
+    "id": "markdown_it.rules_inline.escape",
     "ignore_all": true,
-    "interface_hash": "76b204d20f42cff8ce2106b155e3329779299085797dce9983b3dbf875fa9df8",
+    "interface_hash": "4d41fab364a12e6c62f3bfaad7ea40964d1959b1793e7ad7a61788f72655c34b",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -63,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py",
     "plugin_data": null,
-    "size": 1410,
+    "size": 1116,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/default.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/default.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_export_format.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'hash'": "'ab1815de72a75d0bb585f6e7455b303d8cbe030220d57d0b482e3b70ae6cf239'",*

 * * "'id'": "'rich._export_format'",*

 * * "'interface_hash'": "'fd571c31ad724d67686183b09d73659e24b116ab584d9801c76ba413fab9f8e8'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_export_format.py'",*

 * * "'size'": '2100'}*

```diff
@@ -11,18 +11,18 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "957fcd985ea46df550b39a124d8b07aae239c2a9074d38ca93e352c5c0879f8a",
-    "id": "markdown_it.presets.default",
+    "hash": "ab1815de72a75d0bb585f6e7455b303d8cbe030220d57d0b482e3b70ae6cf239",
+    "id": "rich._export_format",
     "ignore_all": true,
-    "interface_hash": "1fcfb104c14c57a8624b9f624302872a6c8822ec1854ba5ea6a7f1279fbe4f99",
+    "interface_hash": "fd571c31ad724d67686183b09d73659e24b116ab584d9801c76ba413fab9f8e8",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -57,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/presets/default.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_export_format.py",
     "plugin_data": null,
-    "size": 1765,
+    "size": 2100,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7288888888888889%*

 * *Differences: {"'data_mtime'": '1685143684',*

 * * "'dep_lines'": '{insert: [(0, 3), (1, 6), (2, 7), (3, 1), (4, 4), (5, 10)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (3, 5), (4, 5), (5, 25)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'markdown_it.ruler'), (2, "*

 * *                   "'markdown_it.token'), (3, '__future__'), (4, 'typing'), (5, 'markdown_it'), "*

 * *                   "(8, 'markdown_it.main')], delete: [2]}",*

 * * "'hash'": "'043f7ba8bee366d3cc3b1ab107eec2c670edc9bf33e93e53a7b1949bfae30879' […]*

```diff
@@ -1,28 +1,46 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143684,
     "dep_lines": [
+        3,
+        6,
+        7,
+        1,
+        4,
+        10,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        5,
+        5,
+        5,
+        25,
+        5,
         30,
         30
     ],
     "dependencies": [
+        "collections.abc",
+        "markdown_it.ruler",
+        "markdown_it.token",
+        "__future__",
+        "typing",
+        "markdown_it",
         "builtins",
         "abc",
-        "typing"
+        "markdown_it.main"
     ],
-    "hash": "cbf3e0a7955accd025114614677df007b2b0c269e3c70674156c890306115139",
-    "id": "markdown_it.presets.zero",
+    "hash": "043f7ba8bee366d3cc3b1ab107eec2c670edc9bf33e93e53a7b1949bfae30879",
+    "id": "markdown_it.rules_core.state_core",
     "ignore_all": true,
-    "interface_hash": "bfc58c2b73c1b4a7f676b45d0a45cae9f79f5041a38d88ee925c3045cca6c2b7",
+    "interface_hash": "70d545fed3e82eac5ad3ded8cc1cab43b8b5d7c6226600dba6d074a917ff43c6",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -57,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/presets/zero.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py",
     "plugin_data": null,
-    "size": 2006,
+    "size": 584,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7646214896214897%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 2), (2, 1), (3, 1), (4, 1)], delete: [5, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 30), (4, 30), (5, 30)], delete: [5, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'markdown_it.rules_inline.state_inline'), (4, "*

 * *                   "'markdown_it.ruler'), (5, 'markdown_it.token'), (6, 'typing'), (7, "*

 * *                   "'typing_extensions')], delete: [8, 5, 4, 2, 1, 0]}",*

 * * "'hash'": "'6dc276504c210fb7895b540862405bb06b45f26336dcc89423f6138c63c45fb3'",*

 * * "'id'": "'markdown_i […]*

```diff
@@ -1,46 +1,43 @@
 {
     "data_mtime": 1685143684,
     "dep_lines": [
-        3,
-        6,
-        7,
-        1,
         4,
-        10,
+        2,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
-        5,
-        5,
-        25,
-        5,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "markdown_it.ruler",
-        "markdown_it.token",
+        "markdown_it.rules_inline.state_inline",
         "__future__",
-        "typing",
-        "markdown_it",
         "builtins",
         "abc",
-        "markdown_it.main"
+        "markdown_it.ruler",
+        "markdown_it.token",
+        "typing",
+        "typing_extensions"
     ],
-    "hash": "043f7ba8bee366d3cc3b1ab107eec2c670edc9bf33e93e53a7b1949bfae30879",
-    "id": "markdown_it.rules_core.state_core",
+    "hash": "6dc276504c210fb7895b540862405bb06b45f26336dcc89423f6138c63c45fb3",
+    "id": "markdown_it.rules_inline.strikethrough",
     "ignore_all": true,
-    "interface_hash": "70d545fed3e82eac5ad3ded8cc1cab43b8b5d7c6226600dba6d074a917ff43c6",
+    "interface_hash": "9ed5241e2b3b47089b80cbe9f411932cee3922ee62180f21161b01bafe9e822e",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -75,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py",
     "plugin_data": null,
-    "size": 584,
+    "size": 3390,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json` & `su6-0.3.0/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7366666666666667%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{delete: [0]}',*

 * * "'dep_prios'": '{delete: [2]}',*

 * * "'dependencies'": "{insert: [(0, '_collections_abc')], delete: [3, 0]}",*

 * * "'hash'": "'90189900dd153dff2aa642276e3a8a65145ed0f5eb67b8f1366086b38a3950e7'",*

 * * "'id'": "'collections.abc'",*

 * * "'interface_hash'": "'06bab035dfaa5f3ad1efba42299a607e80d44d225139ec1f803fdb074d7a9d93'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/collection […]*

```diff
@@ -1,35 +1,32 @@
 {
-    "data_mtime": 1685143684,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        3,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         30,
-        30,
         30
     ],
     "dependencies": [
-        "markdown_it.rules_inline.state_inline",
+        "_collections_abc",
         "builtins",
         "abc",
-        "markdown_it.ruler",
         "typing"
     ],
-    "hash": "6a172951d7fed25d31359ef48be6e1e05be0a118eb9e4a17272c11eeac4ed6bc",
-    "id": "markdown_it.rules_inline.balance_pairs",
+    "hash": "90189900dd153dff2aa642276e3a8a65145ed0f5eb67b8f1366086b38a3950e7",
+    "id": "collections.abc",
     "ignore_all": true,
-    "interface_hash": "d5318932ca6787d6f7ffbef89f6ca21d3595bec0713dcd65d5253a829d7b242f",
-    "mtime": 1685143296,
+    "interface_hash": "06bab035dfaa5f3ad1efba42299a607e80d44d225139ec1f803fdb074d7a9d93",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +60,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/collections/abc.pyi",
     "plugin_data": null,
-    "size": 4062,
+    "size": 79,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8024242424242424%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 3), (2, 1), (3, 1)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(3, 30), (4, 30)]}',*

 * * "'dependencies'": "{insert: [(5, 'markdown_it.main'), (6, 'markdown_it.parser_inline'), (8, "*

 * *                   "'markdown_it.utils')], delete: [7]}",*

 * * "'hash'": "'f72f49a8720b12555e280fb2e85b469fbb4b5116827304c8550f065368779b36'",*

 * * "'id'": "'markdown_it.rules_inline.link'",*

 * * "'interface_hash'": "'ddb9af2331d6d5295d16bea768685007ab8fa6d38a2b597eddd9601f9bc59974'",*

 * * "'path'": "'/home/robin/wer […]*

```diff
@@ -1,12 +1,14 @@
 {
     "data_mtime": 1685143684,
     "dep_lines": [
+        3,
         4,
-        5,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
@@ -14,30 +16,34 @@
         5,
         5,
         5,
         30,
         30,
         30,
         30,
+        30,
+        30,
         30
     ],
     "dependencies": [
         "markdown_it.common.utils",
         "markdown_it.rules_inline.state_inline",
         "builtins",
         "abc",
         "markdown_it.common",
+        "markdown_it.main",
+        "markdown_it.parser_inline",
         "markdown_it.ruler",
-        "typing",
-        "typing_extensions"
+        "markdown_it.utils",
+        "typing"
     ],
-    "hash": "be4c18f47bf69666ad7fa13820fb2cee4a1b7a49de7c519cc470d4b05c323ded",
-    "id": "markdown_it.rules_inline.escape",
+    "hash": "f72f49a8720b12555e280fb2e85b469fbb4b5116827304c8550f065368779b36",
+    "id": "markdown_it.rules_inline.link",
     "ignore_all": true,
-    "interface_hash": "4d41fab364a12e6c62f3bfaad7ea40964d1959b1793e7ad7a61788f72655c34b",
+    "interface_hash": "ddb9af2331d6d5295d16bea768685007ab8fa6d38a2b597eddd9601f9bc59974",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py",
     "plugin_data": null,
-    "size": 1116,
+    "size": 4362,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7924242424242425%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 5), (2, 2)], delete: [4, 3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 10)], delete: [5, 4, 3]}',*

 * * "'dependencies'": "{insert: [(2, 're')], delete: [8, 6, 5]}",*

 * * "'hash'": "'5ebf0130b63ab316314bf173fc9da9a8d8394fb3df581c01beecc0e114e339f4'",*

 * * "'id'": "'markdown_it.rules_inline.newline'",*

 * * "'interface_hash'": "'5b0e3a9a0df9d98fa4d82bcbad9a7426fee2153fdfbec205941c6c87f6d2b271'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inli […]*

```diff
@@ -1,49 +1,43 @@
 {
     "data_mtime": 1685143684,
     "dep_lines": [
-        3,
         4,
-        1,
-        1,
-        1,
+        5,
+        2,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        10,
         5,
         30,
         30,
         30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
         "markdown_it.common.utils",
         "markdown_it.rules_inline.state_inline",
+        "re",
         "builtins",
         "abc",
         "markdown_it.common",
-        "markdown_it.main",
-        "markdown_it.parser_inline",
         "markdown_it.ruler",
-        "markdown_it.utils",
         "typing"
     ],
-    "hash": "f72f49a8720b12555e280fb2e85b469fbb4b5116827304c8550f065368779b36",
-    "id": "markdown_it.rules_inline.link",
+    "hash": "5ebf0130b63ab316314bf173fc9da9a8d8394fb3df581c01beecc0e114e339f4",
+    "id": "markdown_it.rules_inline.newline",
     "ignore_all": true,
-    "interface_hash": "ddb9af2331d6d5295d16bea768685007ab8fa6d38a2b597eddd9601f9bc59974",
+    "interface_hash": "5b0e3a9a0df9d98fa4d82bcbad9a7426fee2153fdfbec205941c6c87f6d2b271",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -78,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py",
     "plugin_data": null,
-    "size": 4362,
+    "size": 1176,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7888888888888889%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 1), (1, 1)], delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [2, 0]}',*

 * * "'dependencies'": "{insert: [(4, 'markdown_it.token'), (6, 'typing_extensions')], delete: [5, 2, "*

 * *                   '0]}',*

 * * "'hash'": "'51518d384b2588b5a6b67208deb39ad5dc74297fe0ad195ee371ff8f9a7d5715'",*

 * * "'id'": "'markdown_it.rules_inline.text_collapse'",*

 * * "'interface_hash'": "'cc76853f0ed01464c1c34a90e4e8727590159c01448b7b98fe088cdfccab6792'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-c […]*

```diff
@@ -1,43 +1,40 @@
 {
     "data_mtime": 1685143684,
     "dep_lines": [
-        4,
-        5,
-        2,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        10,
-        5,
+        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "markdown_it.common.utils",
         "markdown_it.rules_inline.state_inline",
-        "re",
         "builtins",
         "abc",
-        "markdown_it.common",
         "markdown_it.ruler",
-        "typing"
+        "markdown_it.token",
+        "typing",
+        "typing_extensions"
     ],
-    "hash": "5ebf0130b63ab316314bf173fc9da9a8d8394fb3df581c01beecc0e114e339f4",
-    "id": "markdown_it.rules_inline.newline",
+    "hash": "51518d384b2588b5a6b67208deb39ad5dc74297fe0ad195ee371ff8f9a7d5715",
+    "id": "markdown_it.rules_inline.text_collapse",
     "ignore_all": true,
-    "interface_hash": "5b0e3a9a0df9d98fa4d82bcbad9a7426fee2153fdfbec205941c6c87f6d2b271",
+    "interface_hash": "cc76853f0ed01464c1c34a90e4e8727590159c01448b7b98fe088cdfccab6792",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/text_collapse.py",
     "plugin_data": null,
-    "size": 1176,
+    "size": 1491,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json` & `su6-0.3.0/.mypy_cache/3.11/types.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6921428571428571%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 3), (1, 16), (3, 2), (4, 19), (5, 20), (6, 607)], delete: [4, 3, 2, '*

 * *                '1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 10), (4, 5), (5, 5), (6, 5)], delete: [5, 4, 3]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'importlib.machinery'), (2, 'sys'), (3, "*

 * *                   "'_typeshed'), (6, 'builtins'), (7, 'abc'), (8, 'importlib')], delete: [5, 4, "*

 * *                   '3, 2, 1, 0]}',*

 * * "'hash'": "'bb1594589ec5ca09736286838 […]*

```diff
@@ -1,44 +1,47 @@
 {
-    "data_mtime": 1685143684,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        4,
-        2,
-        1,
-        1,
-        1,
+        3,
+        16,
         1,
+        2,
+        19,
+        20,
+        607,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        10,
+        5,
+        5,
+        5,
         5,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "markdown_it.rules_inline.state_inline",
-        "__future__",
+        "collections.abc",
+        "importlib.machinery",
+        "sys",
+        "_typeshed",
+        "typing",
+        "typing_extensions",
         "builtins",
         "abc",
-        "markdown_it.ruler",
-        "markdown_it.token",
-        "typing",
-        "typing_extensions"
+        "importlib"
     ],
-    "hash": "6dc276504c210fb7895b540862405bb06b45f26336dcc89423f6138c63c45fb3",
-    "id": "markdown_it.rules_inline.strikethrough",
+    "hash": "bb1594589ec5ca09736286838e17153b5f7c33e7eaa783ab884856ab9bbd8f04",
+    "id": "types",
     "ignore_all": true,
-    "interface_hash": "9ed5241e2b3b47089b80cbe9f411932cee3922ee62180f21161b01bafe9e822e",
-    "mtime": 1685143296,
+    "interface_hash": "fea64d1cb455db2f23e925fb7c8aed26dd9823e8395482957e120518d869eabb",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/types.pyi",
     "plugin_data": null,
-    "size": 3390,
+    "size": 20809,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/highlighter.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7265109890109891%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 5), (1, 202), (2, 1), (3, 2), (4, 3), (5, 230), (6, 1), (7, 1), (8, '*

 * *                '1)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 10), (3, 5), (5, 10), (7, 30), (8, 30), (9, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.text'), (1, 'rich.console'), (2, 're'), (5, 'json'), (6, "*

 * *                   "'builtins'), (7, '_random'), (8, 'datetime'), (9, 'json.encoder'), (10, "*

 * *                   "'rich.jupyter'), (11, 'rich.sty […]*

```diff
@@ -1,34 +1,58 @@
 {
-    "data_mtime": 1685143684,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        4,
+        5,
+        202,
+        1,
+        2,
+        3,
+        230,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        10,
+        5,
+        5,
+        10,
+        5,
+        30,
+        30,
+        30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "markdown_it.rules_inline.state_inline",
-        "builtins",
+        "rich.text",
+        "rich.console",
+        "re",
         "abc",
-        "markdown_it.ruler",
-        "typing"
+        "typing",
+        "json",
+        "builtins",
+        "_random",
+        "datetime",
+        "json.encoder",
+        "rich.jupyter",
+        "rich.style",
+        "rich.theme"
     ],
-    "hash": "65b2fc0b43b5b825472278dfb8aa548c5a515c57b97b5e6ba9289d845da16db1",
-    "id": "markdown_it.rules_inline.text",
+    "hash": "a770b5838418cdecc529d47b345f4484f6f3403bdd3d48464604b21861263e4a",
+    "id": "rich.highlighter",
     "ignore_all": true,
-    "interface_hash": "86ef54d7833c704c55a5f05b276d95a6dccf83eee446e767d6090b8a90f188ae",
+    "interface_hash": "9f1264bb283838e4d5e234aea219b1e866711ec3938d007140d0e914dd5f52b3",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -63,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/highlighter.py",
     "plugin_data": null,
-    "size": 1427,
+    "size": 9584,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json` & `su6-0.3.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_ast.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7023569023569024%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(1, 2), (2, 3)], delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (3, 5)], delete: [4, 3, 2]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (3, 'builtins'), (4, '_typeshed'), (5, 'abc')], delete: "*

 * *                   '[4, 3, 2, 1, 0]}',*

 * * "'hash'": "'189ca9e5f979d2fafddf0fde549a04c4da5840422b279c427ac3b84df670b646'",*

 * * "'id'": "'_ast'",*

 * * "'interface_hash'": "'7aaf7eb03088c4a732c70e702b755199cfa669aed9dbaf9b63d04ceb2f07d568'",*

 * * "'mtime'": '1685283 […]*

```diff
@@ -1,41 +1,38 @@
 {
-    "data_mtime": 1685143684,
+    "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        1,
-        1,
-        1,
+        2,
+        3,
         1,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
         5,
         5,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "markdown_it.rules_inline.state_inline",
-        "builtins",
-        "abc",
-        "markdown_it.ruler",
-        "markdown_it.token",
+        "sys",
         "typing",
-        "typing_extensions"
+        "typing_extensions",
+        "builtins",
+        "_typeshed",
+        "abc"
     ],
-    "hash": "51518d384b2588b5a6b67208deb39ad5dc74297fe0ad195ee371ff8f9a7d5715",
-    "id": "markdown_it.rules_inline.text_collapse",
+    "hash": "189ca9e5f979d2fafddf0fde549a04c4da5840422b279c427ac3b84df670b646",
+    "id": "_ast",
     "ignore_all": true,
-    "interface_hash": "cc76853f0ed01464c1c34a90e4e8727590159c01448b7b98fe088cdfccab6792",
-    "mtime": 1685143296,
+    "interface_hash": "7aaf7eb03088c4a732c70e702b755199cfa669aed9dbaf9b63d04ceb2f07d568",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/markdown_it/rules_inline/text_collapse.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_ast.pyi",
     "plugin_data": null,
-    "size": 1491,
+    "size": 14752,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_inspect.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6916006982503146%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 7), (1, 8), (2, 9), (3, 10), (4, 11), (5, 12), (6, 13), (8, 1), (9, '*

 * *                '3), (10, 5), (11, 1), (12, 1), (13, 1)], delete: [4, 3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (3, 5), (4, 5), (5, 5), (12, 30), (13, 30), '*

 * *                '(14, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.console'), (1, 'rich.control'), (2, 'rich.highlighter'), "*

 * *                   "(3, 'rich.jupyter'), (4, 'rich.panel'), (5, 'rich.pr […]*

```diff
@@ -1,44 +1,71 @@
 {
-    "data_mtime": 1685143684,
+    "data_mtime": 1685143685,
     "dep_lines": [
+        7,
+        8,
+        9,
+        10,
+        11,
+        12,
+        13,
         14,
-        15,
-        16,
-        17,
-        18,
+        1,
+        3,
+        5,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
         5,
         5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "mdurl._decode",
-        "mdurl._encode",
-        "mdurl._format",
-        "mdurl._parse",
-        "mdurl._url",
+        "rich.console",
+        "rich.control",
+        "rich.highlighter",
+        "rich.jupyter",
+        "rich.panel",
+        "rich.pretty",
+        "rich.table",
+        "rich.text",
+        "__future__",
+        "inspect",
+        "typing",
         "builtins",
+        "_typeshed",
         "abc",
-        "typing"
+        "rich.box",
+        "rich.style",
+        "typing_extensions"
     ],
-    "hash": "d6fa44f3d3725e7888459342ff87fa04f9b751be1b3e7b637f2ca12d147ba295",
-    "id": "mdurl",
+    "hash": "a19246c37d5eeb87705d20a6ac39ef65bc156f564a8567d4f30237556a218c99",
+    "id": "rich._inspect",
     "ignore_all": true,
-    "interface_hash": "68709c75b089acb3978892b0b110795b2019253d8373e4bf42394bea8f0b2753",
-    "mtime": 1685143295,
+    "interface_hash": "3ab38dffbfb27fbb716054e011e7e9ca7cde6de73b3aa2110ef99a619c30aa14",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +99,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/__init__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_inspect.py",
     "plugin_data": null,
-    "size": 547,
+    "size": 9695,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_decode.data.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_decode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_decode.meta.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_parse.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7811111111111111%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 47), (1, 42), (2, 44), (3, 45)], delete: [7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 5)], delete: [8, 7, 6, 5, 2]}',*

 * * "'dependencies'": "{insert: [(0, 'mdurl._url'), (2, 'collections')], delete: [11, 10, 8, 7, 2, "*

 * *                   '0]}',*

 * * "'hash'": "'7b365290cdbfe0d436671d38eec11d7091bb3584111478992bb63c20d1c5cf06'",*

 * * "'id'": "'mdurl._parse'",*

 * * "'interface_hash'": "'8331201b79c4227837bdf0937cca95e77b436109850b899bfc0d3b343eb9b37b'",*

 * * "'path'": "'/home/robin/w […]*

```diff
@@ -1,61 +1,49 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        3,
-        1,
-        4,
-        5,
-        1,
-        1,
-        1,
-        1,
+        47,
+        42,
+        44,
+        45,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        10,
+        5,
         10,
         5,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
+        "mdurl._url",
         "__future__",
-        "functools",
+        "collections",
         "re",
         "builtins",
         "_typeshed",
         "abc",
-        "array",
-        "ctypes",
         "enum",
-        "mmap",
-        "pickle",
         "typing",
         "typing_extensions"
     ],
-    "hash": "dd0fe00d0a94fff4ef0dbbbbc7e6fd2e36d5978416cb983fa85c258dcbaf37f6",
-    "id": "mdurl._decode",
+    "hash": "7b365290cdbfe0d436671d38eec11d7091bb3584111478992bb63c20d1c5cf06",
+    "id": "mdurl._parse",
     "ignore_all": true,
-    "interface_hash": "6f5f83a6622ef21ad6e3b0383c8cc478e08bbed44b5e5ee6513bf696f36b56d8",
+    "interface_hash": "8331201b79c4227837bdf0937cca95e77b436109850b899bfc0d3b343eb9b37b",
     "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -90,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_decode.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_parse.py",
     "plugin_data": null,
-    "size": 3004,
+    "size": 11374,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_encode.data.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_encode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_encode.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/scope.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.704728835978836%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(2, 5), (3, 6), (4, 7), (5, 8), (6, 11), (7, 2), (8, 71), (9, 1), (10, '*

 * *                '1)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (3, 5), (6, 25), (10, 30), (11, 30)]}',*

 * * "'dependencies'": "{insert: [(1, 'rich.highlighter'), (2, 'rich.panel'), (3, 'rich.pretty'), (4, "*

 * *                   "'rich.table'), (5, 'rich.text'), (6, 'rich.console'), (7, 'typing'), (8, "*

 * *                   "'rich'), (10, '_typeshed'), (12, 'r […]*

```diff
@@ -1,47 +1,68 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        3,
-        5,
         1,
         4,
+        5,
+        6,
+        7,
+        8,
+        11,
+        2,
+        71,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
         5,
+        5,
+        25,
+        5,
+        5,
+        5,
+        30,
+        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "urllib.parse",
-        "__future__",
-        "string",
+        "rich.highlighter",
+        "rich.panel",
+        "rich.pretty",
+        "rich.table",
+        "rich.text",
+        "rich.console",
+        "typing",
+        "rich",
         "builtins",
+        "_typeshed",
         "abc",
-        "typing",
-        "typing_extensions",
-        "urllib"
+        "rich.box",
+        "rich.jupyter",
+        "rich.style",
+        "typing_extensions"
     ],
-    "hash": "82824b505b75878ad564daaa9bdb75e4dc365be6c55d8404cb7691d352265afb",
-    "id": "mdurl._encode",
+    "hash": "95fe907adfdee09398df89708584801be3415d8281718bbab7f8a0bff2681a88",
+    "id": "rich.scope",
     "ignore_all": true,
-    "interface_hash": "c46a8178501394440815b21cce0bea6c32abcb1c9cad344caff69c21789a1940",
-    "mtime": 1685143295,
+    "interface_hash": "145a049def1168757354bd5707ab359e210969ef05b31e520f7c729e9f2e9a35",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -75,13 +96,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_encode.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/scope.py",
     "plugin_data": null,
-    "size": 2602,
+    "size": 2831,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_format.data.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_format.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7396296296296296%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 2), (3, 4), (4, 7), (5, 1)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5), (6, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (3, 'typing_extensions'), (4, "*

 * *                   "'types'), (6, '_typeshed')], delete: [1, 0]}",*

 * * "'hash'": "'a95feb712aa1ad0440aa1c3ff081329b8a7a976bf976c7cdcd39b1c5d227ea57'",*

 * * "'id'": "'_weakrefset'",*

 * * "'interface_hash'": "'b235dadc5fe23ff0afd8bfe6f1ee02cb171d77545e4c45adbd244eca1a7f68eb' […]*

```diff
@@ -1,35 +1,44 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        6,
+        2,
         1,
         3,
+        4,
+        7,
+        1,
         1,
         1
     ],
     "dep_prios": [
-        25,
+        5,
+        10,
+        5,
         5,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
-        "mdurl._url",
-        "__future__",
+        "collections.abc",
+        "sys",
         "typing",
+        "typing_extensions",
+        "types",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "c5972dd2675e3d70341f7900ab18c6b650793bce86df90c060c1a4038e02981e",
-    "id": "mdurl._format",
+    "hash": "a95feb712aa1ad0440aa1c3ff081329b8a7a976bf976c7cdcd39b1c5d227ea57",
+    "id": "_weakrefset",
     "ignore_all": true,
-    "interface_hash": "dba7009860e9aa1a455609dc3b1b29ec8f98225b3e3cd3619daa07d9eefa2086",
-    "mtime": 1685143295,
+    "interface_hash": "b235dadc5fe23ff0afd8bfe6f1ee02cb171d77545e4c45adbd244eca1a7f68eb",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_format.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi",
     "plugin_data": null,
-    "size": 626,
+    "size": 2383,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_parse.data.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_parse.meta.json` & `su6-0.3.0/.mypy_cache/3.11/argparse.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7357142857142857%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 2), (2, 3), (3, 4), (4, 5)], delete: [5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (5, 5)], delete: [7, 6, 5, 3]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (3, 'typing'), (4, "*

 * *                   "'typing_extensions')], delete: [9, 8, 7, 2, 1, 0]}",*

 * * "'hash'": "'618be6b2698dc6ca55699bc25bcfe656b87890132abbe027335919112c82a99a'",*

 * * "'id'": "'argparse'",*

 * * "'interface_hash'": "'950573db8ee28c2bd1dfeb5a32951017483df0332cbdfe95a31faf381ebb5cd5'" […]*

```diff
@@ -1,50 +1,44 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        47,
-        42,
-        44,
-        45,
-        1,
-        1,
+        2,
         1,
+        3,
+        4,
+        5,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
         5,
         5,
-        10,
         5,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "mdurl._url",
-        "__future__",
-        "collections",
+        "collections.abc",
+        "sys",
         "re",
+        "typing",
+        "typing_extensions",
         "builtins",
         "_typeshed",
-        "abc",
-        "enum",
-        "typing",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "7b365290cdbfe0d436671d38eec11d7091bb3584111478992bb63c20d1c5cf06",
-    "id": "mdurl._parse",
+    "hash": "618be6b2698dc6ca55699bc25bcfe656b87890132abbe027335919112c82a99a",
+    "id": "argparse",
     "ignore_all": true,
-    "interface_hash": "8331201b79c4227837bdf0937cca95e77b436109850b899bfc0d3b343eb9b37b",
-    "mtime": 1685143295,
+    "interface_hash": "950573db8ee28c2bd1dfeb5a32951017483df0332cbdfe95a31faf381ebb5cd5",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -78,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_parse.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/argparse.pyi",
     "plugin_data": null,
-    "size": 11374,
+    "size": 19942,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_url.data.json` & `su6-0.3.0/.mypy_cache/3.11/mdurl/_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/mdurl/_url.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/region.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.775%*

 * *Differences: {"'dep_lines'": '{delete: [1]}',*

 * * "'dep_prios'": '{delete: [0]}',*

 * * "'dependencies'": '{delete: [0]}',*

 * * "'hash'": "'acd4fdc59ad56536085d90b43589f8d42250c1835b47e29e70f3b14e042f07c6'",*

 * * "'id'": "'rich.region'",*

 * * "'interface_hash'": "'3c4daa256da6ee49361e01123ed1955effa6af54d049e46091b27ae9104959b7'",*

 * * "'mtime'": '1685143296',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/region.py'",*

 * * "'size'": '166'}*

```diff
@@ -1,32 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        3,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5,
         30
     ],
     "dependencies": [
-        "__future__",
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "e6442745037603f1b8b2f2e747365c1b46dfa03f406c1ad80d7a2eb031d9df3d",
-    "id": "mdurl._url",
+    "hash": "acd4fdc59ad56536085d90b43589f8d42250c1835b47e29e70f3b14e042f07c6",
+    "id": "rich.region",
     "ignore_all": true,
-    "interface_hash": "2a514ad3dcf650747db692ff0fa23e44a0203118f1fbd0b2df0c38e4c5100970",
-    "mtime": 1685143295,
+    "interface_hash": "3c4daa256da6ee49361e01123ed1955effa6af54d049e46091b27ae9104959b7",
+    "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mdurl/_url.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/region.py",
     "plugin_data": null,
-    "size": 284,
+    "size": 166,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/os/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/os/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_operator.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7308601364522417%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 3), (3, 4), (4, 5)], delete: [13, 12, 11, 10, 9, 8, 7, 6, 5, 4, 1, '*

 * *                '0]}',*

 * * "'dep_prios'": '{delete: [14, 13, 12, 7, 6, 5, 4, 3, 1]}',*

 * * "'dependencies'": "{insert: [(5, 'builtins'), (6, 'abc')], delete: [15, 14, 13, 12, 11, 8, 7, 6, "*

 * *                   '5, 4, 1]}',*

 * * "'hash'": "'6af6cdd45bab26f05bd668e6a9adf75595caa87cbfb531af9addb4e0dd18636a'",*

 * * "'id'": "'_operator'",*

 * * "'interface_hash'": "'f1d7d99b1fca61d4b596b68f2c83c01e2a71cc79a0beede674ee626f73a36f3d'",*

 * *  […]*

```diff
@@ -1,68 +1,41 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        23,
-        30,
+        3,
         1,
         2,
-        21,
-        22,
-        24,
-        25,
-        26,
-        27,
-        28,
-        33,
-        1,
-        1,
+        4,
+        5,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
-        10,
-        5,
-        5,
         5,
         5,
         5,
         5,
-        5,
-        5,
-        5,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "os.path",
         "sys",
         "_typeshed",
-        "abc",
-        "builtins",
-        "contextlib",
-        "io",
-        "subprocess",
         "typing",
         "typing_extensions",
-        "types",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle"
+        "builtins",
+        "abc"
     ],
-    "hash": "43f0abc8936c573dfefd04ae185e74a6fc8eac1be65a0daaaf327303d8dc486e",
-    "id": "os",
+    "hash": "6af6cdd45bab26f05bd668e6a9adf75595caa87cbfb531af9addb4e0dd18636a",
+    "id": "_operator",
     "ignore_all": true,
-    "interface_hash": "7857e0241ab1ae7ccf1c6583d54898fa386079260ac7e105c7e8d281784f77c9",
-    "mtime": 1685143295,
+    "interface_hash": "f1d7d99b1fca61d4b596b68f2c83c01e2a71cc79a0beede674ee626f73a36f3d",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -96,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_operator.pyi",
     "plugin_data": null,
-    "size": 36995,
+    "size": 6585,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/os/path.data.json` & `su6-0.3.0/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/os/path.meta.json` & `su6-0.3.0/.mypy_cache/3.11/tty.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7507936507936509%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 2), (2, 3)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 5)], delete: [3]}',*

 * * "'dependencies'": "{insert: [(1, 'typing'), (2, 'typing_extensions')], delete: [4, 1]}",*

 * * "'hash'": "'93eadd2f4010b8e595f7f4af4efc698bd6d7a8fe571bfad7e90078f8fdaf26f8'",*

 * * "'id'": "'tty'",*

 * * "'interface_hash'": "'a9d1399e812eae7c01ab1ab2863f3d2eac3ae027bcc24c004a75d36506742307'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typesh […]*

```diff
@@ -1,35 +1,35 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        7,
-        1,
+        2,
+        3,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
         5,
-        30,
+        5,
         30
     ],
     "dependencies": [
         "sys",
-        "posixpath",
+        "typing",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433",
-    "id": "os.path",
+    "hash": "93eadd2f4010b8e595f7f4af4efc698bd6d7a8fe571bfad7e90078f8fdaf26f8",
+    "id": "tty",
     "ignore_all": true,
-    "interface_hash": "a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e",
-    "mtime": 1685143295,
+    "interface_hash": "a9d1399e812eae7c01ab1ab2863f3d2eac3ae027bcc24c004a75d36506742307",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/path.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/tty.pyi",
     "plugin_data": null,
-    "size": 186,
+    "size": 430,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/__main__.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/__main__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/__main__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/__main__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_cell_widths.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_cell_widths.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_cell_widths.meta.json` & `su6-0.3.0/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7422222222222222%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 2), (2, 3)]}',*

 * * "'dep_prios'": '{insert: [(1, 5), (2, 5), (3, 5)], delete: [1]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'email.message'), (2, 'typing')], "*

 * *                   'delete: [2]}',*

 * * "'hash'": "'53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf'",*

 * * "'id'": "'email.contentmanager'",*

 * * "'interface_hash'": "'86a7db72494c58ed2d0e5e9f95b2906da6e78e83aa31e5d85859dcbc0d594fad'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/s […]*

```diff
@@ -1,29 +1,35 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
+        2,
+        3,
         1,
         1
     ],
     "dep_prios": [
         5,
-        30,
+        5,
+        5,
+        5,
         30
     ],
     "dependencies": [
+        "collections.abc",
+        "email.message",
+        "typing",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "da7e048898b75fdb2a22ad0ed7a91467fcf2e9460c777c457c286529f9d6d477",
-    "id": "rich._cell_widths",
+    "hash": "53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf",
+    "id": "email.contentmanager",
     "ignore_all": true,
-    "interface_hash": "51626b8163420906cde6caed792b590188b485e282bfdfe06cf073271dd588bd",
-    "mtime": 1685143296,
+    "interface_hash": "86a7db72494c58ed2d0e5e9f95b2906da6e78e83aa31e5d85859dcbc0d594fad",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_cell_widths.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi",
     "plugin_data": null,
-    "size": 10096,
+    "size": 480,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_emoji_codes.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_emoji_codes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/rule.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.716421568627451%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 3), (1, 4), (2, 5), (3, 6), (4, 7), (5, 8), (6, 9), (7, 1), (8, '*

 * *                '118), (9, 1), (10, 1), (11, 1), (12, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (3, 5), (4, 5), (5, 5), (6, 5), (7, 5), (8, '*

 * *                '10), (10, 30), (11, 30), (12, 30), (13, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.align'), (1, 'rich.cells'), (2, 'rich.console'), (3, "*

 * *                   "'rich.jupyter'), (4, 'rich.measure'), (5, 'ric […]*

```diff
@@ -1,28 +1,67 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
+        3,
+        4,
+        5,
+        6,
+        7,
+        8,
+        9,
+        1,
+        118,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        10,
+        5,
+        30,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
+        "rich.align",
+        "rich.cells",
+        "rich.console",
+        "rich.jupyter",
+        "rich.measure",
+        "rich.style",
+        "rich.text",
+        "typing",
+        "sys",
         "builtins",
+        "_random",
+        "_typeshed",
         "abc",
-        "typing"
+        "datetime",
+        "rich.theme",
+        "typing_extensions"
     ],
-    "hash": "86ed552fd9db55da6926b5688a356c85195c4517bfbf7763bb7326776b0a65d6",
-    "id": "rich._emoji_codes",
+    "hash": "ba63b6d568f0d0571801e4c1dd4ba634b0ac0d685e8f3c678e57f65708978832",
+    "id": "rich.rule",
     "ignore_all": true,
-    "interface_hash": "3349b076d76c590dd6f9a7ca1c913093d5f7d0c64dc7590e5659121cc9b78246",
+    "interface_hash": "35c6e9d7e3cd1070eb6cf4dbfe676c2123dfa129f9a37351b5d011b3d539375e",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -57,13 +96,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_emoji_codes.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/rule.py",
     "plugin_data": null,
-    "size": 140235,
+    "size": 4590,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_emoji_replace.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_emoji_replace.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_export_format.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_export_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_export_format.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_pick.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'dep_prios'": '{insert: [(1, 5)], delete: [1]}',*

 * * "'dependencies'": "{insert: [(0, 'typing')], delete: [2]}",*

 * * "'hash'": "'7af0edf10378945e428b0ad421794e2429ed8ad0423ac23764b3c42005512c95'",*

 * * "'id'": "'rich._pick'",*

 * * "'interface_hash'": "'7ed533f4c2eb0d9103914acc943fb3899fa2de180f5ec37b574cb6e42193e52c'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_pick.py'",*

 * * "'size'": '423'}*

```diff
@@ -3,26 +3,26 @@
     "dep_lines": [
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        30,
+        5,
         30
     ],
     "dependencies": [
+        "typing",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "ab1815de72a75d0bb585f6e7455b303d8cbe030220d57d0b482e3b70ae6cf239",
-    "id": "rich._export_format",
+    "hash": "7af0edf10378945e428b0ad421794e2429ed8ad0423ac23764b3c42005512c95",
+    "id": "rich._pick",
     "ignore_all": true,
-    "interface_hash": "fd571c31ad724d67686183b09d73659e24b116ab584d9801c76ba413fab9f8e8",
+    "interface_hash": "7ed533f4c2eb0d9103914acc943fb3899fa2de180f5ec37b574cb6e42193e52c",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -57,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_export_format.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_pick.py",
     "plugin_data": null,
-    "size": 2100,
+    "size": 423,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_extension.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_extension.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_extension.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_extension.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_fileno.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_fileno.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_fileno.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_fileno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_inspect.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_inspect.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/measure.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.768073593073593%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 4), (1, 5), (4, 2), (5, 4), (6, 1)], delete: [10, 9, 7, 6, 5, 4, 3, '*

 * *                '2, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (2, 25), (5, 20), (7, 30)], delete: [7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.errors'), (1, 'rich.protocol'), (3, 'operator'), (5, "*

 * *                   "'rich'), (7, '_operator'), (10, 'rich.jupyter'), (12, 'rich.text')], delete: "*

 * *                   '[16, 14, 9, 8, 7, 6, 5, 4, 3, 2, 1]}',*

 * * "'hash'": "'1e6ac8257f2c5914c76 […]*

```diff
@@ -1,70 +1,58 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        7,
+        4,
+        5,
         8,
-        9,
-        10,
-        11,
-        12,
-        13,
-        14,
         1,
-        3,
-        5,
+        2,
+        4,
+        1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
+        10,
         5,
+        25,
         5,
         5,
+        20,
         5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
+        30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
+        "rich.errors",
+        "rich.protocol",
         "rich.console",
-        "rich.control",
-        "rich.highlighter",
-        "rich.jupyter",
-        "rich.panel",
-        "rich.pretty",
-        "rich.table",
-        "rich.text",
-        "__future__",
-        "inspect",
+        "operator",
         "typing",
+        "rich",
         "builtins",
+        "_operator",
         "_typeshed",
         "abc",
-        "rich.box",
+        "rich.jupyter",
         "rich.style",
-        "typing_extensions"
+        "rich.text"
     ],
-    "hash": "a19246c37d5eeb87705d20a6ac39ef65bc156f564a8567d4f30237556a218c99",
-    "id": "rich._inspect",
+    "hash": "1e6ac8257f2c5914c76e087c33111acbff37564a8d5bfef4b3c68a3f965c608f",
+    "id": "rich.measure",
     "ignore_all": true,
-    "interface_hash": "3ab38dffbfb27fbb716054e011e7e9ca7cde6de73b3aa2110ef99a619c30aa14",
+    "interface_hash": "6ea4bfc92f62e00d1612d117cb16c66c0dddb1a8a1ebd33547c16ff964d9cf8a",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -99,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_inspect.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/measure.py",
     "plugin_data": null,
-    "size": 9695,
+    "size": 5305,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_log_render.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_log_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_log_render.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_log_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_loop.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_loop.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_loop.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/protocol.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 5), (2, 2)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 20), (3, 5)], delete: [2]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.console'), (2, 'inspect')], delete: [2]}",*

 * * "'hash'": "'5adfb61d977aece622a295240933b3ee5337f2fca8e6bdc711067d4ce3c39794'",*

 * * "'id'": "'rich.protocol'",*

 * * "'interface_hash'": "'dbc101d777ba6400d696ff7983fabed24a37029e0c5fe0e95847065368b141b2'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packag […]*

```diff
@@ -1,31 +1,34 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
+        5,
         1,
-        1,
+        2,
         1,
         1
     ],
     "dep_prios": [
+        20,
+        5,
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
+        "rich.console",
         "typing",
+        "inspect",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "855ffa08b7683e6d2f6b6d96a70e332aa334458b33dd36715e3d0fa12fbd7834",
-    "id": "rich._loop",
+    "hash": "5adfb61d977aece622a295240933b3ee5337f2fca8e6bdc711067d4ce3c39794",
+    "id": "rich.protocol",
     "ignore_all": true,
-    "interface_hash": "b76fc611635bcba78ac86d56ecdf76df5d52e4165957022fabc6fe38e4bba5bf",
+    "interface_hash": "dbc101d777ba6400d696ff7983fabed24a37029e0c5fe0e95847065368b141b2",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -60,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_loop.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/protocol.py",
     "plugin_data": null,
-    "size": 1236,
+    "size": 1367,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_null_file.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_null_file.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_null_file.meta.json` & `su6-0.3.0/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7511111111111111%*

 * *Differences: {"'dep_lines'": '{delete: [1, 0]}',*

 * * "'dep_prios'": '{delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(2, 'typing')], delete: [3, 1, 0]}",*

 * * "'hash'": "'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'",*

 * * "'id'": "'urllib'",*

 * * "'interface_hash'": "'697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi'",*

 * * "'size'": '0'}*

```diff
@@ -1,35 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        2,
-        1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "types",
-        "typing",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "b4649793fbfe21999b8f5180cc78adf00de460840c882a55b0215fb02fbf289e",
-    "id": "rich._null_file",
+    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
+    "id": "urllib",
     "ignore_all": true,
-    "interface_hash": "879597e4b2f8671f49bd21f5497de7289f9fb377c45b9bd8140b4301219ab3ab",
-    "mtime": 1685143296,
+    "interface_hash": "697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_null_file.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi",
     "plugin_data": null,
-    "size": 1387,
+    "size": 0,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_palettes.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_palettes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_palettes.meta.json` & `su6-0.3.0/.mypy_cache/3.11/datetime.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6990740740740741%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(1, 2), (2, 3), (3, 4), (4, 5)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (3, 5), (4, 5), (5, 5)], delete: [2]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (2, 'time'), (4, 'typing_extensions'), (5, 'builtins'), "*

 * *                   "(6, '_typeshed')], delete: [1, 0]}",*

 * * "'hash'": "'0c60f43831b1f7d0abcfb453bf4fcc2d42dc7a37ad8ffe0d7344f047a6ecb87e'",*

 * * "'id'": "'datetime'",*

 * * "'interface_hash'": "'528f62badeb1a9d3c4aa6851fbf55bccea9c5a718ce08b […]*

```diff
@@ -1,32 +1,41 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        1,
+        2,
+        3,
+        4,
+        5,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
+        5,
+        5,
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
-        "rich.palette",
-        "builtins",
+        "sys",
         "abc",
-        "typing"
+        "time",
+        "typing",
+        "typing_extensions",
+        "builtins",
+        "_typeshed"
     ],
-    "hash": "71d7afd4940a67426f960b95f62a478339d3767be52335050c16f422dd8fce32",
-    "id": "rich._palettes",
+    "hash": "0c60f43831b1f7d0abcfb453bf4fcc2d42dc7a37ad8ffe0d7344f047a6ecb87e",
+    "id": "datetime",
     "ignore_all": true,
-    "interface_hash": "a9a7e508b3c4f8a548b09a97bc8e59ccb7d1c8d4c6301a06adc2593a7b4b12de",
-    "mtime": 1685143296,
+    "interface_hash": "528f62badeb1a9d3c4aa6851fbf55bccea9c5a718ce08b5cd4d3cf20efd41ffd",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_palettes.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/datetime.pyi",
     "plugin_data": null,
-    "size": 7063,
+    "size": 11534,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_pick.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_pick.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_pick.meta.json` & `su6-0.3.0/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7375%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 3), (2, 2), (3, 4)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (3, 'typing_extensions'), (4, "*

 * *                   "'builtins'), (5, 'typing')], delete: [1, 0]}",*

 * * "'hash'": "'5eafef06c53dd8b7d5ef6d7ece9ac1448f3f153c6061af7e9701fdf92f9e307c'",*

 * * "'id'": "'webbrowser'",*

 * * "'interface_hash'": "'713ac81ceecef86d02bf81125c771c8657aa61761f3ce7d997ad5d0eb8f736ca'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/h […]*

```diff
@@ -1,29 +1,38 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        3,
         1,
+        2,
+        4,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
         5,
         30
     ],
     "dependencies": [
-        "typing",
+        "collections.abc",
+        "sys",
+        "abc",
+        "typing_extensions",
         "builtins",
-        "abc"
+        "typing"
     ],
-    "hash": "7af0edf10378945e428b0ad421794e2429ed8ad0423ac23764b3c42005512c95",
-    "id": "rich._pick",
+    "hash": "5eafef06c53dd8b7d5ef6d7ece9ac1448f3f153c6061af7e9701fdf92f9e307c",
+    "id": "webbrowser",
     "ignore_all": true,
-    "interface_hash": "7ed533f4c2eb0d9103914acc943fb3899fa2de180f5ec37b574cb6e42193e52c",
-    "mtime": 1685143296,
+    "interface_hash": "713ac81ceecef86d02bf81125c771c8657aa61761f3ce7d997ad5d0eb8f736ca",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_pick.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/webbrowser.pyi",
     "plugin_data": null,
-    "size": 423,
+    "size": 2527,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_ratio.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_ratio.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_ratio.meta.json` & `su6-0.3.0/.mypy_cache/3.11/subprocess.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7215384615384616%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 3), (4, 5), (5, 6), (6, 1)], delete: [4, 2]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (7, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (2, '_typeshed'), (3, 'types'), (5, "*

 * *                   "'typing_extensions'), (8, 'array'), (9, 'ctypes'), (10, 'mmap'), (11, 'os'), "*

 * *                   "(12, 'pickle')], delete: [10, 9, 7, 6, 4, 2, 1]}",*

 * * "'hash'": "'d4ba0d25f732153c8003c650e12155f803326ed0fac4281b27d871f56a50cd34'",*

 * * "'id'": "'su […]*

```diff
@@ -1,53 +1,59 @@
 {
-    "data_mtime": 1685143684,
+    "data_mtime": 1685143683,
     "dep_lines": [
+        3,
         1,
         2,
-        3,
         4,
-        150,
+        5,
+        6,
+        1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
         10,
         5,
         5,
         5,
         5,
         5,
         30,
         30,
         30,
         30,
+        30,
         30
     ],
     "dependencies": [
+        "collections.abc",
         "sys",
-        "fractions",
-        "math",
+        "_typeshed",
+        "types",
         "typing",
-        "dataclasses",
+        "typing_extensions",
         "builtins",
-        "_decimal",
-        "_typeshed",
         "abc",
-        "numbers",
-        "typing_extensions"
+        "array",
+        "ctypes",
+        "mmap",
+        "os",
+        "pickle"
     ],
-    "hash": "e9d047c62c3f49835145d719f600ca2391a701e1d9f16be64e072d36972eb665",
-    "id": "rich._ratio",
+    "hash": "d4ba0d25f732153c8003c650e12155f803326ed0fac4281b27d871f56a50cd34",
+    "id": "subprocess",
     "ignore_all": true,
-    "interface_hash": "382f661f12b18379bc061ff96638f37c925dc21430a12725701db59da6db2d38",
-    "mtime": 1685143296,
+    "interface_hash": "5ae7ed6dca59aec33fec130abf5d53e13e5ac14c1cf73804d5046aaf8303bc28",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -81,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_ratio.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/subprocess.pyi",
     "plugin_data": null,
-    "size": 5460,
+    "size": 91091,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_spinners.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_spinners.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_spinners.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/theme.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7187301587301588%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 4), (1, 5), (2, 1), (3, 2), (4, 1), (5, 1), (6, 1), (7, 1), (8, 1), '*

 * *                '(9, 1), (10, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 10), (3, 5), (5, 30), (6, 30), (7, 30), (8, 30), '*

 * *                '(9, 30), (10, 30), (11, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.default_styles'), (1, 'rich.style'), (2, 'configparser'), "*

 * *                   "(3, 'typing'), (5, '_collections_abc'), (6, '_typeshed'), (8, 'enum'), (9, " […]*

```diff
@@ -1,28 +1,61 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
+        4,
+        5,
+        1,
+        2,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        10,
+        5,
+        5,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
+        "rich.default_styles",
+        "rich.style",
+        "configparser",
+        "typing",
         "builtins",
+        "_collections_abc",
+        "_typeshed",
         "abc",
-        "typing"
+        "enum",
+        "functools",
+        "io",
+        "rich.color",
+        "rich.color_triplet",
+        "typing_extensions"
     ],
-    "hash": "536af5fe0ff5cd28ec8e251d00449cda200c7378b8ae2fd2f0f60fea4439cf52",
-    "id": "rich._spinners",
+    "hash": "6de9452688330345b41f2b1069b29a1ce7374561f6928ddf400261a0df8015da",
+    "id": "rich.theme",
     "ignore_all": true,
-    "interface_hash": "f558f1ab7e7f9f21e444f7e168b8db6631e82ff78cd9044f5868b920441ad001",
+    "interface_hash": "60a22d4634a36c6a61e216557b933a97f163c0457d5c5980cd1a347ce29e181d",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -57,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_spinners.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/theme.py",
     "plugin_data": null,
-    "size": 19919,
+    "size": 3777,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_stack.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_stack.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_stack.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_stack.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_timer.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_timer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_timer.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/file_proxy.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7388034188034188%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 4), (1, 5), (3, 1), (4, 2), (5, 1), (6, 1)], delete: [2, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (2, 25), (6, 30), (7, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.ansi'), (1, 'rich.text'), (2, 'rich.console'), (3, 'io'), "*

 * *                   "(7, 'rich.jupyter'), (8, 'rich.style'), (9, 'typing_extensions')], delete: [4, "*

 * *                   '1, 0]}',*

 * * "'hash'": "'4e5f531cc0d9f8f9395a6f2c23580683f5390e1bac9b10fe159d1f51b714d16d'",*

 * * "'id'": "' […]*

```diff
@@ -1,37 +1,49 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        6,
+        4,
+        5,
         8,
-        9,
+        1,
+        2,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        25,
         10,
         5,
         5,
         30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "time",
-        "contextlib",
+        "rich.ansi",
+        "rich.text",
+        "rich.console",
+        "io",
         "typing",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "rich.jupyter",
+        "rich.style",
+        "typing_extensions"
     ],
-    "hash": "cde9716d3ea83c566736bc163e973592d51e013f957387ee15c4592d018bb4c2",
-    "id": "rich._timer",
+    "hash": "4e5f531cc0d9f8f9395a6f2c23580683f5390e1bac9b10fe159d1f51b714d16d",
+    "id": "rich.file_proxy",
     "ignore_all": true,
-    "interface_hash": "bfdd6c20b7ecfcd57c73148117aefe0872f821c646cd5582579b33fad184e569",
+    "interface_hash": "f154d096b0d4d06ddd96567900fd9594349cf99bea8c7c56e33232e05f44ef31",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -66,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_timer.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/file_proxy.py",
     "plugin_data": null,
-    "size": 417,
+    "size": 1683,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_win32_console.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_win32_console.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_win32_console.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/emoji.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7837979797979798%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 4), (4, 8), (5, 17), (6, 84), (7, 1), (8, 2), (9, 1)], delete: [7, '*

 * *                '3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 5), (5, 5), (8, 5), (10, 30)], delete: [5, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.jupyter'), (1, 'rich.segment'), (3, 'rich._emoji_codes'), "*

 * *                   "(4, 'rich._emoji_replace'), (6, 'rich.columns'), (10, '_collections_abc'), "*

 * *                   "(11, '_random'), (14, 'datetime'), (16, 're'), (17, 'rich.terminal_theme'), "*

 * *      […]*

```diff
@@ -1,73 +1,79 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        16,
-        19,
-        20,
-        579,
+        4,
         5,
         6,
         7,
-        15,
+        8,
+        17,
+        84,
+        1,
+        2,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
         5,
         5,
         5,
         5,
-        10,
+        5,
+        5,
         5,
         10,
         5,
+        5,
+        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "ctypes.wintypes",
-        "rich.color",
+        "rich.jupyter",
+        "rich.segment",
         "rich.style",
+        "rich._emoji_codes",
+        "rich._emoji_replace",
         "rich.console",
-        "ctypes",
+        "rich.columns",
         "sys",
         "typing",
-        "time",
         "builtins",
+        "_collections_abc",
+        "_random",
         "_typeshed",
         "abc",
-        "array",
+        "datetime",
         "enum",
-        "functools",
-        "mmap",
-        "pickle",
-        "rich.color_triplet",
-        "typing_extensions"
+        "re",
+        "rich.terminal_theme",
+        "rich.text",
+        "rich.theme"
     ],
-    "hash": "f8db5e6a5b105d0e79f1efb3a49b64c21f31fdda82f928e500603cef674613a5",
-    "id": "rich._win32_console",
+    "hash": "d634d11c5c2f431635722ba5db631d11971673b6eb7e3293f051ba6635e3e5d3",
+    "id": "rich.emoji",
     "ignore_all": true,
-    "interface_hash": "4f75d220b2446d31efd07881418ba81ada3c0c96c6cd26363ae6f0a214580e8e",
+    "interface_hash": "26d979ea4664b3bfc09b9cd4cfc8971144bb635aeba33014d6df6c82350a8fa1",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -102,13 +108,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_win32_console.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/emoji.py",
     "plugin_data": null,
-    "size": 22784,
+    "size": 2465,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_windows.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_windows.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_windows.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/params.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7328826728826728%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 5), (1, 8), (3, 3), (4, 1)], delete: [5, 4, 3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 25), (5, 30)], delete: [5, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'typer.models'), (1, 'click.shell_completion'), (2, 'typing'), "*

 * *                   "(3, 'click'), (6, 'click.core'), (7, 'click.types')], delete: [8, 5, 4, 3, 2, "*

 * *                   '1, 0]}',*

 * * "'hash'": "'fcf07893bfc8bf4aa53628a147a0b9383364d9146d16d97b31bf5d993a818c4c'",*

 * * "'id'": "'typer.params'",*

 * * "'interface_hash'": " […]*

```diff
@@ -1,47 +1,44 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        25,
+        5,
+        8,
+        1,
+        3,
         1,
-        2,
-        16,
-        66,
-        69,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
+        25,
         5,
         10,
         5,
-        5,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "rich._win32_console",
-        "sys",
-        "dataclasses",
-        "ctypes",
-        "platform",
-        "rich",
+        "typer.models",
+        "click.shell_completion",
+        "typing",
+        "click",
         "builtins",
         "abc",
-        "typing"
+        "click.core",
+        "click.types"
     ],
-    "hash": "27fae1687ec73377f95ef1f96ec02b18aaa84e88da57c1deb4d2d4275497f48e",
-    "id": "rich._windows",
+    "hash": "fcf07893bfc8bf4aa53628a147a0b9383364d9146d16d97b31bf5d993a818c4c",
+    "id": "typer.params",
     "ignore_all": true,
-    "interface_hash": "974e41661a343e129a1f46290e766656bdf10299e6f66d27c26a6d0da8c1cabf",
-    "mtime": 1685143296,
+    "interface_hash": "e8e28933e640b7a78446e418ed017d302c5b8ec515ab27ca1c0cc9c2eac83b45",
+    "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -75,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/_windows.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/params.py",
     "plugin_data": null,
-    "size": 1902,
+    "size": 13401,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_windows_renderer.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_windows_renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_wrap.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_wrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/_wrap.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/_wrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/abc.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/abc.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/align.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/align.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/align.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/align.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/ansi.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/ansi.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/ansi.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/box.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/box.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/box.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/box.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/cells.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/cells.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/cells.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/color_triplet.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7708333333333334%*

 * *Differences: {"'dep_lines'": '{delete: [4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [6, 5, 2, 1, 0]}',*

 * * "'dependencies'": '{delete: [7, 5, 2, 1, 0]}',*

 * * "'hash'": "'de585091d25bbd63e82c33be0276089805a626f579765818342559f7b39168de'",*

 * * "'id'": "'rich.color_triplet'",*

 * * "'interface_hash'": "'cd387d4245c3d37b323f42a80c63ddcd6517d832a6903654fd780b0cb389cd8b'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/color_triplet.py'",*

 * * "'size'": '1054'}*

```diff
@@ -1,43 +1,28 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        5,
-        1,
-        2,
-        3,
-        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
         5,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "rich._cell_widths",
-        "re",
-        "functools",
         "typing",
         "builtins",
-        "_typeshed",
-        "abc",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "eb6ef3b49b3dcce2fedfc1c9ee45c17ab47e813f0a05f602f14cc4c0c243618a",
-    "id": "rich.cells",
+    "hash": "de585091d25bbd63e82c33be0276089805a626f579765818342559f7b39168de",
+    "id": "rich.color_triplet",
     "ignore_all": true,
-    "interface_hash": "172e16952ab394c6ff692362a0d695ea8e0835948ad5846a9a454987745962e0",
+    "interface_hash": "cd387d4245c3d37b323f42a80c63ddcd6517d832a6903654fd780b0cb389cd8b",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/cells.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/color_triplet.py",
     "plugin_data": null,
-    "size": 4509,
+    "size": 1054,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/color.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/color.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/color.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/color.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/color_triplet.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/color_triplet.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/color_triplet.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/terminal_theme.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.76%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 3), (1, 4)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.color_triplet'), (1, 'rich.palette')]}",*

 * * "'hash'": "'d63e7eb9f25f9ef940a3942c8bf0026625c39b0317cea826141c8e6d3f7ec896'",*

 * * "'id'": "'rich.terminal_theme'",*

 * * "'interface_hash'": "'cb0f63719435d76dbd314726350fc38ea160216dd2a40c3c64077245141adf2e'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/terminal_theme. […]*

```diff
@@ -1,28 +1,34 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685143685,
     "dep_lines": [
+        3,
+        4,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        5,
+        5,
         30
     ],
     "dependencies": [
+        "rich.color_triplet",
+        "rich.palette",
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "de585091d25bbd63e82c33be0276089805a626f579765818342559f7b39168de",
-    "id": "rich.color_triplet",
+    "hash": "d63e7eb9f25f9ef940a3942c8bf0026625c39b0317cea826141c8e6d3f7ec896",
+    "id": "rich.terminal_theme",
     "ignore_all": true,
-    "interface_hash": "cd387d4245c3d37b323f42a80c63ddcd6517d832a6903654fd780b0cb389cd8b",
+    "interface_hash": "cb0f63719435d76dbd314726350fc38ea160216dd2a40c3c64077245141adf2e",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -57,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/color_triplet.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/terminal_theme.py",
     "plugin_data": null,
-    "size": 1054,
+    "size": 3370,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/columns.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/columns.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/columns.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/columns.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/console.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/console.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/console.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/constrain.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/constrain.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/constrain.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/constrain.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/containers.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/containers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/containers.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/containers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/control.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/control.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/control.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/control.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/default_styles.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/default_styles.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/default_styles.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/default_styles.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/emoji.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/emoji.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/emoji.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/styled.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7775403726708076%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 3), (4, 39), (6, 38)], delete: [12, 11, 10, 9, 8, 7, 6, 5, 3, 2]}',*

 * * "'dep_prios'": '{insert: [(3, 25)], delete: [14, 13, 12, 11, 10, 7, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.measure'), (4, 'rich.panel'), (6, 'rich'), (10, "*

 * *                   "'rich.box'), (11, 'rich.jupyter')], delete: [19, 17, 16, 14, 12, 11, 10, 7, 6, "*

 * *                   '4, 3, 0]}',*

 * * "'hash'": "'c258d5b154d76c004c319be4ce43b8dd9124ffe8abcc4b6f52243eb0d9e2910f'",*

 * * "'id'": "'rich.styled'",*

 * * "'in […]*

```diff
@@ -1,79 +1,58 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
+        3,
         4,
         5,
-        6,
-        7,
         8,
-        17,
-        84,
-        1,
-        2,
-        1,
-        1,
-        1,
-        1,
+        39,
         1,
+        38,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
+        25,
         5,
         5,
         5,
         5,
-        10,
-        5,
-        5,
-        30,
-        30,
-        30,
-        30,
-        30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "rich.jupyter",
+        "rich.measure",
         "rich.segment",
         "rich.style",
-        "rich._emoji_codes",
-        "rich._emoji_replace",
         "rich.console",
-        "rich.columns",
-        "sys",
+        "rich.panel",
         "typing",
+        "rich",
         "builtins",
-        "_collections_abc",
-        "_random",
-        "_typeshed",
         "abc",
-        "datetime",
         "enum",
-        "re",
-        "rich.terminal_theme",
-        "rich.text",
-        "rich.theme"
+        "rich.box",
+        "rich.jupyter",
+        "rich.text"
     ],
-    "hash": "d634d11c5c2f431635722ba5db631d11971673b6eb7e3293f051ba6635e3e5d3",
-    "id": "rich.emoji",
+    "hash": "c258d5b154d76c004c319be4ce43b8dd9124ffe8abcc4b6f52243eb0d9e2910f",
+    "id": "rich.styled",
     "ignore_all": true,
-    "interface_hash": "26d979ea4664b3bfc09b9cd4cfc8971144bb635aeba33014d6df6c82350a8fa1",
+    "interface_hash": "e950fe9af602055d5bd175e8aebc26b5ab0ed48f01495bd939716430abbacac8",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -108,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/emoji.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/styled.py",
     "plugin_data": null,
-    "size": 2465,
+    "size": 1234,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/errors.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/errors.meta.json` & `su6-0.3.0/.mypy_cache/3.11/numbers.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.73%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 4), (1, 5)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 5), (2, 5)], delete: [2, 1]}',*

 * * "'dependencies'": "{insert: [(2, 'builtins')], delete: [0]}",*

 * * "'hash'": "'aa29ea52bc87c75f589211fa38294e2cc1bc735c97f4fa331ebaff28e5f2cb84'",*

 * * "'id'": "'numbers'",*

 * * "'interface_hash'": "'73479f60f40dd74ecc1b17ddb3686ec0848505c1e59ff61c46c3c55a1919cf16'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/nu […]*

```diff
@@ -1,29 +1,29 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        1,
-        1,
+        4,
+        5,
         1
     ],
     "dep_prios": [
         5,
-        30,
-        30
+        5,
+        5
     ],
     "dependencies": [
-        "builtins",
         "abc",
-        "typing"
+        "typing",
+        "builtins"
     ],
-    "hash": "e693f729ce5de1027f734285b31adfca18e23d57bb275ccea9215b140cdc57e6",
-    "id": "rich.errors",
+    "hash": "aa29ea52bc87c75f589211fa38294e2cc1bc735c97f4fa331ebaff28e5f2cb84",
+    "id": "numbers",
     "ignore_all": true,
-    "interface_hash": "534ee3082dbc4ad481e7299060952717c174935b937136d76df876eaf8407f10",
-    "mtime": 1685143296,
+    "interface_hash": "73479f60f40dd74ecc1b17ddb3686ec0848505c1e59ff61c46c3c55a1919cf16",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/errors.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/numbers.pyi",
     "plugin_data": null,
-    "size": 642,
+    "size": 3914,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/file_proxy.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/file_proxy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/file_proxy.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/style.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7698321891685735%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 7), (2, 9), (3, 10), (6, 3), (7, 4), (8, 5), (9, 7), (10, 1), (11, '*

 * *                '1)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (3, 5), (5, 5), (6, 5), (7, 5), (9, 20), (11, 30), (12, 30)], '*

 * *                'delete: [2]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.errors'), (1, 'rich.color'), (2, 'rich.repr'), (3, "*

 * *                   "'rich.terminal_theme'), (4, 'sys'), (5, 'functools'), (6, 'marshal'), (7, "*

 * *                   "'random'), (9, 'rich'), (11, '_ […]*

```diff
@@ -1,49 +1,70 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        4,
-        5,
+        7,
         8,
+        9,
+        10,
         1,
         2,
+        3,
+        4,
+        5,
+        7,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
         5,
         5,
-        25,
         10,
         5,
         5,
+        5,
+        5,
+        20,
+        5,
+        30,
+        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "rich.ansi",
-        "rich.text",
-        "rich.console",
-        "io",
+        "rich.errors",
+        "rich.color",
+        "rich.repr",
+        "rich.terminal_theme",
+        "sys",
+        "functools",
+        "marshal",
+        "random",
         "typing",
+        "rich",
         "builtins",
+        "_collections_abc",
+        "_typeshed",
         "abc",
-        "rich.jupyter",
-        "rich.style",
+        "enum",
+        "rich.color_triplet",
         "typing_extensions"
     ],
-    "hash": "4e5f531cc0d9f8f9395a6f2c23580683f5390e1bac9b10fe159d1f51b714d16d",
-    "id": "rich.file_proxy",
+    "hash": "de18a8707ff837cbf0466dfef32156ccceed4b08e312f7a7ebd5ea59ab124303",
+    "id": "rich.style",
     "ignore_all": true,
-    "interface_hash": "f154d096b0d4d06ddd96567900fd9594349cf99bea8c7c56e33232e05f44ef31",
+    "interface_hash": "c7e1e2ffb01b0740660c610c2734c5fe7cfe558f111403728cc12f3470cf5fbe",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -78,13 +99,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/file_proxy.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/style.py",
     "plugin_data": null,
-    "size": 1683,
+    "size": 27073,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/highlighter.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/highlighter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/highlighter.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/repr.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7898929308565531%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 133), (4, 1), (5, 1), (6, 1)], delete: [5, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 30), (6, 30), (7, 30)], delete: [5, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'inspect'), (2, 'functools'), (6, 'abc'), (8, 'enum'), (11, "*

 * *                   "'rich.text'), (13, 'types')], delete: [9, 5, 3, 2, 0]}",*

 * * "'hash'": "'76093a20c29892c683ce82766bacb1b5d699780c27e5e6651b8152054f1b7b7b'",*

 * * "'id'": "'rich.repr'",*

 * * "'interface_hash'": "'b907c5f6f586d02574e93dd3e53daefb27eb0668c4731ca2ebaae3a […]*

```diff
@@ -1,58 +1,61 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        5,
-        202,
+        133,
         1,
         2,
         3,
-        230,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
         10,
         5,
         5,
-        10,
         5,
         30,
         30,
         30,
         30,
         30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "rich.text",
         "rich.console",
-        "re",
-        "abc",
+        "inspect",
+        "functools",
         "typing",
-        "json",
         "builtins",
         "_random",
+        "abc",
         "datetime",
-        "json.encoder",
+        "enum",
         "rich.jupyter",
         "rich.style",
-        "rich.theme"
+        "rich.text",
+        "rich.theme",
+        "types"
     ],
-    "hash": "a770b5838418cdecc529d47b345f4484f6f3403bdd3d48464604b21861263e4a",
-    "id": "rich.highlighter",
+    "hash": "76093a20c29892c683ce82766bacb1b5d699780c27e5e6651b8152054f1b7b7b",
+    "id": "rich.repr",
     "ignore_all": true,
-    "interface_hash": "9f1264bb283838e4d5e234aea219b1e866711ec3938d007140d0e914dd5f52b3",
+    "interface_hash": "b907c5f6f586d02574e93dd3e53daefb27eb0668c4731ca2ebaae3a6429c0f69",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -87,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/highlighter.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/repr.py",
     "plugin_data": null,
-    "size": 9584,
+    "size": 4419,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/json.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/json.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/json.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/json.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/jupyter.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/jupyter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/jupyter.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/jupyter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/live.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/live.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/live.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/live.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/live_render.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/live_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/live_render.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/live_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/markdown.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/markdown.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/markdown.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/markdown.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/markup.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/markup.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/markup.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/markup.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/measure.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/measure.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/measure.meta.json` & `su6-0.3.0/.mypy_cache/3.11/glob.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6967261904761906%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 3)], delete: [10, 9, 8, 7, 6, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10)], delete: [11, 10, 9, 8, 7, 5, 2, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, '_typeshed')], delete: [12, "*

 * *                   '11, 10, 8, 7, 5, 3, 2, 1, 0]}',*

 * * "'hash'": "'b23877cf7cc743ec86f6a87b449a4cc1a92ad72e573a19c7a17a82c3fc3507a2'",*

 * * "'id'": "'glob'",*

 * * "'interface_hash'": "'0b54d93d4031a2a78bad77ffdb5e562a1953657395d23eb1249760d4ef […]*

```diff
@@ -1,59 +1,38 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        4,
-        5,
-        8,
+        3,
         1,
         2,
         4,
         1,
-        1,
-        1,
-        1,
-        1,
-        1,
         1
     ],
     "dep_prios": [
-        10,
         5,
-        25,
+        10,
         5,
         5,
-        20,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "rich.errors",
-        "rich.protocol",
-        "rich.console",
-        "operator",
+        "collections.abc",
+        "sys",
+        "_typeshed",
         "typing",
-        "rich",
         "builtins",
-        "_operator",
-        "_typeshed",
-        "abc",
-        "rich.jupyter",
-        "rich.style",
-        "rich.text"
+        "abc"
     ],
-    "hash": "1e6ac8257f2c5914c76e087c33111acbff37564a8d5bfef4b3c68a3f965c608f",
-    "id": "rich.measure",
+    "hash": "b23877cf7cc743ec86f6a87b449a4cc1a92ad72e573a19c7a17a82c3fc3507a2",
+    "id": "glob",
     "ignore_all": true,
-    "interface_hash": "6ea4bfc92f62e00d1612d117cb16c66c0dddb1a8a1ebd33547c16ff964d9cf8a",
-    "mtime": 1685143296,
+    "interface_hash": "0b54d93d4031a2a78bad77ffdb5e562a1953657395d23eb1249760d4eff0837f",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -87,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/measure.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/glob.pyi",
     "plugin_data": null,
-    "size": 5305,
+    "size": 1421,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/padding.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/padding.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/padding.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/palette.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7776016873718024%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 5), (1, 8), (2, 21), (3, 22), (4, 23), (5, 79), (6, 80), (8, 2), '*

 * *                '(9, 3), (10, 76), (11, 1)], delete: [6, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 20), (2, 5), (4, 20), (10, 10), (12, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.color_triplet'), (1, 'rich.table'), (2, 'rich.color'), (4, "*

 * *                   "'rich.text'), (5, 'rich.console'), (7, 'math'), (8, 'functools'), (10, "*

 * *                   "'colorsys'), (12, '_random') […]*

```diff
@@ -1,67 +1,82 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        4,
-        10,
-        11,
-        12,
-        13,
+        5,
+        8,
+        21,
+        22,
+        23,
+        79,
+        80,
+        1,
+        2,
+        3,
+        76,
         1,
-        139,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        25,
+        5,
+        20,
         5,
         5,
+        20,
         5,
         5,
         5,
         5,
         5,
+        10,
+        5,
+        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "rich.console",
-        "rich.jupyter",
-        "rich.measure",
+        "rich.color_triplet",
+        "rich.table",
+        "rich.color",
         "rich.style",
+        "rich.text",
+        "rich.console",
         "rich.segment",
+        "math",
+        "functools",
         "typing",
-        "rich",
+        "colorsys",
         "builtins",
+        "_random",
         "_typeshed",
         "abc",
-        "array",
-        "ctypes",
+        "datetime",
         "enum",
-        "mmap",
-        "pickle",
+        "rich.box",
+        "rich.jupyter",
+        "rich.theme",
         "typing_extensions"
     ],
-    "hash": "f08d5d40d4102b58828c7b46043127efc911a77a76ec6633979511dea07b7b61",
-    "id": "rich.padding",
+    "hash": "02be9952b607885b7af91af693e93d17c57b87180960735daa3936bd55ec2e07",
+    "id": "rich.palette",
     "ignore_all": true,
-    "interface_hash": "bc537bd6ac0e6faddeca536a672e1b6bf709b52f24ab1303bcb5841a890d3cca",
+    "interface_hash": "82db41141470f5bc064033957838d7861436656101e31fe2f14051ff6dfd5e42",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -96,13 +111,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/padding.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/palette.py",
     "plugin_data": null,
-    "size": 4958,
+    "size": 3288,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/pager.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/pager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/pager.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/text.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7625534625534626%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 18), (1, 19), (2, 20), (3, 21), (4, 22), (5, 23), (6, 24), (7, 25), '*

 * *                '(8, 26), (9, 27), (10, 28), (12, 32), (13, 219), (14, 297), (17, 3), (18, 4), '*

 * *                '(19, 5), (20, 1), (21, 1), (22, 1), (23, 1), (24, 1), (25, 1)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (3, 5), (4, 5), (5, 5), (6, 5), (7, 5), (8, 5), '*

 * *                '(9, 5), (10, 5), (11, 5), (12, 5), (13, 20), (14, 20), (15, 10), (21, 30), (22, '*

 * *                '3 […]*

```diff
@@ -1,14 +1,36 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
+        18,
+        19,
+        20,
+        21,
+        22,
+        23,
+        24,
+        25,
+        26,
+        27,
+        28,
         29,
-        30,
+        32,
+        219,
+        297,
         1,
         2,
+        3,
+        4,
+        5,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
@@ -18,44 +40,88 @@
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
         5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        20,
+        20,
+        10,
+        5,
+        5,
+        5,
+        5,
+        5,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "rich.__main__",
+        "rich._loop",
+        "rich._pick",
+        "rich._wrap",
+        "rich.align",
+        "rich.cells",
+        "rich.containers",
+        "rich.control",
+        "rich.emoji",
+        "rich.jupyter",
+        "rich.measure",
+        "rich.segment",
+        "rich.style",
         "rich.console",
-        "abc",
+        "rich.markup",
+        "rich.ansi",
+        "re",
+        "functools",
+        "math",
+        "operator",
         "typing",
         "builtins",
+        "_collections_abc",
+        "_operator",
         "_random",
+        "_typeshed",
+        "abc",
+        "array",
+        "ctypes",
         "datetime",
-        "importlib",
-        "rich.jupyter",
-        "rich.style",
-        "rich.table",
-        "rich.text",
+        "enum",
+        "mmap",
+        "pickle",
+        "rich.color",
+        "rich.color_triplet",
         "rich.theme",
-        "types"
+        "typing_extensions"
     ],
-    "hash": "48efc44c114a6e0de7fc080ecd79b8d52bf7e98c57032237fd1f8a398dbfb927",
-    "id": "rich.pager",
+    "hash": "ab2364a4c8261f73ef9fca6336b60ca15f0c2d16e38b5c7e10e3f6a3a74433ad",
+    "id": "rich.text",
     "ignore_all": true,
-    "interface_hash": "459e2e84034139b55dbab928e42d39aeaa0e874ccc261e1c24a435dd20953020",
+    "interface_hash": "7dda9dbd02bd21fd9a4743298292110d1d478c433cff11c86d57acbc1b1f3914",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -90,13 +156,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/pager.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/text.py",
     "plugin_data": null,
-    "size": 828,
+    "size": 45513,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/palette.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/palette.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/palette.meta.json` & `su6-0.3.0/.mypy_cache/3.11/io.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6914583333333333%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 6), (4, 4), (5, 5), (6, 7), (7, 8), (8, 9), (9, 10)], delete: [16, '*

 * *                '15, 14, 13, 12, 11, 10, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (3, 10), (4, 10)], delete: [16, 15, 14, 13, 12, 10, '*

 * *                '4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'abc'), (3, 'codecs'), (4, 'sys'), (6, "*

 * *                   "'os'), (7, 'types'), (8, 'typing'), (10, 'array'), (11, 'ctypes […]*

```diff
@@ -1,83 +1,62 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        5,
-        8,
-        21,
-        22,
-        23,
-        79,
-        80,
+        6,
         1,
         2,
         3,
-        76,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
+        4,
+        5,
+        7,
+        8,
+        9,
+        10,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        20,
-        5,
-        5,
-        20,
-        5,
+        10,
+        10,
+        10,
+        10,
         5,
         5,
         5,
         5,
-        10,
         5,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "rich.color_triplet",
-        "rich.table",
-        "rich.color",
-        "rich.style",
-        "rich.text",
-        "rich.console",
-        "rich.segment",
-        "math",
-        "functools",
-        "typing",
-        "colorsys",
+        "collections.abc",
+        "abc",
         "builtins",
-        "_random",
+        "codecs",
+        "sys",
         "_typeshed",
-        "abc",
-        "datetime",
-        "enum",
-        "rich.box",
-        "rich.jupyter",
-        "rich.theme",
-        "typing_extensions"
+        "os",
+        "types",
+        "typing",
+        "typing_extensions",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "02be9952b607885b7af91af693e93d17c57b87180960735daa3936bd55ec2e07",
-    "id": "rich.palette",
+    "hash": "0b41ad24faa49ac20e0c8c0d0bf223ff7de8ce8ea44fe01e3a4a2cb1f363054d",
+    "id": "io",
     "ignore_all": true,
-    "interface_hash": "82db41141470f5bc064033957838d7861436656101e31fe2f14051ff6dfd5e42",
-    "mtime": 1685143296,
+    "interface_hash": "f9869284f2a5be1f4215bfc4c458a1220d04288cfd924c5156bc82dfd3c84906",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -111,13 +90,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/palette.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/io.pyi",
     "plugin_data": null,
-    "size": 3288,
+    "size": 7875,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/panel.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/panel.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/panel.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/panel.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/pretty.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/pretty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/pretty.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/pretty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/protocol.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/protocol.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/protocol.meta.json` & `su6-0.3.0/.mypy_cache/3.11/mmap.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6992424242424242%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 3), (3, 4), (4, 5), (5, 1), (6, 1), (7, 1)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5), (6, 30), (7, 30), (8, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, '_typeshed'), (4, "*

 * *                   "'typing_extensions'), (7, 'array'), (8, 'ctypes'), (9, 'pickle')], delete: [2, "*

 * *                   '0]}',*

 * * "'hash'": "'d9e78f0946bc6297002b245e9d85b5be1bcfe36b9a503843f57923c1574200ea' […]*

```diff
@@ -1,35 +1,50 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        5,
+        3,
         1,
         2,
+        4,
+        5,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
-        20,
+        5,
+        10,
+        5,
         5,
         5,
         5,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "rich.console",
+        "collections.abc",
+        "sys",
+        "_typeshed",
         "typing",
-        "inspect",
+        "typing_extensions",
         "builtins",
-        "abc"
+        "abc",
+        "array",
+        "ctypes",
+        "pickle"
     ],
-    "hash": "5adfb61d977aece622a295240933b3ee5337f2fca8e6bdc711067d4ce3c39794",
-    "id": "rich.protocol",
+    "hash": "d9e78f0946bc6297002b245e9d85b5be1bcfe36b9a503843f57923c1574200ea",
+    "id": "mmap",
     "ignore_all": true,
-    "interface_hash": "dbc101d777ba6400d696ff7983fabed24a37029e0c5fe0e95847065368b141b2",
-    "mtime": 1685143296,
+    "interface_hash": "4826eca11c6294e24662f5d0ea3aeb5050023b4d7584ca360d81eca7a5d7a39d",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/protocol.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/mmap.pyi",
     "plugin_data": null,
-    "size": 1367,
+    "size": 4009,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/region.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/region.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/region.meta.json` & `su6-0.3.0/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7428571428571428%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 1), (1, 2), (2, 3)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (4, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'importlib.abc'), (2, 'types'), (5, "*

 * *                   "'typing')], delete: [0]}",*

 * * "'hash'": "'93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914'",*

 * * "'id'": "'importlib'",*

 * * "'interface_hash'": "'5f92435a83c8d015c7f5083f731f4b7db32ae1cd81d45c2986fdcbc6fcba52a3'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su […]*

```diff
@@ -1,29 +1,38 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
+        2,
+        3,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        5,
+        5,
+        30,
         30
     ],
     "dependencies": [
-        "typing",
+        "collections.abc",
+        "importlib.abc",
+        "types",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "acd4fdc59ad56536085d90b43589f8d42250c1835b47e29e70f3b14e042f07c6",
-    "id": "rich.region",
+    "hash": "93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914",
+    "id": "importlib",
     "ignore_all": true,
-    "interface_hash": "3c4daa256da6ee49361e01123ed1955effa6af54d049e46091b27ae9104959b7",
-    "mtime": 1685143296,
+    "interface_hash": "5f92435a83c8d015c7f5083f731f4b7db32ae1cd81d45c2986fdcbc6fcba52a3",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/region.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi",
     "plugin_data": null,
-    "size": 166,
+    "size": 801,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/repr.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/repr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/repr.meta.json` & `su6-0.3.0/.mypy_cache/3.11/su6/cli.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6430406549971768%*

 * *Differences: {"'data_mtime'": '1685286348',*

 * * "'dep_lines'": '{insert: [(0, 10), (3, 5), (4, 8), (5, 1), (6, 1), (7, 1), (8, 1), (19, 7), (20, '*

 * *                '6)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 10), (3, 10), (6, 30), (7, 30), (8, 30), (9, 30), (19, 5), (20, '*

 * *                '5)], delete: [2]}',*

 * * "'dependencies'": "{insert: [(0, 'su6.core'), (3, 'typer'), (4, 'rich'), (6, '_typeshed'), (8, "*

 * *                   "'array'), (9, 'click'), (10, 'click.core'), (11, 'click.exceptions'), (12, "*

 * *             […]*

```diff
@@ -1,62 +1,81 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685286348,
     "dep_lines": [
-        133,
-        1,
+        10,
         2,
         3,
+        5,
+        8,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1
+        1,
+        1,
+        1,
+        7,
+        6
     ],
     "dep_prios": [
         5,
         10,
+        10,
+        10,
         5,
         5,
-        5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30
+        30,
+        30,
+        30,
+        30,
+        30,
+        5,
+        5
     ],
     "dependencies": [
-        "rich.console",
-        "inspect",
+        "su6.core",
         "functools",
         "typing",
+        "typer",
+        "rich",
         "builtins",
-        "_random",
+        "_typeshed",
         "abc",
-        "datetime",
+        "array",
+        "click",
+        "click.core",
+        "click.exceptions",
+        "ctypes",
         "enum",
-        "rich.jupyter",
-        "rich.style",
-        "rich.text",
-        "rich.theme",
-        "types"
+        "mmap",
+        "pickle",
+        "typer.core",
+        "typer.main",
+        "typing_extensions"
     ],
-    "hash": "76093a20c29892c683ce82766bacb1b5d699780c27e5e6651b8152054f1b7b7b",
-    "id": "rich.repr",
-    "ignore_all": true,
-    "interface_hash": "b907c5f6f586d02574e93dd3e53daefb27eb0668c4731ca2ebaae3a6429c0f69",
-    "mtime": 1685143296,
+    "hash": "49ba80b78234f87dbd2763809293d48d44671952d0c7442f010695a257d80481",
+    "id": "su6.cli",
+    "ignore_all": false,
+    "interface_hash": "88fc7def833a3b1546dd0b27abd8eb4607206612975f2047f340d42b31bd41de",
+    "mtime": 1685286338,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -90,13 +109,16 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/repr.py",
+    "path": "./src/su6/cli.py",
     "plugin_data": null,
-    "size": 4419,
-    "suppressed": [],
+    "size": 7100,
+    "suppressed": [
+        "plumbum.commands.processes",
+        "plumbum"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/rule.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/rule.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/rule.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/syntax.meta.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7344155844155844%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 1), (1, 40), (2, 41), (3, 43), (4, 44), (5, 45), (6, 46), (7, 47), '*

 * *                '(8, 48), (9, 49), (10, 50), (11, 51), (12, 1), (13, 2), (20, 832), (22, 1), (23, '*

 * *                '1), (24, 1), (25, 1), (26, 1), (27, 1), (28, 1), (36, 22), (37, 23), (38, 24), '*

 * *                '(39, 25), (40, 26), (41, 38)], delete: [8, 6]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5), (2, 5), (3, 5), (4, 5), (5, 5), (6, 5), (12, 20), (13, '*

 * *                '10), (14, 10), (15, 10), (16,  […]*

```diff
@@ -1,67 +1,139 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
+        1,
+        40,
+        41,
+        43,
+        44,
+        45,
+        46,
+        47,
+        48,
+        49,
+        50,
+        51,
+        1,
+        2,
         3,
         4,
         5,
         6,
         7,
         8,
-        9,
+        832,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
-        118,
         1,
         1,
         1,
         1,
         1,
         1,
-        1
+        22,
+        23,
+        24,
+        25,
+        26,
+        38
     ],
     "dep_prios": [
+        10,
+        5,
+        5,
+        5,
+        5,
         5,
         5,
         5,
         5,
         5,
         5,
         5,
+        20,
+        10,
+        10,
+        10,
+        10,
+        5,
+        5,
         5,
         10,
         5,
         30,
         30,
         30,
         30,
         30,
-        30
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5
     ],
     "dependencies": [
-        "rich.align",
+        "os.path",
+        "rich.containers",
+        "rich.padding",
+        "rich._loop",
         "rich.cells",
+        "rich.color",
         "rich.console",
         "rich.jupyter",
         "rich.measure",
+        "rich.segment",
         "rich.style",
         "rich.text",
-        "typing",
+        "os",
+        "platform",
+        "re",
         "sys",
+        "textwrap",
+        "abc",
+        "pathlib",
+        "typing",
+        "argparse",
         "builtins",
+        "_operator",
         "_random",
         "_typeshed",
-        "abc",
+        "array",
+        "ctypes",
         "datetime",
+        "enum",
+        "mmap",
+        "pickle",
+        "posixpath",
+        "rich.color_triplet",
+        "rich.terminal_theme",
         "rich.theme",
         "typing_extensions"
     ],
-    "hash": "ba63b6d568f0d0571801e4c1dd4ba634b0ac0d685e8f3c678e57f65708978832",
-    "id": "rich.rule",
+    "hash": "9a38be6e37e9f8a7caf77ca1bc6f15efb6b533d6bcef6fef750f1f7a2c967ce5",
+    "id": "rich.syntax",
     "ignore_all": true,
-    "interface_hash": "35c6e9d7e3cd1070eb6cf4dbfe676c2123dfa129f9a37351b5d011b3d539375e",
+    "interface_hash": "4d55a51d2f6d778e468cfbc604e9564429b36c2315dbfc35156cd6b4d46e7038",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -96,13 +168,20 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/rule.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/syntax.py",
     "plugin_data": null,
-    "size": 4590,
-    "suppressed": [],
+    "size": 35065,
+    "suppressed": [
+        "pygments.lexer",
+        "pygments.lexers",
+        "pygments.style",
+        "pygments.styles",
+        "pygments.token",
+        "pygments.util"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/scope.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/scope.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/models.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7271506271506271%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 18), (1, 22), (2, 24), (3, 25), (6, 3), (7, 16)], delete: [10, 9, '*

 * *                '8, 6, 5, 4, 3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(2, 25), (3, 25), (4, 10), (5, 10), (7, 10)], delete: [11, 10, 7, 4, 3, '*

 * *                '2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'typer._compat_utils'), (1, 'click.shell_completion'), (2, "*

 * *                   "'typer.core'), (3, 'typer.main'), (4, 'inspect'), (5, 'io'), (7, 'click'), "*

 * *                   "(10, 'click.core'), (11, 'clic […]*

```diff
@@ -1,68 +1,59 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
+        18,
+        22,
+        24,
+        25,
         1,
-        4,
-        5,
-        6,
-        7,
-        8,
-        11,
         2,
-        71,
-        1,
-        1,
+        3,
+        16,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
-        5,
-        5,
-        5,
         25,
+        25,
+        25,
+        10,
+        10,
         5,
+        10,
         5,
-        5,
-        30,
-        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "rich.highlighter",
-        "rich.panel",
-        "rich.pretty",
-        "rich.table",
-        "rich.text",
-        "rich.console",
+        "typer._compat_utils",
+        "click.shell_completion",
+        "typer.core",
+        "typer.main",
+        "inspect",
+        "io",
         "typing",
-        "rich",
+        "click",
         "builtins",
-        "_typeshed",
         "abc",
-        "rich.box",
-        "rich.jupyter",
-        "rich.style",
-        "typing_extensions"
+        "click.core",
+        "click.types",
+        "enum"
     ],
-    "hash": "95fe907adfdee09398df89708584801be3415d8281718bbab7f8a0bff2681a88",
-    "id": "rich.scope",
+    "hash": "0d625201001a209a45048efff3154017d132f4d3479b8755ea29f6b81ecdeca9",
+    "id": "typer.models",
     "ignore_all": true,
-    "interface_hash": "145a049def1168757354bd5707ab359e210969ef05b31e520f7c729e9f2e9a35",
-    "mtime": 1685143296,
+    "interface_hash": "239046e43ed828fba7030bdc4119029e194d6de90d24865db4033b0bab8d21c6",
+    "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -96,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/scope.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/models.py",
     "plugin_data": null,
-    "size": 2831,
+    "size": 15981,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/screen.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/screen.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/screen.meta.json` & `su6-0.3.0/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6885080988917306%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 23), (1, 30), (2, 1), (3, 2), (4, 21), (5, 22), (6, 24), (7, 25), '*

 * *                '(8, 26), (9, 27), (10, 28), (11, 33)], delete: [3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (5, 5), (6, 5), (7, 5), (8, 5), (9, 5), (12, 30), '*

 * *                '(13, 30)], delete: [3]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'os.path'), (2, 'sys'), (3, "*

 * *                   "'_typeshed'), (5, 'builtins'), (6, 'contextlib'), (7,  […]*

```diff
@@ -1,44 +1,68 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        3,
-        4,
-        5,
-        9,
+        23,
+        30,
+        1,
+        2,
+        21,
+        22,
+        24,
+        25,
+        26,
+        27,
+        28,
+        33,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        10,
+        5,
+        5,
+        5,
+        5,
         5,
         5,
-        20,
         5,
         5,
+        5,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "rich.segment",
-        "rich.style",
-        "rich._loop",
-        "rich.console",
-        "typing",
-        "builtins",
+        "collections.abc",
+        "os.path",
+        "sys",
+        "_typeshed",
         "abc",
-        "enum"
+        "builtins",
+        "contextlib",
+        "io",
+        "subprocess",
+        "typing",
+        "typing_extensions",
+        "types",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "acbfe3db05fee127ae20e236a0e95ce35f103fd100bc3e7d1889d4984004ea34",
-    "id": "rich.screen",
+    "hash": "43f0abc8936c573dfefd04ae185e74a6fc8eac1be65a0daaaf327303d8dc486e",
+    "id": "os",
     "ignore_all": true,
-    "interface_hash": "8db842986b5cbf3353da698ac5ce0831e10b1b74953434b144367bdd7fa15210",
-    "mtime": 1685143296,
+    "interface_hash": "7857e0241ab1ae7ccf1c6583d54898fa386079260ac7e105c7e8d281784f77c9",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +96,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/screen.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
     "plugin_data": null,
-    "size": 1579,
+    "size": 36995,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/segment.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/segment.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/segment.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/segment.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/spinner.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/spinner.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/spinner.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/spinner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/status.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/status.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/status.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/status.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/style.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/style.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/style.meta.json` & `su6-0.3.0/.mypy_cache/3.11/tests/__init__.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6488017429193901%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{delete: [13, 12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [14, 13, 12, 11, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(2, 'typing')], delete: [16, 15, 14, 12, 11, 9, 8, 7, 6, 5, 4, 3, 2, "*

 * *                   '1, 0]}',*

 * * "'hash'": "'9cb95505c34a091a9b6468d522af11f6aaf9c74162ad95203ed31ec0b221f000'",*

 * * "'id'": "'tests'",*

 * * "'ignore_all'": 'False',*

 * * "'interface_hash'": "'21c07076089f75f20122c2c5361d5ecfde47ebd323b9d3a43 […]*

```diff
@@ -1,71 +1,29 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        7,
-        8,
-        9,
-        10,
-        1,
-        2,
-        3,
-        4,
-        5,
-        7,
-        1,
-        1,
-        1,
-        1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
-        5,
-        5,
-        10,
         5,
-        5,
-        5,
-        5,
-        20,
-        5,
-        30,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "rich.errors",
-        "rich.color",
-        "rich.repr",
-        "rich.terminal_theme",
-        "sys",
-        "functools",
-        "marshal",
-        "random",
-        "typing",
-        "rich",
         "builtins",
-        "_collections_abc",
-        "_typeshed",
         "abc",
-        "enum",
-        "rich.color_triplet",
-        "typing_extensions"
+        "typing"
     ],
-    "hash": "de18a8707ff837cbf0466dfef32156ccceed4b08e312f7a7ebd5ea59ab124303",
-    "id": "rich.style",
-    "ignore_all": true,
-    "interface_hash": "c7e1e2ffb01b0740660c610c2734c5fe7cfe558f111403728cc12f3470cf5fbe",
-    "mtime": 1685143296,
+    "hash": "9cb95505c34a091a9b6468d522af11f6aaf9c74162ad95203ed31ec0b221f000",
+    "id": "tests",
+    "ignore_all": false,
+    "interface_hash": "21c07076089f75f20122c2c5361d5ecfde47ebd323b9d3a43f203539bfaaa50f",
+    "mtime": 1685143094,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -99,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/style.py",
+    "path": "./tests/__init__.py",
     "plugin_data": null,
-    "size": 27073,
+    "size": 121,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/styled.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/styled.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/styled.meta.json` & `su6-0.3.0/.mypy_cache/3.11/genericpath.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6979458450046685%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(1, 1), (2, 2)], delete: [10, 9, 8, 7, 6, 5, 4, 3]}',*

 * * "'dep_prios'": '{insert: [(1, 10)], delete: [11, 10, 9, 8, 3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'os'), (2, '_typeshed'), (4, "*

 * *                   "'typing_extensions')], delete: [12, 11, 10, 9, 6, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'50d45ab3fd6f6adc2a69a00ae4885e0c123e9e773ee3d3366768e99b9e6e8fbd'",*

 * * "'id'": "'genericpath'",*

 * * "'interface_hash'": "'592081edf3b264e91eeb7 […]*

```diff
@@ -1,59 +1,41 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
         3,
+        1,
+        2,
         4,
         5,
-        8,
-        39,
-        1,
-        38,
-        1,
-        1,
-        1,
-        1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
-        25,
+        10,
         5,
         5,
         5,
         5,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "rich.measure",
-        "rich.segment",
-        "rich.style",
-        "rich.console",
-        "rich.panel",
+        "collections.abc",
+        "os",
+        "_typeshed",
         "typing",
-        "rich",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "enum",
-        "rich.box",
-        "rich.jupyter",
-        "rich.text"
+        "abc"
     ],
-    "hash": "c258d5b154d76c004c319be4ce43b8dd9124ffe8abcc4b6f52243eb0d9e2910f",
-    "id": "rich.styled",
+    "hash": "50d45ab3fd6f6adc2a69a00ae4885e0c123e9e773ee3d3366768e99b9e6e8fbd",
+    "id": "genericpath",
     "ignore_all": true,
-    "interface_hash": "e950fe9af602055d5bd175e8aebc26b5ab0ed48f01495bd939716430abbacac8",
-    "mtime": 1685143296,
+    "interface_hash": "592081edf3b264e91eeb7bf8e751aaf367fa3108b344596ac367b31465b846dc",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -87,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/styled.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/genericpath.pyi",
     "plugin_data": null,
-    "size": 1234,
+    "size": 1756,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/syntax.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/syntax.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/syntax.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/traceback.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7668922305764412%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 29), (1, 30), (2, 31), (3, 32), (4, 33), (5, 34), (6, 35), (7, 36), '*

 * *                '(8, 37), (9, 38), (10, 39), (19, 9), (20, 10), (21, 29), (38, 27)], delete: [41, '*

 * *                '40, 39, 36, 21, 20, 13, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(12, 5), (21, 20), (22, 5)], delete: [38, 37, 36, 22, 20, 12]}',*

 * * "'dependencies'": "{insert: [(0, 'rich.pretty'), (2, 'rich.columns'), (4, 'rich.constrain'), (5, "*

 * *                   "'rich.highlighter'), […]*

```diff
@@ -1,139 +1,133 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        1,
+        29,
+        30,
+        31,
+        32,
+        33,
+        34,
+        35,
+        36,
+        37,
+        38,
+        39,
         40,
-        41,
-        43,
-        44,
-        45,
-        46,
-        47,
-        48,
-        49,
-        50,
-        51,
         1,
-        2,
         3,
         4,
         5,
         6,
         7,
         8,
-        832,
-        1,
+        9,
+        10,
+        29,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        22,
         23,
         24,
-        25,
-        26,
-        38
+        27
     ],
     "dep_prios": [
         10,
         5,
         5,
         5,
         5,
         5,
         5,
         5,
         5,
         5,
         5,
         5,
-        20,
+        5,
         10,
         10,
         10,
         10,
         5,
         5,
         5,
-        10,
+        5,
+        20,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        5,
-        5,
-        5,
         5,
         5,
         5
     ],
     "dependencies": [
-        "os.path",
-        "rich.containers",
-        "rich.padding",
+        "rich.pretty",
         "rich._loop",
-        "rich.cells",
-        "rich.color",
+        "rich.columns",
         "rich.console",
-        "rich.jupyter",
-        "rich.measure",
-        "rich.segment",
+        "rich.constrain",
+        "rich.highlighter",
+        "rich.panel",
+        "rich.scope",
         "rich.style",
+        "rich.syntax",
         "rich.text",
+        "rich.theme",
+        "__future__",
+        "linecache",
         "os",
         "platform",
-        "re",
         "sys",
-        "textwrap",
-        "abc",
-        "pathlib",
+        "dataclasses",
+        "traceback",
+        "types",
         "typing",
-        "argparse",
+        "rich",
         "builtins",
-        "_operator",
+        "_collections_abc",
         "_random",
         "_typeshed",
-        "array",
-        "ctypes",
+        "abc",
         "datetime",
         "enum",
-        "mmap",
-        "pickle",
+        "genericpath",
         "posixpath",
+        "rich.box",
+        "rich.color",
         "rich.color_triplet",
-        "rich.terminal_theme",
-        "rich.theme",
+        "rich.jupyter",
         "typing_extensions"
     ],
-    "hash": "9a38be6e37e9f8a7caf77ca1bc6f15efb6b533d6bcef6fef750f1f7a2c967ce5",
-    "id": "rich.syntax",
+    "hash": "b4124fe2ca292386eb42d94cad2f94cd9c580b3a1478294b7cb26f7ece0dd452",
+    "id": "rich.traceback",
     "ignore_all": true,
-    "interface_hash": "4d55a51d2f6d778e468cfbc604e9564429b36c2315dbfc35156cd6b4d46e7038",
+    "interface_hash": "d2ef2df374bfefbb85d247bf38b8e15d81062f6bf096279b6e233fad01d92608",
     "mtime": 1685143296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -168,20 +162,17 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/syntax.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/traceback.py",
     "plugin_data": null,
-    "size": 35065,
+    "size": 29532,
     "suppressed": [
-        "pygments.lexer",
         "pygments.lexers",
-        "pygments.style",
-        "pygments.styles",
         "pygments.token",
         "pygments.util"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/table.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/table.meta.json` & `su6-0.3.0/.mypy_cache/3.11/rich/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/terminal_theme.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/terminal_theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/terminal_theme.meta.json` & `su6-0.3.0/.mypy_cache/3.11/_warnings.meta.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7266666666666667%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{delete: [1, 0]}',*

 * * "'dep_prios'": '{delete: [1, 0]}',*

 * * "'dependencies'": '{delete: [1, 0]}',*

 * * "'hash'": "'12ca327a8db64a2d4a7ce3e48dec89640981b34dbc8f6485f78899f6bd7625bc'",*

 * * "'id'": "'_warnings'",*

 * * "'interface_hash'": "'d82c2fe96f249f6c67c9f318da861954091d569054e5678599df9778edc8c3ee'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_warnings.pyi'",*

 * * "'size'": '1026'}*

```diff
@@ -1,35 +1,29 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        3,
-        4,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5,
-        5,
         30
     ],
     "dependencies": [
-        "rich.color_triplet",
-        "rich.palette",
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "d63e7eb9f25f9ef940a3942c8bf0026625c39b0317cea826141c8e6d3f7ec896",
-    "id": "rich.terminal_theme",
+    "hash": "12ca327a8db64a2d4a7ce3e48dec89640981b34dbc8f6485f78899f6bd7625bc",
+    "id": "_warnings",
     "ignore_all": true,
-    "interface_hash": "cb0f63719435d76dbd314726350fc38ea160216dd2a40c3c64077245141adf2e",
-    "mtime": 1685143296,
+    "interface_hash": "d82c2fe96f249f6c67c9f318da861954091d569054e5678599df9778edc8c3ee",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/terminal_theme.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/_warnings.pyi",
     "plugin_data": null,
-    "size": 3370,
+    "size": 1026,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/text.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/text.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7002244421380384%*

 * *Differences: {"'dep_lines'": '{insert: [(5, 6), (6, 7), (7, 9), (20, 12)], delete: [23, 22, 21, 20, 14, 13, 12, '*

 * *                '11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (3, 10), (7, 10), (20, 10)], delete: [24, 23, 22, 21, '*

 * *                '16, 14, 13, 12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'os'), (2, 'subprocess'), (3, 'sys'), (4, 'enum'), (5, "*

 * *                   "'pathlib'), (7, 'click'), (11, 'click.core'), (12, 'click.exception […]*

```diff
@@ -1,128 +1,82 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        18,
-        19,
-        20,
-        21,
-        22,
-        23,
-        24,
-        25,
-        26,
-        27,
-        28,
-        29,
-        32,
-        219,
-        297,
         1,
         2,
         3,
         4,
         5,
+        6,
+        7,
+        9,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
-        1,
-        1,
-        1
+        12
     ],
     "dep_prios": [
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        20,
-        20,
+        10,
+        10,
+        10,
         10,
         5,
         5,
         5,
-        5,
+        10,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30
+        10
     ],
     "dependencies": [
-        "rich._loop",
-        "rich._pick",
-        "rich._wrap",
-        "rich.align",
-        "rich.cells",
-        "rich.containers",
-        "rich.control",
-        "rich.emoji",
-        "rich.jupyter",
-        "rich.measure",
-        "rich.segment",
-        "rich.style",
-        "rich.console",
-        "rich.markup",
-        "rich.ansi",
+        "os",
         "re",
-        "functools",
-        "math",
-        "operator",
+        "subprocess",
+        "sys",
+        "enum",
+        "pathlib",
         "typing",
+        "click",
         "builtins",
-        "_collections_abc",
-        "_operator",
-        "_random",
-        "_typeshed",
         "abc",
         "array",
+        "click.core",
+        "click.exceptions",
+        "click.globals",
+        "click.utils",
         "ctypes",
-        "datetime",
-        "enum",
+        "io",
         "mmap",
         "pickle",
-        "rich.color",
-        "rich.color_triplet",
-        "rich.theme",
         "typing_extensions"
     ],
-    "hash": "ab2364a4c8261f73ef9fca6336b60ca15f0c2d16e38b5c7e10e3f6a3a74433ad",
-    "id": "rich.text",
+    "hash": "07d57ab9af0bc9668092450a3be34d73bbc19793d036b5b9a1366b0434c02eb8",
+    "id": "typer._completion_shared",
     "ignore_all": true,
-    "interface_hash": "7dda9dbd02bd21fd9a4743298292110d1d478c433cff11c86d57acbc1b1f3914",
-    "mtime": 1685143296,
+    "interface_hash": "8a2072c243e4201d8048e9c080be92b7fb7bf1f0af99bbcca8e61271fd19a2af",
+    "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -156,13 +110,15 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/text.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_completion_shared.py",
     "plugin_data": null,
-    "size": 45513,
-    "suppressed": [],
+    "size": 8541,
+    "suppressed": [
+        "shellingham"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/theme.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/theme.meta.json` & `su6-0.3.0/.mypy_cache/3.11/su6_checker/core.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6513888888888888%*

 * *Differences: {"'data_mtime'": '1685143739',*

 * * "'dep_lines'": '{insert: [(2, 3), (3, 4), (4, 7), (15, 6)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 10), (2, 10), (15, 5)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'enum'), (1, 'inspect'), (2, 'operator'), (4, 'rich'), (6, "*

 * *                   "'_operator'), (9, 'array'), (10, 'ctypes'), (11, 'mmap'), (12, 'pickle'), (13, "*

 * *                   "'types')], delete: [12, 11, 10, 9, 8, 5, 2, 1, 0]}",*

 * * "'hash'": "'8b0663919c3c0dd90562c38fd1a1b39423b977 […]*

```diff
@@ -1,62 +1,67 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143739,
     "dep_lines": [
-        4,
-        5,
         1,
         2,
+        3,
+        4,
+        7,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1
+        6
     ],
     "dep_prios": [
-        5,
-        5,
+        10,
+        10,
+        10,
         10,
         5,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30
+        30,
+        5
     ],
     "dependencies": [
-        "rich.default_styles",
-        "rich.style",
-        "configparser",
+        "enum",
+        "inspect",
+        "operator",
         "typing",
+        "rich",
         "builtins",
-        "_collections_abc",
+        "_operator",
         "_typeshed",
         "abc",
-        "enum",
-        "functools",
-        "io",
-        "rich.color",
-        "rich.color_triplet",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle",
+        "types",
         "typing_extensions"
     ],
-    "hash": "6de9452688330345b41f2b1069b29a1ce7374561f6928ddf400261a0df8015da",
-    "id": "rich.theme",
-    "ignore_all": true,
-    "interface_hash": "60a22d4634a36c6a61e216557b933a97f163c0457d5c5980cd1a347ce29e181d",
-    "mtime": 1685143296,
+    "hash": "8b0663919c3c0dd90562c38fd1a1b39423b977de58b0bb1c6a616024d4d115d5",
+    "id": "su6_checker.core",
+    "ignore_all": false,
+    "interface_hash": "b0b2dfd0a37866e3640371d6d066f122b1a7cc5ee332534e093bf5707d163a85",
+    "mtime": 1685144281,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -90,13 +95,15 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/theme.py",
+    "path": "./src/su6_checker/core.py",
     "plugin_data": null,
-    "size": 3777,
-    "suppressed": [],
+    "size": 2823,
+    "suppressed": [
+        "plumbum.machines"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/themes.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/themes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/themes.meta.json` & `su6-0.3.0/.mypy_cache/3.11/su6_checker/cli.meta.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6344322344322344%*

 * *Differences: {"'data_mtime'": '1685143739',*

 * * "'dep_lines'": '{insert: [(0, 6), (2, 4), (3, 1), (4, 1), (5, 1), (6, 1), (11, 3), (12, 2)], '*

 * *                'delete: [1]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (4, 30), (5, 30), (6, 30), (7, 30), (11, 5), (12, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'su6_checker.core'), (1, 'typer'), (2, 'rich'), (5, 'click'), "*

 * *                   "(6, 'click.core'), (7, 'enum'), (8, 'typer.core'), (9, 'typer.main')], delete: "*

 * *                   '[4, 1, 0]}',*

 * * "'hash'": "'cd18a4ff378eef9 […]*

```diff
@@ -1,38 +1,57 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143739,
     "dep_lines": [
+        6,
         1,
-        2,
+        4,
         1,
         1,
         1,
-        1
+        1,
+        1,
+        1,
+        1,
+        1,
+        3,
+        2
     ],
     "dep_prios": [
         5,
+        10,
         5,
         5,
         30,
         30,
-        30
+        30,
+        30,
+        30,
+        30,
+        30,
+        5,
+        5
     ],
     "dependencies": [
-        "rich.default_styles",
-        "rich.theme",
+        "su6_checker.core",
+        "typer",
+        "rich",
         "builtins",
         "abc",
-        "rich.style",
+        "click",
+        "click.core",
+        "enum",
+        "typer.core",
+        "typer.main",
         "typing"
     ],
-    "hash": "d318132e8cdf69b79b62d709b43742e50917e4855411abe2a83509261e185459",
-    "id": "rich.themes",
-    "ignore_all": true,
-    "interface_hash": "c7645ea79e02f663c3e35494c3e38d3edbfed0d874cd39434350c8e598165d3a",
-    "mtime": 1685143296,
+    "hash": "cd18a4ff378eef9130e69d979763c8cee0daca13d45b2afbab68dafee4b20ca7",
+    "id": "su6_checker.cli",
+    "ignore_all": false,
+    "interface_hash": "3588acc0ff46745f90b61b8a8564c0d5c3a661f511418c007067a49e0009cefe",
+    "mtime": 1685144149,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -66,13 +85,16 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/themes.py",
+    "path": "./src/su6_checker/cli.py",
     "plugin_data": null,
-    "size": 102,
-    "suppressed": [],
+    "size": 2355,
+    "suppressed": [
+        "plumbum.commands.processes",
+        "plumbum"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/traceback.data.json` & `su6-0.3.0/.mypy_cache/3.11/rich/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/rich/traceback.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/core.meta.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6961691086691086%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 21), (1, 22), (2, 23), (3, 24), (4, 25), (5, 26), (6, 28), (8, 45), '*

 * *                '(10, 2), (15, 20), (16, 36), (17, 38), (18, 75)], delete: [38, 37, 36, 25, 24, '*

 * *                '23, 22, 21, 20, 19, 18, 17, 11, 10, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(7, 10), (8, 20), (9, 10), (10, 10), (11, 10), (12, 10), (15, 10), (16, '*

 * *                '10), (17, 20)], delete: [38, 37, 36, 26, 25, 24, 23, 12, 11, 10, 9, 8, 7, 6, 5, '*

 * *                '4, 3, 2, 1]}' […]*

```diff
@@ -1,134 +1,107 @@
 {
     "data_mtime": 1685143685,
     "dep_lines": [
-        29,
-        30,
-        31,
-        32,
-        33,
-        34,
-        35,
-        36,
-        37,
+        21,
+        22,
+        23,
+        24,
+        25,
+        26,
+        28,
         38,
-        39,
-        40,
+        45,
         1,
+        2,
         3,
         4,
         5,
         6,
-        7,
-        8,
-        9,
-        10,
-        29,
-        1,
-        1,
-        1,
-        1,
-        1,
+        20,
+        36,
+        38,
+        75,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        23,
-        24,
-        27
+        1
     ],
     "dep_prios": [
         10,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
         10,
         10,
         10,
         10,
         5,
         5,
+        10,
+        20,
+        10,
+        10,
+        10,
+        10,
         5,
         5,
+        10,
+        10,
+        20,
         20,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        5,
-        5,
-        5
+        30
     ],
     "dependencies": [
-        "rich.pretty",
-        "rich._loop",
-        "rich.columns",
-        "rich.console",
-        "rich.constrain",
-        "rich.highlighter",
-        "rich.panel",
-        "rich.scope",
-        "rich.style",
-        "rich.syntax",
-        "rich.text",
-        "rich.theme",
-        "__future__",
-        "linecache",
+        "click.core",
+        "click.formatting",
+        "click.parser",
+        "click.types",
+        "click.utils",
+        "typer.completion",
+        "typer._compat_utils",
+        "typer.rich_utils",
+        "click.shell_completion",
+        "errno",
+        "inspect",
         "os",
-        "platform",
         "sys",
-        "dataclasses",
-        "traceback",
-        "types",
+        "gettext",
         "typing",
+        "click",
         "rich",
+        "typer",
+        "warnings",
         "builtins",
-        "_collections_abc",
-        "_random",
         "_typeshed",
+        "_warnings",
         "abc",
-        "datetime",
-        "enum",
-        "genericpath",
+        "click.exceptions",
+        "contextlib",
         "posixpath",
-        "rich.box",
-        "rich.color",
-        "rich.color_triplet",
-        "rich.jupyter",
+        "typer._completion_click8",
+        "types",
         "typing_extensions"
     ],
-    "hash": "b4124fe2ca292386eb42d94cad2f94cd9c580b3a1478294b7cb26f7ece0dd452",
-    "id": "rich.traceback",
+    "hash": "4e854e1f3b38cac177e4a25af37050960cc2cdc54d10c257791d45283ac3a5a9",
+    "id": "typer.core",
     "ignore_all": true,
-    "interface_hash": "d2ef2df374bfefbb85d247bf38b8e15d81062f6bf096279b6e233fad01d92608",
-    "mtime": 1685143296,
+    "interface_hash": "33d5bc0ff98d72d3db1e6bf73791db31120d3dafa533c19c29166de8075ffbde",
+    "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -162,17 +135,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/rich/traceback.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/core.py",
     "plugin_data": null,
-    "size": 29532,
-    "suppressed": [
-        "pygments.lexers",
-        "pygments.token",
-        "pygments.util"
-    ],
+    "size": 26545,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6/__about__.data.json` & `su6-0.3.0/.mypy_cache/3.11/su6/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6/__about__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/su6_checker/__about__.meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'hash'": "'46e2988ae1702a50dd3052be264502bf790bc8ca34b94c10734f97eb9318bbbd'",*

 * * "'id'": "'su6_checker.__about__'",*

 * * "'interface_hash'": "'a79aa7369a97c75e7bfc1e2f3354408dc43aee52edbee9bbe45bc7e844e176b6'",*

 * * "'mtime'": '1685144868',*

 * * "'path'": "'./src/su6_checker/__about__.py'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1685146214,
+    "data_mtime": 1685143683,
     "dep_lines": [
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
@@ -11,19 +11,19 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "e9a58844f67aff84c431d3aac8f4f74bbbc44b3f749c6a3e202143fef0e0eeb0",
-    "id": "su6.__about__",
+    "hash": "46e2988ae1702a50dd3052be264502bf790bc8ca34b94c10734f97eb9318bbbd",
+    "id": "su6_checker.__about__",
     "ignore_all": false,
-    "interface_hash": "73c9ac79eb0b2bf75c6e787a1d921f977526fc73313e41372a43d62b6fc02d1d",
-    "mtime": 1685148487,
+    "interface_hash": "a79aa7369a97c75e7bfc1e2f3354408dc43aee52edbee9bbe45bc7e844e176b6",
+    "mtime": 1685144868,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "./src/su6/__about__.py",
+    "path": "./src/su6_checker/__about__.py",
     "plugin_data": null,
     "size": 143,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/su6/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/su6/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8533333333333334%*

 * *Differences: {"'data_mtime'": '1685286348',*

 * * "'dep_lines'": '{insert: [(0, 9)], delete: [0]}',*

 * * "'hash'": "'cab9864f675f6c76c8579e49a2ea81629110297e5cafd6028bf9b9873113a865'",*

 * * "'mtime'": '1685282367',*

 * * "'size'": '236'}*

```diff
@@ -1,11 +1,11 @@
 {
-    "data_mtime": 1685148117,
+    "data_mtime": 1685286348,
     "dep_lines": [
-        5,
+        9,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
@@ -14,19 +14,19 @@
     ],
     "dependencies": [
         "su6.cli",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "ca089ccb38ce7569624ce14a10bea4336b681d56e19c91a9406801ae2abb5a53",
+    "hash": "cab9864f675f6c76c8579e49a2ea81629110297e5cafd6028bf9b9873113a865",
     "id": "su6",
     "ignore_all": false,
     "interface_hash": "b2f06ca7a6b4477d164accefc86cd30f898f9f83f7dcbbcd81fa1923e5082dbf",
-    "mtime": 1685146356,
+    "mtime": 1685282367,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -62,11 +62,11 @@
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
     "path": "./src/su6/__init__.py",
     "plugin_data": null,
-    "size": 188,
+    "size": 236,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6/cli.data.json` & `su6-0.3.0/.mypy_cache/3.11/su6_checker/core.data.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8063949938949939%*

 * *Differences: {"'_fullname'": "'su6_checker.core'",*

 * * "'names'": "{'DEFAULT_VERBOSITY': {'node': OrderedDict([('.class', 'Var'), ('flags', "*

 * *            "['is_inferred', 'has_explicit_value']), ('fullname', "*

 * *            "'su6_checker.core.DEFAULT_VERBOSITY'), ('name', 'DEFAULT_VERBOSITY'), ('type', "*

 * *            "'su6_checker.core.Verbosity')]), delete: ['cross_ref', 'module_hidden', "*

 * *            "'module_public']}, 'Verbosity': {'node': OrderedDict([('.class', 'TypeInfo'), "*

 * *            "('_promote', []), ('abstract_at […]*

```diff
@@ -1,238 +1,685 @@
 {
     ".class": "MypyFile",
-    "_fullname": "su6.cli",
+    "_fullname": "su6_checker.core",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
         "DEFAULT_VERBOSITY": {
             ".class": "SymbolTableNode",
-            "cross_ref": "su6.core.DEFAULT_VERBOSITY",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "GREEN_CIRCLE": {
-            ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
                     "is_inferred",
                     "has_explicit_value"
                 ],
-                "fullname": "su6.cli.GREEN_CIRCLE",
-                "name": "GREEN_CIRCLE",
-                "type": "builtins.str"
+                "fullname": "su6_checker.core.DEFAULT_VERBOSITY",
+                "name": "DEFAULT_VERBOSITY",
+                "type": "su6_checker.core.Verbosity"
             }
         },
-        "ProcessExecutionError": {
+        "LocalCommand": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_suppressed_import",
                     "is_ready",
                     "is_inferred"
                 ],
-                "fullname": "su6.cli.ProcessExecutionError",
-                "name": "ProcessExecutionError",
+                "fullname": "su6_checker.core.LocalCommand",
+                "name": "LocalCommand",
                 "type": {
                     ".class": "AnyType",
-                    "missing_import_name": "su6.cli.ProcessExecutionError",
+                    "missing_import_name": "su6_checker.core.LocalCommand",
                     "source_any": null,
                     "type_of_any": 3
                 }
             }
         },
-        "RED_CIRCLE": {
+        "Verbosity": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "Var",
+                ".class": "TypeInfo",
+                "_promote": [],
+                "abstract_attributes": [],
+                "alt_promote": null,
+                "bases": [
+                    "enum.Enum"
+                ],
+                "dataclass_transform_spec": null,
+                "declared_metaclass": null,
+                "defn": {
+                    ".class": "ClassDef",
+                    "fullname": "su6_checker.core.Verbosity",
+                    "name": "Verbosity",
+                    "type_vars": []
+                },
+                "deletable_attributes": [],
                 "flags": [
-                    "is_ready",
-                    "is_inferred",
-                    "has_explicit_value"
+                    "is_enum"
                 ],
-                "fullname": "su6.cli.RED_CIRCLE",
-                "name": "RED_CIRCLE",
-                "type": "builtins.str"
-            }
-        },
-        "T_Command": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeAlias",
-                "alias_tvars": [],
-                "column": 0,
-                "fullname": "su6.cli.T_Command",
-                "line": 35,
-                "no_args": false,
-                "normalized": false,
-                "target": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        2,
-                        4
-                    ],
-                    "arg_names": [
-                        null,
-                        null
-                    ],
-                    "arg_types": [
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 6
-                        },
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 6
+                "fullname": "su6_checker.core.Verbosity",
+                "has_param_spec_type": false,
+                "metaclass_type": "enum.EnumMeta",
+                "metadata": {},
+                "module_name": "su6_checker.core",
+                "mro": [
+                    "su6_checker.core.Verbosity",
+                    "enum.Enum",
+                    "builtins.object"
+                ],
+                "names": {
+                    ".class": "SymbolTable",
+                    "__eq__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                null,
+                                null
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6_checker.core.Verbosity.__eq__",
+                            "name": "__eq__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    null,
+                                    null
+                                ],
+                                "arg_types": [
+                                    "su6_checker.core.Verbosity",
+                                    {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "su6_checker.core.Verbosity",
+                                            "builtins.str",
+                                            "builtins.int",
+                                            "builtins.object"
+                                        ]
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__eq__ of Verbosity",
+                                "ret_type": "builtins.bool",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
                         }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {},
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": true,
-                    "name": null,
-                    "ret_type": {
-                        ".class": "UnionType",
-                        "items": [
-                            "builtins.bool",
-                            "builtins.int"
-                        ]
                     },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
-        },
-        "T_Inner_Wrapper": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeAlias",
-                "alias_tvars": [],
-                "column": 0,
-                "fullname": "su6.cli.T_Inner_Wrapper",
-                "line": 37,
-                "no_args": false,
-                "normalized": false,
-                "target": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        2,
-                        4
-                    ],
-                    "arg_names": [
-                        null,
-                        null
-                    ],
-                    "arg_types": [
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 6
-                        },
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 6
+                    "__ge__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                null,
+                                null
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6_checker.core.Verbosity.__ge__",
+                            "name": "__ge__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    null,
+                                    null
+                                ],
+                                "arg_types": [
+                                    "su6_checker.core.Verbosity",
+                                    {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__ge__ of Verbosity",
+                                "ret_type": "builtins.bool",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
                         }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {},
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": true,
-                    "name": null,
-                    "ret_type": "builtins.int",
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
+                    },
+                    "__gt__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                null,
+                                null
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6_checker.core.Verbosity.__gt__",
+                            "name": "__gt__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    null,
+                                    null
+                                ],
+                                "arg_types": [
+                                    "su6_checker.core.Verbosity",
+                                    {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__gt__ of Verbosity",
+                                "ret_type": "builtins.bool",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "__hash__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6_checker.core.Verbosity.__hash__",
+                            "name": "__hash__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "su6_checker.core.Verbosity"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__hash__ of Verbosity",
+                                "ret_type": "builtins.int",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "__le__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                null,
+                                null
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6_checker.core.Verbosity.__le__",
+                            "name": "__le__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    null,
+                                    null
+                                ],
+                                "arg_types": [
+                                    "su6_checker.core.Verbosity",
+                                    {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__le__ of Verbosity",
+                                "ret_type": "builtins.bool",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "__lt__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                null,
+                                null
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6_checker.core.Verbosity.__lt__",
+                            "name": "__lt__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    null,
+                                    null
+                                ],
+                                "arg_types": [
+                                    "su6_checker.core.Verbosity",
+                                    {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__lt__ of Verbosity",
+                                "ret_type": "builtins.bool",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "_compare": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Decorator",
+                            "func": {
+                                ".class": "FuncDef",
+                                "abstract_status": 0,
+                                "arg_kinds": [
+                                    0,
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "other",
+                                    "_operator"
+                                ],
+                                "dataclass_transform_spec": null,
+                                "flags": [
+                                    "is_static",
+                                    "is_decorated"
+                                ],
+                                "fullname": "su6_checker.core.Verbosity._compare",
+                                "name": "_compare",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0,
+                                        0,
+                                        0
+                                    ],
+                                    "arg_names": [
+                                        "self",
+                                        "other",
+                                        "_operator"
+                                    ],
+                                    "arg_types": [
+                                        "su6_checker.core.Verbosity",
+                                        {
+                                            ".class": "TypeAliasType",
+                                            "args": [],
+                                            "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                        },
+                                        {
+                                            ".class": "CallableType",
+                                            "arg_kinds": [
+                                                0,
+                                                0
+                                            ],
+                                            "arg_names": [
+                                                null,
+                                                null
+                                            ],
+                                            "arg_types": [
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                                },
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                                }
+                                            ],
+                                            "bound_args": [],
+                                            "def_extras": {},
+                                            "fallback": "builtins.function",
+                                            "from_concatenate": false,
+                                            "implicit": false,
+                                            "is_ellipsis_args": false,
+                                            "name": null,
+                                            "ret_type": "builtins.bool",
+                                            "type_guard": null,
+                                            "unpack_kwargs": false,
+                                            "variables": []
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": null
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "_compare of Verbosity",
+                                    "ret_type": "builtins.bool",
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            },
+                            "is_overload": false,
+                            "var": {
+                                ".class": "Var",
+                                "flags": [
+                                    "is_initialized_in_class",
+                                    "is_staticmethod",
+                                    "is_ready",
+                                    "is_inferred"
+                                ],
+                                "fullname": "su6_checker.core.Verbosity._compare",
+                                "name": "_compare",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0,
+                                        0,
+                                        0
+                                    ],
+                                    "arg_names": [
+                                        "self",
+                                        "other",
+                                        "_operator"
+                                    ],
+                                    "arg_types": [
+                                        "su6_checker.core.Verbosity",
+                                        {
+                                            ".class": "TypeAliasType",
+                                            "args": [],
+                                            "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                        },
+                                        {
+                                            ".class": "CallableType",
+                                            "arg_kinds": [
+                                                0,
+                                                0
+                                            ],
+                                            "arg_names": [
+                                                null,
+                                                null
+                                            ],
+                                            "arg_types": [
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                                },
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "su6_checker.core.Verbosity_Comparable"
+                                                }
+                                            ],
+                                            "bound_args": [],
+                                            "def_extras": {},
+                                            "fallback": "builtins.function",
+                                            "from_concatenate": false,
+                                            "implicit": false,
+                                            "is_ellipsis_args": false,
+                                            "name": null,
+                                            "ret_type": "builtins.bool",
+                                            "type_guard": null,
+                                            "unpack_kwargs": false,
+                                            "variables": []
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": null
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "_compare of Verbosity",
+                                    "ret_type": "builtins.bool",
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            }
+                        }
+                    },
+                    "normal": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_final",
+                                "is_ready",
+                                "is_inferred",
+                                "has_explicit_value"
+                            ],
+                            "fullname": "su6_checker.core.Verbosity.normal",
+                            "name": "normal",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [],
+                                "last_known_value": {
+                                    ".class": "LiteralType",
+                                    "fallback": "builtins.str",
+                                    "value": "2"
+                                },
+                                "type_ref": "builtins.str"
+                            }
+                        }
+                    },
+                    "quiet": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_final",
+                                "is_ready",
+                                "is_inferred",
+                                "has_explicit_value"
+                            ],
+                            "fullname": "su6_checker.core.Verbosity.quiet",
+                            "name": "quiet",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [],
+                                "last_known_value": {
+                                    ".class": "LiteralType",
+                                    "fallback": "builtins.str",
+                                    "value": "1"
+                                },
+                                "type_ref": "builtins.str"
+                            }
+                        }
+                    },
+                    "verbose": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_final",
+                                "is_ready",
+                                "is_inferred",
+                                "has_explicit_value"
+                            ],
+                            "fullname": "su6_checker.core.Verbosity.verbose",
+                            "name": "verbose",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [],
+                                "last_known_value": {
+                                    ".class": "LiteralType",
+                                    "fallback": "builtins.str",
+                                    "value": "3"
+                                },
+                                "type_ref": "builtins.str"
+                            }
+                        }
+                    }
+                },
+                "self_type": null,
+                "slots": null,
+                "tuple_type": null,
+                "type_vars": [],
+                "typeddict_type": null
             }
         },
-        "T_Outer_Wrapper": {
+        "Verbosity_Comparable": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
-                "fullname": "su6.cli.T_Outer_Wrapper",
-                "line": 40,
+                "fullname": "su6_checker.core.Verbosity_Comparable",
+                "line": 63,
                 "no_args": false,
                 "normalized": false,
                 "target": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0
-                    ],
-                    "arg_names": [
-                        null
-                    ],
-                    "arg_types": [
-                        {
-                            ".class": "TypeAliasType",
-                            "args": [],
-                            "type_ref": "su6.cli.T_Command"
-                        }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {},
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": null,
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "su6.cli.T_Inner_Wrapper"
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
+                    ".class": "UnionType",
+                    "items": [
+                        "su6_checker.core.Verbosity",
+                        "builtins.str",
+                        "builtins.int"
+                    ]
                 }
             }
         },
-        "Verbosity": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "su6.core.Verbosity",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
         "__annotations__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.cli.__annotations__",
+                "fullname": "su6_checker.core.__annotations__",
                 "name": "__annotations__",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
                             ".class": "AnyType",
@@ -249,897 +696,335 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.cli.__doc__",
+                "fullname": "su6_checker.core.__doc__",
                 "name": "__doc__",
                 "type": "builtins.str"
             }
         },
         "__file__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.cli.__file__",
+                "fullname": "su6_checker.core.__file__",
                 "name": "__file__",
                 "type": "builtins.str"
             }
         },
         "__name__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.cli.__name__",
+                "fullname": "su6_checker.core.__name__",
                 "name": "__name__",
                 "type": "builtins.str"
             }
         },
         "__package__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.cli.__package__",
+                "fullname": "su6_checker.core.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
-        "_check_tool": {
+        "danger": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
-                    0,
-                    2,
-                    5
+                    2
                 ],
                 "arg_names": [
-                    "tool",
-                    "args",
-                    "verbosity"
+                    "args"
                 ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "su6.cli._check_tool",
-                "name": "_check_tool",
+                "fullname": "su6_checker.core.danger",
+                "name": "danger",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
-                        0,
-                        2,
-                        5
+                        2
                     ],
                     "arg_names": [
-                        "tool",
-                        "args",
-                        "verbosity"
+                        "args"
                     ],
                     "arg_types": [
-                        "builtins.str",
-                        "builtins.str",
-                        "su6.core.Verbosity"
+                        "builtins.str"
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "_check_tool",
-                    "ret_type": "builtins.int",
+                    "name": "danger",
+                    "ret_type": {
+                        ".class": "NoneType"
+                    },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "app": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "Var",
-                "flags": [
-                    "is_inferred",
-                    "has_explicit_value"
-                ],
-                "fullname": "su6.cli.app",
-                "name": "app",
-                "type": "typer.main.Typer"
-            }
-        },
-        "bandit": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "Decorator",
-                "func": {
-                    ".class": "FuncDef",
-                    "abstract_status": 0,
-                    "arg_kinds": [
-                        1
-                    ],
-                    "arg_names": [
-                        "verbosity"
-                    ],
-                    "dataclass_transform_spec": null,
-                    "flags": [
-                        "is_decorated"
-                    ],
-                    "fullname": "su6.cli.bandit",
-                    "name": "bandit",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            1
-                        ],
-                        "arg_names": [
-                            "verbosity"
-                        ],
-                        "arg_types": [
-                            "su6.core.Verbosity"
-                        ],
-                        "bound_args": [],
-                        "def_extras": {
-                            "first_arg": null
-                        },
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": false,
-                        "name": "bandit",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                },
-                "is_overload": false,
-                "var": {
-                    ".class": "Var",
-                    "flags": [
-                        "is_ready",
-                        "is_inferred"
-                    ],
-                    "fullname": "su6.cli.bandit",
-                    "name": "bandit",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            2,
-                            4
-                        ],
-                        "arg_names": [
-                            null,
-                            null
-                        ],
-                        "arg_types": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            }
-                        ],
-                        "bound_args": [],
-                        "def_extras": {},
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": true,
-                        "name": "bandit",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                }
-            }
-        },
-        "black": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "Decorator",
-                "func": {
-                    ".class": "FuncDef",
-                    "abstract_status": 0,
-                    "arg_kinds": [
-                        1,
-                        1
-                    ],
-                    "arg_names": [
-                        "fix",
-                        "verbosity"
-                    ],
-                    "dataclass_transform_spec": null,
-                    "flags": [
-                        "is_decorated"
-                    ],
-                    "fullname": "su6.cli.black",
-                    "name": "black",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            1,
-                            1
-                        ],
-                        "arg_names": [
-                            "fix",
-                            "verbosity"
-                        ],
-                        "arg_types": [
-                            "builtins.bool",
-                            "su6.core.Verbosity"
-                        ],
-                        "bound_args": [],
-                        "def_extras": {
-                            "first_arg": null
-                        },
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": false,
-                        "name": "black",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                },
-                "is_overload": false,
-                "var": {
-                    ".class": "Var",
-                    "flags": [
-                        "is_ready",
-                        "is_inferred"
-                    ],
-                    "fullname": "su6.cli.black",
-                    "name": "black",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            2,
-                            4
-                        ],
-                        "arg_names": [
-                            null,
-                            null
-                        ],
-                        "arg_types": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            }
-                        ],
-                        "bound_args": [],
-                        "def_extras": {},
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": true,
-                        "name": "black",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                }
-            }
-        },
-        "check_all": {
+        "enum": {
             ".class": "SymbolTableNode",
+            "cross_ref": "enum",
             "kind": "Gdef",
-            "node": {
-                ".class": "Decorator",
-                "func": {
-                    ".class": "FuncDef",
-                    "abstract_status": 0,
-                    "arg_kinds": [
-                        1
-                    ],
-                    "arg_names": [
-                        "verbosity"
-                    ],
-                    "dataclass_transform_spec": null,
-                    "flags": [
-                        "is_decorated"
-                    ],
-                    "fullname": "su6.cli.check_all",
-                    "name": "check_all",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            1
-                        ],
-                        "arg_names": [
-                            "verbosity"
-                        ],
-                        "arg_types": [
-                            "su6.core.Verbosity"
-                        ],
-                        "bound_args": [],
-                        "def_extras": {
-                            "first_arg": null
-                        },
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": false,
-                        "name": "check_all",
-                        "ret_type": "builtins.bool",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                },
-                "is_overload": false,
-                "var": {
-                    ".class": "Var",
-                    "flags": [
-                        "is_ready",
-                        "is_inferred"
-                    ],
-                    "fullname": "su6.cli.check_all",
-                    "name": "check_all",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            2,
-                            4
-                        ],
-                        "arg_names": [
-                            null,
-                            null
-                        ],
-                        "arg_types": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            }
-                        ],
-                        "bound_args": [],
-                        "def_extras": {},
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": true,
-                        "name": "check_all",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                }
-            }
+            "module_hidden": true,
+            "module_public": false
         },
-        "do_fix": {
+        "info": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "Decorator",
-                "func": {
-                    ".class": "FuncDef",
-                    "abstract_status": 0,
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    2
+                ],
+                "arg_names": [
+                    "args"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "su6_checker.core.info",
+                "name": "info",
+                "type": {
+                    ".class": "CallableType",
                     "arg_kinds": [
-                        1
+                        2
                     ],
                     "arg_names": [
-                        "verbosity"
+                        "args"
                     ],
-                    "dataclass_transform_spec": null,
-                    "flags": [
-                        "is_decorated"
-                    ],
-                    "fullname": "su6.cli.do_fix",
-                    "name": "do_fix",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            1
-                        ],
-                        "arg_names": [
-                            "verbosity"
-                        ],
-                        "arg_types": [
-                            "su6.core.Verbosity"
-                        ],
-                        "bound_args": [],
-                        "def_extras": {
-                            "first_arg": null
-                        },
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": false,
-                        "name": "do_fix",
-                        "ret_type": "builtins.bool",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                },
-                "is_overload": false,
-                "var": {
-                    ".class": "Var",
-                    "flags": [
-                        "is_ready",
-                        "is_inferred"
+                    "arg_types": [
+                        "builtins.str"
                     ],
-                    "fullname": "su6.cli.do_fix",
-                    "name": "do_fix",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            2,
-                            4
-                        ],
-                        "arg_names": [
-                            null,
-                            null
-                        ],
-                        "arg_types": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            }
-                        ],
-                        "bound_args": [],
-                        "def_extras": {},
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": true,
-                        "name": "do_fix",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "info",
+                    "ret_type": {
+                        ".class": "NoneType"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
                 }
             }
         },
-        "functools": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "functools",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "info": {
+        "inspect": {
             ".class": "SymbolTableNode",
-            "cross_ref": "su6.core.info",
+            "cross_ref": "inspect",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "isort": {
+        "log_cmd_output": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "Decorator",
-                "func": {
-                    ".class": "FuncDef",
-                    "abstract_status": 0,
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    0
+                ],
+                "arg_names": [
+                    "stdout",
+                    "stderr"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "su6_checker.core.log_cmd_output",
+                "name": "log_cmd_output",
+                "type": {
+                    ".class": "CallableType",
                     "arg_kinds": [
-                        1,
-                        1
+                        0,
+                        0
                     ],
                     "arg_names": [
-                        "fix",
-                        "verbosity"
-                    ],
-                    "dataclass_transform_spec": null,
-                    "flags": [
-                        "is_decorated"
+                        "stdout",
+                        "stderr"
                     ],
-                    "fullname": "su6.cli.isort",
-                    "name": "isort",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            1,
-                            1
-                        ],
-                        "arg_names": [
-                            "fix",
-                            "verbosity"
-                        ],
-                        "arg_types": [
-                            "builtins.bool",
-                            "su6.core.Verbosity"
-                        ],
-                        "bound_args": [],
-                        "def_extras": {
-                            "first_arg": null
-                        },
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": false,
-                        "name": "isort",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                },
-                "is_overload": false,
-                "var": {
-                    ".class": "Var",
-                    "flags": [
-                        "is_ready",
-                        "is_inferred"
+                    "arg_types": [
+                        "builtins.str",
+                        "builtins.str"
                     ],
-                    "fullname": "su6.cli.isort",
-                    "name": "isort",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            2,
-                            4
-                        ],
-                        "arg_names": [
-                            null,
-                            null
-                        ],
-                        "arg_types": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            }
-                        ],
-                        "bound_args": [],
-                        "def_extras": {},
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": true,
-                        "name": "isort",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "log_cmd_output",
+                    "ret_type": {
+                        ".class": "NoneType"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
                 }
             }
         },
-        "local": {
+        "log_command": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false,
             "node": {
-                ".class": "Var",
-                "flags": [
-                    "is_suppressed_import",
-                    "is_ready",
-                    "is_inferred"
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    0
                 ],
-                "fullname": "su6.cli.local",
-                "name": "local",
+                "arg_names": [
+                    "command",
+                    "args"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "su6_checker.core.log_command",
+                "name": "log_command",
                 "type": {
-                    ".class": "AnyType",
-                    "missing_import_name": "su6.cli.local",
-                    "source_any": null,
-                    "type_of_any": 3
-                }
-            }
-        },
-        "log_cmd_output": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "su6.core.log_cmd_output",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "log_command": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "su6.core.log_command",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "mypy": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "Decorator",
-                "func": {
-                    ".class": "FuncDef",
-                    "abstract_status": 0,
+                    ".class": "CallableType",
                     "arg_kinds": [
-                        1
+                        0,
+                        0
                     ],
                     "arg_names": [
-                        "verbosity"
+                        "command",
+                        "args"
                     ],
-                    "dataclass_transform_spec": null,
-                    "flags": [
-                        "is_decorated"
-                    ],
-                    "fullname": "su6.cli.mypy",
-                    "name": "mypy",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            1
-                        ],
-                        "arg_names": [
-                            "verbosity"
-                        ],
-                        "arg_types": [
-                            "su6.core.Verbosity"
-                        ],
-                        "bound_args": [],
-                        "def_extras": {
-                            "first_arg": null
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": "su6_checker.core.LocalCommand",
+                            "source_any": null,
+                            "type_of_any": 3
                         },
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": false,
-                        "name": "mypy",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                },
-                "is_overload": false,
-                "var": {
-                    ".class": "Var",
-                    "flags": [
-                        "is_ready",
-                        "is_inferred"
+                        {
+                            ".class": "Instance",
+                            "args": [
+                                "builtins.str"
+                            ],
+                            "type_ref": "typing.Iterable"
+                        }
                     ],
-                    "fullname": "su6.cli.mypy",
-                    "name": "mypy",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            2,
-                            4
-                        ],
-                        "arg_names": [
-                            null,
-                            null
-                        ],
-                        "arg_types": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            }
-                        ],
-                        "bound_args": [],
-                        "def_extras": {},
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": true,
-                        "name": "mypy",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "log_command",
+                    "ret_type": {
+                        ".class": "NoneType"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
                 }
             }
         },
-        "print": {
+        "operator": {
             ".class": "SymbolTableNode",
-            "cross_ref": "rich.print",
+            "cross_ref": "operator",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "ruff": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "Decorator",
-                "func": {
-                    ".class": "FuncDef",
-                    "abstract_status": 0,
-                    "arg_kinds": [
-                        1
-                    ],
-                    "arg_names": [
-                        "verbosity"
-                    ],
-                    "dataclass_transform_spec": null,
-                    "flags": [
-                        "is_decorated"
-                    ],
-                    "fullname": "su6.cli.ruff",
-                    "name": "ruff",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            1
-                        ],
-                        "arg_names": [
-                            "verbosity"
-                        ],
-                        "arg_types": [
-                            "su6.core.Verbosity"
-                        ],
-                        "bound_args": [],
-                        "def_extras": {
-                            "first_arg": null
-                        },
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": false,
-                        "name": "ruff",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                },
-                "is_overload": false,
-                "var": {
-                    ".class": "Var",
-                    "flags": [
-                        "is_ready",
-                        "is_inferred"
-                    ],
-                    "fullname": "su6.cli.ruff",
-                    "name": "ruff",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            2,
-                            4
-                        ],
-                        "arg_names": [
-                            null,
-                            null
-                        ],
-                        "arg_types": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 6
-                            }
-                        ],
-                        "bound_args": [],
-                        "def_extras": {},
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": true,
-                        "name": "ruff",
-                        "ret_type": "builtins.int",
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                }
-            }
-        },
-        "typer": {
+        "print": {
             ".class": "SymbolTableNode",
-            "cross_ref": "typer",
+            "cross_ref": "rich.print",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
         "typing": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "with_exit_code": {
+        "warn": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
-                "arg_kinds": [],
-                "arg_names": [],
+                "arg_kinds": [
+                    2
+                ],
+                "arg_names": [
+                    "args"
+                ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "su6.cli.with_exit_code",
-                "name": "with_exit_code",
+                "fullname": "su6_checker.core.warn",
+                "name": "warn",
                 "type": {
                     ".class": "CallableType",
-                    "arg_kinds": [],
-                    "arg_names": [],
-                    "arg_types": [],
+                    "arg_kinds": [
+                        2
+                    ],
+                    "arg_names": [
+                        "args"
+                    ],
+                    "arg_types": [
+                        "builtins.str"
+                    ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "with_exit_code",
+                    "name": "warn",
                     "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "su6.cli.T_Outer_Wrapper"
+                        ".class": "NoneType"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         }
     },
-    "path": "./src/su6/cli.py"
+    "path": "./src/su6_checker/core.py"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6/cli.meta.json` & `su6-0.3.0/.mypy_cache/3.11/zlib.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6359683794466403%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(2, 3)], delete: [20, 19, 11, 10, 9, 8, 7, 6, 5, 4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 5)], delete: [20, 19, 12, 11, 10, 9, 8, 7, 6, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (2, 'typing_extensions'), (3, 'builtins'), (9, "*

 * *                   "'typing')], delete: [18, 17, 16, 13, 11, 10, 9, 5, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'5cfaadb83c98fbafc7b16f74eb5a6a88e32ad3912d1b9d89a788983ed3e6a8e3'",*

 * * "'id'": "'zlib'",*

 * * "'ignore_all'": 'True', […]*

```diff
@@ -1,81 +1,50 @@
 {
-    "data_mtime": 1685148928,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        9,
         1,
         2,
-        4,
-        7,
+        3,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        6,
-        5
+        1
     ],
     "dep_prios": [
-        5,
-        10,
-        10,
         10,
         5,
         5,
+        5,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        5,
-        5
+        30
     ],
     "dependencies": [
-        "su6.core",
-        "functools",
-        "typing",
-        "typer",
-        "rich",
-        "builtins",
+        "sys",
         "_typeshed",
+        "typing_extensions",
+        "builtins",
         "abc",
         "array",
-        "click",
-        "click.core",
-        "click.exceptions",
         "ctypes",
-        "enum",
         "mmap",
         "pickle",
-        "typer.core",
-        "typer.main",
-        "typing_extensions"
+        "typing"
     ],
-    "hash": "2f622c4e1719bfd8acce3044af22cd86be69334fe1ae828e9684e1ef9f41f503",
-    "id": "su6.cli",
-    "ignore_all": false,
-    "interface_hash": "07d95b9b95509e8cbc7df0688784cc647a2f9b18b61a07ff36cf66e8b991df86",
-    "mtime": 1685149859,
+    "hash": "5cfaadb83c98fbafc7b16f74eb5a6a88e32ad3912d1b9d89a788983ed3e6a8e3",
+    "id": "zlib",
+    "ignore_all": true,
+    "interface_hash": "bdf2de9a898fcc3adbcefd8746e9d3e9006aa3491765c1ac71dd5e4efa0dc516",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -109,16 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "./src/su6/cli.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/zlib.pyi",
     "plugin_data": null,
-    "size": 4337,
-    "suppressed": [
-        "plumbum.commands.processes",
-        "plumbum"
-    ],
+    "size": 1787,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6/core.data.json` & `su6-0.3.0/.mypy_cache/3.11/su6/core.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999813988095239%*

 * *Differences: {"'names'": "{'Verbosity_Comparable': {'node': {'line': 93}}}"}*

```diff
@@ -650,15 +650,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.Verbosity_Comparable",
-                "line": 63,
+                "line": 93,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "su6.core.Verbosity",
                         "builtins.str",
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6/core.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6231601731601731%*

 * *Differences: {"'data_mtime'": '1685143685',*

 * * "'dep_lines'": '{insert: [(0, 101), (1, 491), (2, 5), (3, 6), (5, 29), (6, 43)], delete: [15, 10, '*

 * *                '9, 8, 7, 6, 5, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 20), (5, 5), (6, 5), (7, 5)], delete: [15, 11, 10, 9, 8, 7, '*

 * *                '6, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'typer.utils'), (2, 'sys'), (3, 'os'), "*

 * *                   "(5, 'typing_extensions'), (6, 'types'), (8, '_collections_abc')], delete: [14, "*

 * * […]*

```diff
@@ -1,67 +1,53 @@
 {
-    "data_mtime": 1685146214,
+    "data_mtime": 1685143685,
     "dep_lines": [
-        1,
-        2,
-        3,
-        4,
+        101,
+        491,
+        5,
+        6,
         7,
+        29,
+        43,
         1,
         1,
         1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        6
+        1
     ],
     "dep_prios": [
-        10,
-        10,
-        10,
+        5,
+        20,
         10,
         5,
         5,
+        5,
+        5,
+        5,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        5
+        30
     ],
     "dependencies": [
-        "enum",
-        "inspect",
-        "operator",
+        "collections.abc",
+        "typer.utils",
+        "sys",
+        "os",
         "typing",
-        "rich",
+        "typing_extensions",
+        "types",
         "builtins",
-        "_operator",
+        "_collections_abc",
         "_typeshed",
-        "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle",
-        "types",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "8b0663919c3c0dd90562c38fd1a1b39423b977de58b0bb1c6a616024d4d115d5",
-    "id": "su6.core",
-    "ignore_all": false,
-    "interface_hash": "d83c118a6138cd5f2f7af684c09b497dc10fc2eb27f9907feda828c7835bf8d4",
-    "mtime": 1685144281,
+    "hash": "1211bc8ebacfc892f46d646cc389f5e3793aa03da83de623e2c65f2b52adc389",
+    "id": "typer._typing",
+    "ignore_all": true,
+    "interface_hash": "0f3d3599045f3d24c61dcdc82fc0d7878684a5647fb9689d5be4c96189e04edc",
+    "mtime": 1685143295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -95,15 +81,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "./src/su6/core.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_typing.py",
     "plugin_data": null,
-    "size": 2823,
-    "suppressed": [
-        "plumbum.machines"
-    ],
+    "size": 19743,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6_checker/__about__.data.json` & `su6-0.3.0/.mypy_cache/3.11/su6_checker/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6_checker/__about__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/su6/__about__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7666666666666667%*

 * *Differences: {"'data_mtime'": '1685146214',*

 * * "'hash'": "'409ebf413db20f20687e9f62a8684ac69d9efa3eb9a1496f47fb651c0073dad7'",*

 * * "'id'": "'su6.__about__'",*

 * * "'interface_hash'": "'73c9ac79eb0b2bf75c6e787a1d921f977526fc73313e41372a43d62b6fc02d1d'",*

 * * "'mtime'": '1685282354',*

 * * "'path'": "'./src/su6/__about__.py'",*

 * * "'size'": '206'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1685143683,
+    "data_mtime": 1685146214,
     "dep_lines": [
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
@@ -11,19 +11,19 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "46e2988ae1702a50dd3052be264502bf790bc8ca34b94c10734f97eb9318bbbd",
-    "id": "su6_checker.__about__",
+    "hash": "409ebf413db20f20687e9f62a8684ac69d9efa3eb9a1496f47fb651c0073dad7",
+    "id": "su6.__about__",
     "ignore_all": false,
-    "interface_hash": "a79aa7369a97c75e7bfc1e2f3354408dc43aee52edbee9bbe45bc7e844e176b6",
-    "mtime": 1685144868,
+    "interface_hash": "73c9ac79eb0b2bf75c6e787a1d921f977526fc73313e41372a43d62b6fc02d1d",
+    "mtime": 1685282354,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "./src/su6_checker/__about__.py",
+    "path": "./src/su6/__about__.py",
     "plugin_data": null,
-    "size": 143,
+    "size": 206,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6_checker/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/su6_checker/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6_checker/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/su6_checker/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6_checker/cli.data.json` & `su6-0.3.0/.mypy_cache/3.11/su6_checker/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6_checker/cli.meta.json` & `su6-0.3.0/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6266638819270398%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 5), (2, 2), (3, 3), (5, 6), (6, 7), (7, 10)], delete: [12, 11, 6, '*

 * *                '5, 4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 5), (5, 5), (6, 5), (7, 5), (8, 5)], delete: [12, 11, 7, 6, 5, 4]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, '_ctypes'), (3, "*

 * *                   "'_typeshed'), (6, 'typing_extensions'), (7, 'types'), (8, 'builtins'), (9, "*

 * *                   "'array'), (10, 'mmap'), (11, 'pickle')], dele […]*

```diff
@@ -1,57 +1,56 @@
 {
-    "data_mtime": 1685143739,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        6,
+        5,
         1,
+        2,
+        3,
         4,
+        6,
+        7,
+        10,
         1,
         1,
         1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        3,
-        2
+        1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
+        5,
+        5,
+        5,
+        5,
+        5,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        5,
-        5
+        30
     ],
     "dependencies": [
-        "su6_checker.core",
-        "typer",
-        "rich",
-        "builtins",
+        "collections.abc",
+        "sys",
+        "_ctypes",
+        "_typeshed",
         "abc",
-        "click",
-        "click.core",
-        "enum",
-        "typer.core",
-        "typer.main",
-        "typing"
+        "typing",
+        "typing_extensions",
+        "types",
+        "builtins",
+        "array",
+        "mmap",
+        "pickle"
     ],
-    "hash": "cd18a4ff378eef9130e69d979763c8cee0daca13d45b2afbab68dafee4b20ca7",
-    "id": "su6_checker.cli",
-    "ignore_all": false,
-    "interface_hash": "3588acc0ff46745f90b61b8a8564c0d5c3a661f511418c007067a49e0009cefe",
-    "mtime": 1685144149,
+    "hash": "4e07f95e28e46e9d4c5eda8e3a693994b25ddc9e70955e59f569acc5472d3284",
+    "id": "ctypes",
+    "ignore_all": true,
+    "interface_hash": "258d6db8de019fc835a41737c0c96359c2e8e1c006da708ce31c5b3846725a76",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -85,16 +84,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "./src/su6_checker/cli.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi",
     "plugin_data": null,
-    "size": 2355,
-    "suppressed": [
-        "plumbum.commands.processes",
-        "plumbum"
-    ],
+    "size": 11646,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6_checker/core.data.json` & `su6-0.3.0/.mypy_cache/3.11/su6/cli.data.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8046957671957672%*

 * *Differences: {"'_fullname'": "'su6.cli'",*

 * * "'names'": "{'DEFAULT_VERBOSITY': {'cross_ref': 'su6.core.DEFAULT_VERBOSITY', 'module_hidden': "*

 * *            "True, 'module_public': False, delete: ['node']}, 'Verbosity': {'cross_ref': "*

 * *            "'su6.core.Verbosity', 'module_hidden': True, 'module_public': False, delete: "*

 * *            "['node']}, '__annotations__': {'node': {'fullname': 'su6.cli.__annotations__'}}, "*

 * *            "'__doc__': {'node': {'fullname': 'su6.cli.__doc__'}}, '__file__': {'node': "*

 * *            "{'f […]*

```diff
@@ -1,685 +1,320 @@
 {
     ".class": "MypyFile",
-    "_fullname": "su6_checker.core",
+    "_fullname": "su6.cli",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
+        "CommandNotFound": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false,
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_suppressed_import",
+                    "is_ready",
+                    "is_inferred"
+                ],
+                "fullname": "su6.cli.CommandNotFound",
+                "name": "CommandNotFound",
+                "type": {
+                    ".class": "AnyType",
+                    "missing_import_name": "su6.cli.CommandNotFound",
+                    "source_any": null,
+                    "type_of_any": 3
+                }
+            }
+        },
         "DEFAULT_VERBOSITY": {
             ".class": "SymbolTableNode",
+            "cross_ref": "su6.core.DEFAULT_VERBOSITY",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "EXIT_CODE_COMMAND_NOT_FOUND": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_ready",
+                    "is_inferred",
+                    "has_explicit_value"
+                ],
+                "fullname": "su6.cli.EXIT_CODE_COMMAND_NOT_FOUND",
+                "name": "EXIT_CODE_COMMAND_NOT_FOUND",
+                "type": "builtins.int"
+            }
+        },
+        "EXIT_CODE_ERROR": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_ready",
+                    "is_inferred",
+                    "has_explicit_value"
+                ],
+                "fullname": "su6.cli.EXIT_CODE_ERROR",
+                "name": "EXIT_CODE_ERROR",
+                "type": "builtins.int"
+            }
+        },
+        "EXIT_CODE_SUCCESS": {
+            ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
+                    "is_ready",
                     "is_inferred",
                     "has_explicit_value"
                 ],
-                "fullname": "su6_checker.core.DEFAULT_VERBOSITY",
-                "name": "DEFAULT_VERBOSITY",
-                "type": "su6_checker.core.Verbosity"
+                "fullname": "su6.cli.EXIT_CODE_SUCCESS",
+                "name": "EXIT_CODE_SUCCESS",
+                "type": "builtins.int"
             }
         },
-        "LocalCommand": {
+        "GREEN_CIRCLE": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_ready",
+                    "is_inferred",
+                    "has_explicit_value"
+                ],
+                "fullname": "su6.cli.GREEN_CIRCLE",
+                "name": "GREEN_CIRCLE",
+                "type": "builtins.str"
+            }
+        },
+        "ProcessExecutionError": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_suppressed_import",
                     "is_ready",
                     "is_inferred"
                 ],
-                "fullname": "su6_checker.core.LocalCommand",
-                "name": "LocalCommand",
+                "fullname": "su6.cli.ProcessExecutionError",
+                "name": "ProcessExecutionError",
                 "type": {
                     ".class": "AnyType",
-                    "missing_import_name": "su6_checker.core.LocalCommand",
+                    "missing_import_name": "su6.cli.ProcessExecutionError",
                     "source_any": null,
                     "type_of_any": 3
                 }
             }
         },
-        "Verbosity": {
+        "RED_CIRCLE": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "TypeInfo",
-                "_promote": [],
-                "abstract_attributes": [],
-                "alt_promote": null,
-                "bases": [
-                    "enum.Enum"
-                ],
-                "dataclass_transform_spec": null,
-                "declared_metaclass": null,
-                "defn": {
-                    ".class": "ClassDef",
-                    "fullname": "su6_checker.core.Verbosity",
-                    "name": "Verbosity",
-                    "type_vars": []
-                },
-                "deletable_attributes": [],
+                ".class": "Var",
                 "flags": [
-                    "is_enum"
-                ],
-                "fullname": "su6_checker.core.Verbosity",
-                "has_param_spec_type": false,
-                "metaclass_type": "enum.EnumMeta",
-                "metadata": {},
-                "module_name": "su6_checker.core",
-                "mro": [
-                    "su6_checker.core.Verbosity",
-                    "enum.Enum",
-                    "builtins.object"
+                    "is_ready",
+                    "is_inferred",
+                    "has_explicit_value"
                 ],
-                "names": {
-                    ".class": "SymbolTable",
-                    "__eq__": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0,
-                                0
-                            ],
-                            "arg_names": [
-                                null,
-                                null
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [],
-                            "fullname": "su6_checker.core.Verbosity.__eq__",
-                            "name": "__eq__",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0,
-                                    0
-                                ],
-                                "arg_names": [
-                                    null,
-                                    null
-                                ],
-                                "arg_types": [
-                                    "su6_checker.core.Verbosity",
-                                    {
-                                        ".class": "UnionType",
-                                        "items": [
-                                            "su6_checker.core.Verbosity",
-                                            "builtins.str",
-                                            "builtins.int",
-                                            "builtins.object"
-                                        ]
-                                    }
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": "self"
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "__eq__ of Verbosity",
-                                "ret_type": "builtins.bool",
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        }
-                    },
-                    "__ge__": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0,
-                                0
-                            ],
-                            "arg_names": [
-                                null,
-                                null
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [],
-                            "fullname": "su6_checker.core.Verbosity.__ge__",
-                            "name": "__ge__",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0,
-                                    0
-                                ],
-                                "arg_names": [
-                                    null,
-                                    null
-                                ],
-                                "arg_types": [
-                                    "su6_checker.core.Verbosity",
-                                    {
-                                        ".class": "TypeAliasType",
-                                        "args": [],
-                                        "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                    }
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": "self"
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "__ge__ of Verbosity",
-                                "ret_type": "builtins.bool",
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        }
-                    },
-                    "__gt__": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0,
-                                0
-                            ],
-                            "arg_names": [
-                                null,
-                                null
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [],
-                            "fullname": "su6_checker.core.Verbosity.__gt__",
-                            "name": "__gt__",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0,
-                                    0
-                                ],
-                                "arg_names": [
-                                    null,
-                                    null
-                                ],
-                                "arg_types": [
-                                    "su6_checker.core.Verbosity",
-                                    {
-                                        ".class": "TypeAliasType",
-                                        "args": [],
-                                        "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                    }
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": "self"
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "__gt__ of Verbosity",
-                                "ret_type": "builtins.bool",
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        }
-                    },
-                    "__hash__": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0
-                            ],
-                            "arg_names": [
-                                "self"
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [],
-                            "fullname": "su6_checker.core.Verbosity.__hash__",
-                            "name": "__hash__",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0
-                                ],
-                                "arg_names": [
-                                    "self"
-                                ],
-                                "arg_types": [
-                                    "su6_checker.core.Verbosity"
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": "self"
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "__hash__ of Verbosity",
-                                "ret_type": "builtins.int",
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        }
-                    },
-                    "__le__": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0,
-                                0
-                            ],
-                            "arg_names": [
-                                null,
-                                null
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [],
-                            "fullname": "su6_checker.core.Verbosity.__le__",
-                            "name": "__le__",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0,
-                                    0
-                                ],
-                                "arg_names": [
-                                    null,
-                                    null
-                                ],
-                                "arg_types": [
-                                    "su6_checker.core.Verbosity",
-                                    {
-                                        ".class": "TypeAliasType",
-                                        "args": [],
-                                        "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                    }
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": "self"
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "__le__ of Verbosity",
-                                "ret_type": "builtins.bool",
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        }
-                    },
-                    "__lt__": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0,
-                                0
-                            ],
-                            "arg_names": [
-                                null,
-                                null
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [],
-                            "fullname": "su6_checker.core.Verbosity.__lt__",
-                            "name": "__lt__",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0,
-                                    0
-                                ],
-                                "arg_names": [
-                                    null,
-                                    null
-                                ],
-                                "arg_types": [
-                                    "su6_checker.core.Verbosity",
-                                    {
-                                        ".class": "TypeAliasType",
-                                        "args": [],
-                                        "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                    }
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": "self"
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "__lt__ of Verbosity",
-                                "ret_type": "builtins.bool",
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        }
-                    },
-                    "_compare": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "Decorator",
-                            "func": {
-                                ".class": "FuncDef",
-                                "abstract_status": 0,
-                                "arg_kinds": [
-                                    0,
-                                    0,
-                                    0
-                                ],
-                                "arg_names": [
-                                    "self",
-                                    "other",
-                                    "_operator"
-                                ],
-                                "dataclass_transform_spec": null,
-                                "flags": [
-                                    "is_static",
-                                    "is_decorated"
-                                ],
-                                "fullname": "su6_checker.core.Verbosity._compare",
-                                "name": "_compare",
-                                "type": {
-                                    ".class": "CallableType",
-                                    "arg_kinds": [
-                                        0,
-                                        0,
-                                        0
-                                    ],
-                                    "arg_names": [
-                                        "self",
-                                        "other",
-                                        "_operator"
-                                    ],
-                                    "arg_types": [
-                                        "su6_checker.core.Verbosity",
-                                        {
-                                            ".class": "TypeAliasType",
-                                            "args": [],
-                                            "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                        },
-                                        {
-                                            ".class": "CallableType",
-                                            "arg_kinds": [
-                                                0,
-                                                0
-                                            ],
-                                            "arg_names": [
-                                                null,
-                                                null
-                                            ],
-                                            "arg_types": [
-                                                {
-                                                    ".class": "TypeAliasType",
-                                                    "args": [],
-                                                    "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                                },
-                                                {
-                                                    ".class": "TypeAliasType",
-                                                    "args": [],
-                                                    "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                                }
-                                            ],
-                                            "bound_args": [],
-                                            "def_extras": {},
-                                            "fallback": "builtins.function",
-                                            "from_concatenate": false,
-                                            "implicit": false,
-                                            "is_ellipsis_args": false,
-                                            "name": null,
-                                            "ret_type": "builtins.bool",
-                                            "type_guard": null,
-                                            "unpack_kwargs": false,
-                                            "variables": []
-                                        }
-                                    ],
-                                    "bound_args": [],
-                                    "def_extras": {
-                                        "first_arg": null
-                                    },
-                                    "fallback": "builtins.function",
-                                    "from_concatenate": false,
-                                    "implicit": false,
-                                    "is_ellipsis_args": false,
-                                    "name": "_compare of Verbosity",
-                                    "ret_type": "builtins.bool",
-                                    "type_guard": null,
-                                    "unpack_kwargs": false,
-                                    "variables": []
-                                }
-                            },
-                            "is_overload": false,
-                            "var": {
-                                ".class": "Var",
-                                "flags": [
-                                    "is_initialized_in_class",
-                                    "is_staticmethod",
-                                    "is_ready",
-                                    "is_inferred"
-                                ],
-                                "fullname": "su6_checker.core.Verbosity._compare",
-                                "name": "_compare",
-                                "type": {
-                                    ".class": "CallableType",
-                                    "arg_kinds": [
-                                        0,
-                                        0,
-                                        0
-                                    ],
-                                    "arg_names": [
-                                        "self",
-                                        "other",
-                                        "_operator"
-                                    ],
-                                    "arg_types": [
-                                        "su6_checker.core.Verbosity",
-                                        {
-                                            ".class": "TypeAliasType",
-                                            "args": [],
-                                            "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                        },
-                                        {
-                                            ".class": "CallableType",
-                                            "arg_kinds": [
-                                                0,
-                                                0
-                                            ],
-                                            "arg_names": [
-                                                null,
-                                                null
-                                            ],
-                                            "arg_types": [
-                                                {
-                                                    ".class": "TypeAliasType",
-                                                    "args": [],
-                                                    "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                                },
-                                                {
-                                                    ".class": "TypeAliasType",
-                                                    "args": [],
-                                                    "type_ref": "su6_checker.core.Verbosity_Comparable"
-                                                }
-                                            ],
-                                            "bound_args": [],
-                                            "def_extras": {},
-                                            "fallback": "builtins.function",
-                                            "from_concatenate": false,
-                                            "implicit": false,
-                                            "is_ellipsis_args": false,
-                                            "name": null,
-                                            "ret_type": "builtins.bool",
-                                            "type_guard": null,
-                                            "unpack_kwargs": false,
-                                            "variables": []
-                                        }
-                                    ],
-                                    "bound_args": [],
-                                    "def_extras": {
-                                        "first_arg": null
-                                    },
-                                    "fallback": "builtins.function",
-                                    "from_concatenate": false,
-                                    "implicit": false,
-                                    "is_ellipsis_args": false,
-                                    "name": "_compare of Verbosity",
-                                    "ret_type": "builtins.bool",
-                                    "type_guard": null,
-                                    "unpack_kwargs": false,
-                                    "variables": []
-                                }
-                            }
-                        }
-                    },
-                    "normal": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_initialized_in_class",
-                                "is_final",
-                                "is_ready",
-                                "is_inferred",
-                                "has_explicit_value"
-                            ],
-                            "fullname": "su6_checker.core.Verbosity.normal",
-                            "name": "normal",
-                            "type": {
-                                ".class": "Instance",
-                                "args": [],
-                                "last_known_value": {
-                                    ".class": "LiteralType",
-                                    "fallback": "builtins.str",
-                                    "value": "2"
-                                },
-                                "type_ref": "builtins.str"
-                            }
-                        }
-                    },
-                    "quiet": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_initialized_in_class",
-                                "is_final",
-                                "is_ready",
-                                "is_inferred",
-                                "has_explicit_value"
-                            ],
-                            "fullname": "su6_checker.core.Verbosity.quiet",
-                            "name": "quiet",
-                            "type": {
-                                ".class": "Instance",
-                                "args": [],
-                                "last_known_value": {
-                                    ".class": "LiteralType",
-                                    "fallback": "builtins.str",
-                                    "value": "1"
-                                },
-                                "type_ref": "builtins.str"
-                            }
+                "fullname": "su6.cli.RED_CIRCLE",
+                "name": "RED_CIRCLE",
+                "type": "builtins.str"
+            }
+        },
+        "T_Command": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeAlias",
+                "alias_tvars": [],
+                "column": 0,
+                "fullname": "su6.cli.T_Command",
+                "line": 56,
+                "no_args": false,
+                "normalized": false,
+                "target": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        2,
+                        4
+                    ],
+                    "arg_names": [
+                        null,
+                        null
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 6
+                        },
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 6
                         }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {},
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": true,
+                    "name": null,
+                    "ret_type": {
+                        ".class": "UnionType",
+                        "items": [
+                            "builtins.bool",
+                            "builtins.int"
+                        ]
                     },
-                    "verbose": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_initialized_in_class",
-                                "is_final",
-                                "is_ready",
-                                "is_inferred",
-                                "has_explicit_value"
-                            ],
-                            "fullname": "su6_checker.core.Verbosity.verbose",
-                            "name": "verbose",
-                            "type": {
-                                ".class": "Instance",
-                                "args": [],
-                                "last_known_value": {
-                                    ".class": "LiteralType",
-                                    "fallback": "builtins.str",
-                                    "value": "3"
-                                },
-                                "type_ref": "builtins.str"
-                            }
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "T_Inner_Wrapper": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeAlias",
+                "alias_tvars": [],
+                "column": 0,
+                "fullname": "su6.cli.T_Inner_Wrapper",
+                "line": 58,
+                "no_args": false,
+                "normalized": false,
+                "target": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        2,
+                        4
+                    ],
+                    "arg_names": [
+                        null,
+                        null
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 6
+                        },
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 6
                         }
-                    }
-                },
-                "self_type": null,
-                "slots": null,
-                "tuple_type": null,
-                "type_vars": [],
-                "typeddict_type": null
+                    ],
+                    "bound_args": [],
+                    "def_extras": {},
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": true,
+                    "name": null,
+                    "ret_type": "builtins.int",
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
             }
         },
-        "Verbosity_Comparable": {
+        "T_Outer_Wrapper": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
-                "fullname": "su6_checker.core.Verbosity_Comparable",
-                "line": 63,
+                "fullname": "su6.cli.T_Outer_Wrapper",
+                "line": 61,
                 "no_args": false,
                 "normalized": false,
                 "target": {
-                    ".class": "UnionType",
-                    "items": [
-                        "su6_checker.core.Verbosity",
-                        "builtins.str",
-                        "builtins.int"
-                    ]
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0
+                    ],
+                    "arg_names": [
+                        null
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "TypeAliasType",
+                            "args": [],
+                            "type_ref": "su6.cli.T_Command"
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {},
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": null,
+                    "ret_type": {
+                        ".class": "TypeAliasType",
+                        "args": [],
+                        "type_ref": "su6.cli.T_Inner_Wrapper"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
                 }
             }
         },
+        "Verbosity": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "su6.core.Verbosity",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "YELLOW_CIRCLE": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_ready",
+                    "is_inferred",
+                    "has_explicit_value"
+                ],
+                "fullname": "su6.cli.YELLOW_CIRCLE",
+                "name": "YELLOW_CIRCLE",
+                "type": "builtins.str"
+            }
+        },
         "__annotations__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6_checker.core.__annotations__",
+                "fullname": "su6.cli.__annotations__",
                 "name": "__annotations__",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
                             ".class": "AnyType",
@@ -696,335 +331,1003 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6_checker.core.__doc__",
+                "fullname": "su6.cli.__doc__",
                 "name": "__doc__",
                 "type": "builtins.str"
             }
         },
         "__file__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6_checker.core.__file__",
+                "fullname": "su6.cli.__file__",
                 "name": "__file__",
                 "type": "builtins.str"
             }
         },
         "__name__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6_checker.core.__name__",
+                "fullname": "su6.cli.__name__",
                 "name": "__name__",
                 "type": "builtins.str"
             }
         },
         "__package__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6_checker.core.__package__",
+                "fullname": "su6.cli.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
-        "danger": {
+        "_check_tool": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
-                    2
+                    0,
+                    2,
+                    5
                 ],
                 "arg_names": [
-                    "args"
+                    "tool",
+                    "args",
+                    "verbosity"
                 ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "su6_checker.core.danger",
-                "name": "danger",
+                "fullname": "su6.cli._check_tool",
+                "name": "_check_tool",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
-                        2
+                        0,
+                        2,
+                        5
                     ],
                     "arg_names": [
-                        "args"
+                        "tool",
+                        "args",
+                        "verbosity"
                     ],
                     "arg_types": [
-                        "builtins.str"
+                        "builtins.str",
+                        "builtins.str",
+                        "su6.core.Verbosity"
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "danger",
-                    "ret_type": {
-                        ".class": "NoneType"
-                    },
+                    "name": "_check_tool",
+                    "ret_type": "builtins.int",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "enum": {
+        "app": {
             ".class": "SymbolTableNode",
-            "cross_ref": "enum",
             "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_inferred",
+                    "has_explicit_value"
+                ],
+                "fullname": "su6.cli.app",
+                "name": "app",
+                "type": "typer.main.Typer"
+            }
         },
-        "info": {
+        "bandit": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    2
-                ],
-                "arg_names": [
-                    "args"
-                ],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "su6_checker.core.info",
-                "name": "info",
-                "type": {
-                    ".class": "CallableType",
+                ".class": "Decorator",
+                "func": {
+                    ".class": "FuncDef",
+                    "abstract_status": 0,
                     "arg_kinds": [
-                        2
+                        1
                     ],
                     "arg_names": [
-                        "args"
+                        "verbosity"
                     ],
-                    "arg_types": [
-                        "builtins.str"
+                    "dataclass_transform_spec": null,
+                    "flags": [
+                        "is_decorated"
                     ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "info",
-                    "ret_type": {
-                        ".class": "NoneType"
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
+                    "fullname": "su6.cli.bandit",
+                    "name": "bandit",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            1
+                        ],
+                        "arg_names": [
+                            "verbosity"
+                        ],
+                        "arg_types": [
+                            "su6.core.Verbosity"
+                        ],
+                        "bound_args": [],
+                        "def_extras": {
+                            "first_arg": null
+                        },
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": false,
+                        "name": "bandit",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                },
+                "is_overload": false,
+                "var": {
+                    ".class": "Var",
+                    "flags": [
+                        "is_ready",
+                        "is_inferred"
+                    ],
+                    "fullname": "su6.cli.bandit",
+                    "name": "bandit",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            2,
+                            4
+                        ],
+                        "arg_names": [
+                            null,
+                            null
+                        ],
+                        "arg_types": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            }
+                        ],
+                        "bound_args": [],
+                        "def_extras": {},
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": true,
+                        "name": "bandit",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                }
+            }
+        },
+        "black": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Decorator",
+                "func": {
+                    ".class": "FuncDef",
+                    "abstract_status": 0,
+                    "arg_kinds": [
+                        1,
+                        1
+                    ],
+                    "arg_names": [
+                        "fix",
+                        "verbosity"
+                    ],
+                    "dataclass_transform_spec": null,
+                    "flags": [
+                        "is_decorated"
+                    ],
+                    "fullname": "su6.cli.black",
+                    "name": "black",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            1,
+                            1
+                        ],
+                        "arg_names": [
+                            "fix",
+                            "verbosity"
+                        ],
+                        "arg_types": [
+                            "builtins.bool",
+                            "su6.core.Verbosity"
+                        ],
+                        "bound_args": [],
+                        "def_extras": {
+                            "first_arg": null
+                        },
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": false,
+                        "name": "black",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                },
+                "is_overload": false,
+                "var": {
+                    ".class": "Var",
+                    "flags": [
+                        "is_ready",
+                        "is_inferred"
+                    ],
+                    "fullname": "su6.cli.black",
+                    "name": "black",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            2,
+                            4
+                        ],
+                        "arg_names": [
+                            null,
+                            null
+                        ],
+                        "arg_types": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            }
+                        ],
+                        "bound_args": [],
+                        "def_extras": {},
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": true,
+                        "name": "black",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                }
+            }
+        },
+        "check_all": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Decorator",
+                "func": {
+                    ".class": "FuncDef",
+                    "abstract_status": 0,
+                    "arg_kinds": [
+                        1,
+                        1
+                    ],
+                    "arg_names": [
+                        "ignore_uninstalled",
+                        "verbosity"
+                    ],
+                    "dataclass_transform_spec": null,
+                    "flags": [
+                        "is_decorated"
+                    ],
+                    "fullname": "su6.cli.check_all",
+                    "name": "check_all",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            1,
+                            1
+                        ],
+                        "arg_names": [
+                            "ignore_uninstalled",
+                            "verbosity"
+                        ],
+                        "arg_types": [
+                            "builtins.bool",
+                            "su6.core.Verbosity"
+                        ],
+                        "bound_args": [],
+                        "def_extras": {
+                            "first_arg": null
+                        },
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": false,
+                        "name": "check_all",
+                        "ret_type": "builtins.bool",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                },
+                "is_overload": false,
+                "var": {
+                    ".class": "Var",
+                    "flags": [
+                        "is_ready",
+                        "is_inferred"
+                    ],
+                    "fullname": "su6.cli.check_all",
+                    "name": "check_all",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            2,
+                            4
+                        ],
+                        "arg_names": [
+                            null,
+                            null
+                        ],
+                        "arg_types": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            }
+                        ],
+                        "bound_args": [],
+                        "def_extras": {},
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": true,
+                        "name": "check_all",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
                 }
             }
         },
-        "inspect": {
+        "do_fix": {
             ".class": "SymbolTableNode",
-            "cross_ref": "inspect",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Decorator",
+                "func": {
+                    ".class": "FuncDef",
+                    "abstract_status": 0,
+                    "arg_kinds": [
+                        1
+                    ],
+                    "arg_names": [
+                        "verbosity"
+                    ],
+                    "dataclass_transform_spec": null,
+                    "flags": [
+                        "is_decorated"
+                    ],
+                    "fullname": "su6.cli.do_fix",
+                    "name": "do_fix",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            1
+                        ],
+                        "arg_names": [
+                            "verbosity"
+                        ],
+                        "arg_types": [
+                            "su6.core.Verbosity"
+                        ],
+                        "bound_args": [],
+                        "def_extras": {
+                            "first_arg": null
+                        },
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": false,
+                        "name": "do_fix",
+                        "ret_type": "builtins.bool",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                },
+                "is_overload": false,
+                "var": {
+                    ".class": "Var",
+                    "flags": [
+                        "is_ready",
+                        "is_inferred"
+                    ],
+                    "fullname": "su6.cli.do_fix",
+                    "name": "do_fix",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            2,
+                            4
+                        ],
+                        "arg_names": [
+                            null,
+                            null
+                        ],
+                        "arg_types": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            }
+                        ],
+                        "bound_args": [],
+                        "def_extras": {},
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": true,
+                        "name": "do_fix",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                }
+            }
+        },
+        "functools": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "functools",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "log_cmd_output": {
+        "info": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "su6.core.info",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "isort": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0,
-                    0
-                ],
-                "arg_names": [
-                    "stdout",
-                    "stderr"
-                ],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "su6_checker.core.log_cmd_output",
-                "name": "log_cmd_output",
-                "type": {
-                    ".class": "CallableType",
+                ".class": "Decorator",
+                "func": {
+                    ".class": "FuncDef",
+                    "abstract_status": 0,
                     "arg_kinds": [
-                        0,
-                        0
+                        1,
+                        1
                     ],
                     "arg_names": [
-                        "stdout",
-                        "stderr"
+                        "fix",
+                        "verbosity"
                     ],
-                    "arg_types": [
-                        "builtins.str",
-                        "builtins.str"
+                    "dataclass_transform_spec": null,
+                    "flags": [
+                        "is_decorated"
                     ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "log_cmd_output",
-                    "ret_type": {
-                        ".class": "NoneType"
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
+                    "fullname": "su6.cli.isort",
+                    "name": "isort",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            1,
+                            1
+                        ],
+                        "arg_names": [
+                            "fix",
+                            "verbosity"
+                        ],
+                        "arg_types": [
+                            "builtins.bool",
+                            "su6.core.Verbosity"
+                        ],
+                        "bound_args": [],
+                        "def_extras": {
+                            "first_arg": null
+                        },
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": false,
+                        "name": "isort",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                },
+                "is_overload": false,
+                "var": {
+                    ".class": "Var",
+                    "flags": [
+                        "is_ready",
+                        "is_inferred"
+                    ],
+                    "fullname": "su6.cli.isort",
+                    "name": "isort",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            2,
+                            4
+                        ],
+                        "arg_names": [
+                            null,
+                            null
+                        ],
+                        "arg_types": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            }
+                        ],
+                        "bound_args": [],
+                        "def_extras": {},
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": true,
+                        "name": "isort",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
                 }
             }
         },
-        "log_command": {
+        "local": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false,
             "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0,
-                    0
-                ],
-                "arg_names": [
-                    "command",
-                    "args"
+                ".class": "Var",
+                "flags": [
+                    "is_suppressed_import",
+                    "is_ready",
+                    "is_inferred"
                 ],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "su6_checker.core.log_command",
-                "name": "log_command",
+                "fullname": "su6.cli.local",
+                "name": "local",
                 "type": {
-                    ".class": "CallableType",
+                    ".class": "AnyType",
+                    "missing_import_name": "su6.cli.local",
+                    "source_any": null,
+                    "type_of_any": 3
+                }
+            }
+        },
+        "log_cmd_output": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "su6.core.log_cmd_output",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "log_command": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "su6.core.log_command",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "mypy": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Decorator",
+                "func": {
+                    ".class": "FuncDef",
+                    "abstract_status": 0,
                     "arg_kinds": [
-                        0,
-                        0
+                        1
                     ],
                     "arg_names": [
-                        "command",
-                        "args"
+                        "verbosity"
                     ],
-                    "arg_types": [
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": "su6_checker.core.LocalCommand",
-                            "source_any": null,
-                            "type_of_any": 3
+                    "dataclass_transform_spec": null,
+                    "flags": [
+                        "is_decorated"
+                    ],
+                    "fullname": "su6.cli.mypy",
+                    "name": "mypy",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            1
+                        ],
+                        "arg_names": [
+                            "verbosity"
+                        ],
+                        "arg_types": [
+                            "su6.core.Verbosity"
+                        ],
+                        "bound_args": [],
+                        "def_extras": {
+                            "first_arg": null
                         },
-                        {
-                            ".class": "Instance",
-                            "args": [
-                                "builtins.str"
-                            ],
-                            "type_ref": "typing.Iterable"
-                        }
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": false,
+                        "name": "mypy",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                },
+                "is_overload": false,
+                "var": {
+                    ".class": "Var",
+                    "flags": [
+                        "is_ready",
+                        "is_inferred"
                     ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "log_command",
-                    "ret_type": {
-                        ".class": "NoneType"
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
+                    "fullname": "su6.cli.mypy",
+                    "name": "mypy",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            2,
+                            4
+                        ],
+                        "arg_names": [
+                            null,
+                            null
+                        ],
+                        "arg_types": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            }
+                        ],
+                        "bound_args": [],
+                        "def_extras": {},
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": true,
+                        "name": "mypy",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
                 }
             }
         },
-        "operator": {
+        "print": {
             ".class": "SymbolTableNode",
-            "cross_ref": "operator",
+            "cross_ref": "rich.print",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "print": {
+        "pydocstyle": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Decorator",
+                "func": {
+                    ".class": "FuncDef",
+                    "abstract_status": 0,
+                    "arg_kinds": [
+                        1
+                    ],
+                    "arg_names": [
+                        "verbosity"
+                    ],
+                    "dataclass_transform_spec": null,
+                    "flags": [
+                        "is_decorated"
+                    ],
+                    "fullname": "su6.cli.pydocstyle",
+                    "name": "pydocstyle",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            1
+                        ],
+                        "arg_names": [
+                            "verbosity"
+                        ],
+                        "arg_types": [
+                            "su6.core.Verbosity"
+                        ],
+                        "bound_args": [],
+                        "def_extras": {
+                            "first_arg": null
+                        },
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": false,
+                        "name": "pydocstyle",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                },
+                "is_overload": false,
+                "var": {
+                    ".class": "Var",
+                    "flags": [
+                        "is_ready",
+                        "is_inferred"
+                    ],
+                    "fullname": "su6.cli.pydocstyle",
+                    "name": "pydocstyle",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            2,
+                            4
+                        ],
+                        "arg_names": [
+                            null,
+                            null
+                        ],
+                        "arg_types": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            }
+                        ],
+                        "bound_args": [],
+                        "def_extras": {},
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": true,
+                        "name": "pydocstyle",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                }
+            }
+        },
+        "ruff": {
             ".class": "SymbolTableNode",
-            "cross_ref": "rich.print",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Decorator",
+                "func": {
+                    ".class": "FuncDef",
+                    "abstract_status": 0,
+                    "arg_kinds": [
+                        1
+                    ],
+                    "arg_names": [
+                        "verbosity"
+                    ],
+                    "dataclass_transform_spec": null,
+                    "flags": [
+                        "is_decorated"
+                    ],
+                    "fullname": "su6.cli.ruff",
+                    "name": "ruff",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            1
+                        ],
+                        "arg_names": [
+                            "verbosity"
+                        ],
+                        "arg_types": [
+                            "su6.core.Verbosity"
+                        ],
+                        "bound_args": [],
+                        "def_extras": {
+                            "first_arg": null
+                        },
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": false,
+                        "name": "ruff",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                },
+                "is_overload": false,
+                "var": {
+                    ".class": "Var",
+                    "flags": [
+                        "is_ready",
+                        "is_inferred"
+                    ],
+                    "fullname": "su6.cli.ruff",
+                    "name": "ruff",
+                    "type": {
+                        ".class": "CallableType",
+                        "arg_kinds": [
+                            2,
+                            4
+                        ],
+                        "arg_names": [
+                            null,
+                            null
+                        ],
+                        "arg_types": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            }
+                        ],
+                        "bound_args": [],
+                        "def_extras": {},
+                        "fallback": "builtins.function",
+                        "from_concatenate": false,
+                        "implicit": false,
+                        "is_ellipsis_args": true,
+                        "name": "ruff",
+                        "ret_type": "builtins.int",
+                        "type_guard": null,
+                        "unpack_kwargs": false,
+                        "variables": []
+                    }
+                }
+            }
+        },
+        "typer": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typer",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
         "typing": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
         "warn": {
             ".class": "SymbolTableNode",
+            "cross_ref": "su6.core.warn",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "with_exit_code": {
+            ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
-                "arg_kinds": [
-                    2
-                ],
-                "arg_names": [
-                    "args"
-                ],
+                "arg_kinds": [],
+                "arg_names": [],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "su6_checker.core.warn",
-                "name": "warn",
+                "fullname": "su6.cli.with_exit_code",
+                "name": "with_exit_code",
                 "type": {
                     ".class": "CallableType",
-                    "arg_kinds": [
-                        2
-                    ],
-                    "arg_names": [
-                        "args"
-                    ],
-                    "arg_types": [
-                        "builtins.str"
-                    ],
+                    "arg_kinds": [],
+                    "arg_names": [],
+                    "arg_types": [],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "warn",
+                    "name": "with_exit_code",
                     "ret_type": {
-                        ".class": "NoneType"
+                        ".class": "TypeAliasType",
+                        "args": [],
+                        "type_ref": "su6.cli.T_Outer_Wrapper"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         }
     },
-    "path": "./src/su6_checker/core.py"
+    "path": "./src/su6/cli.py"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/su6_checker/core.meta.json` & `su6-0.3.0/.mypy_cache/3.11/su6/core.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7533333333333334%*

 * *Differences: {"'data_mtime'": '1685283595',*

 * * "'dep_lines'": '{insert: [(1, 5), (2, 6), (4, 10), (15, 9)], delete: [15, 2, 1, 0]}',*

 * * "'hash'": "'9ded4b5f40265a3805292f9cab436f3f18d449ae6fc87c312cc5fe0463329b0e'",*

 * * "'id'": "'su6.core'",*

 * * "'interface_hash'": "'6e59916014e397105823da62e237450511094a806cc212dfecd8b7c68cb27eff'",*

 * * "'mtime'": '1685282963',*

 * * "'path'": "'./src/su6/core.py'",*

 * * "'size'": '3967'}*

```diff
@@ -1,26 +1,26 @@
 {
-    "data_mtime": 1685143739,
+    "data_mtime": 1685283595,
     "dep_lines": [
-        1,
-        2,
-        3,
         4,
+        5,
+        6,
         7,
+        10,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        6
+        9
     ],
     "dep_prios": [
         10,
         10,
         10,
         10,
         5,
@@ -49,19 +49,19 @@
         "array",
         "ctypes",
         "mmap",
         "pickle",
         "types",
         "typing_extensions"
     ],
-    "hash": "8b0663919c3c0dd90562c38fd1a1b39423b977de58b0bb1c6a616024d4d115d5",
-    "id": "su6_checker.core",
+    "hash": "9ded4b5f40265a3805292f9cab436f3f18d449ae6fc87c312cc5fe0463329b0e",
+    "id": "su6.core",
     "ignore_all": false,
-    "interface_hash": "b0b2dfd0a37866e3640371d6d066f122b1a7cc5ee332534e093bf5707d163a85",
-    "mtime": 1685144281,
+    "interface_hash": "6e59916014e397105823da62e237450511094a806cc212dfecd8b7c68cb27eff",
+    "mtime": 1685282963,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -95,15 +95,15 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "./src/su6_checker/core.py",
+    "path": "./src/su6/core.py",
     "plugin_data": null,
-    "size": 2823,
+    "size": 3967,
     "suppressed": [
         "plumbum.machines"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/tests/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/tests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/tests/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/uuid.meta.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6939393939393939%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 1), (1, 2), (2, 3), (3, 4), (4, 1), (5, 1), (6, 1), (7, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5), (2, 5), (3, 5), (5, 30), (6, 30), (7, 30), (8, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (1, '_typeshed'), (2, 'enum'), (3, 'typing_extensions'), "*

 * *                   "(6, 'array'), (7, 'ctypes'), (8, 'mmap'), (9, 'pickle')]}",*

 * * "'hash'": "'8c28006bde3a41ef255422bf6626035a62a8e9edaf430622e7f05e329a3c422e'",*

 * * "'id'": "'uuid'",*

 * * "'ignore_all'": 'True',*

 * * "'interface_ […]*

```diff
@@ -1,29 +1,53 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
         1,
+        2,
+        3,
+        4,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
         5,
+        5,
+        5,
+        30,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
+        "sys",
+        "_typeshed",
+        "enum",
+        "typing_extensions",
         "builtins",
         "abc",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle",
         "typing"
     ],
-    "hash": "9cb95505c34a091a9b6468d522af11f6aaf9c74162ad95203ed31ec0b221f000",
-    "id": "tests",
-    "ignore_all": false,
-    "interface_hash": "21c07076089f75f20122c2c5361d5ecfde47ebd323b9d3a43f203539bfaaa50f",
-    "mtime": 1685143094,
+    "hash": "8c28006bde3a41ef255422bf6626035a62a8e9edaf430622e7f05e329a3c422e",
+    "id": "uuid",
+    "ignore_all": true,
+    "interface_hash": "68be08b7157d0b400fe2a32ba2ffd7e27aaf1bf6bcd798739b799c9e5dc737c6",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +81,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "./tests/__init__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/uuid.pyi",
     "plugin_data": null,
-    "size": 121,
+    "size": 2558,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/time.meta.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6964357864357865%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(1, 2), (2, 3), (3, 4)], delete: [7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [9, 4, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (1, '_typeshed'), (2, 'typing'), (3, "*

 * *                   "'typing_extensions')], delete: [10, 7, 6, 5, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'81ee1e52c98cc1cd26d7a6aa6d5a9c23d100b4e14cdd725b405a720187e41f8c'",*

 * * "'id'": "'time'",*

 * * "'interface_hash'": "'7816257c61ae61d9828ffbe5f5b912a849465f4aabae1d902ea98aeb326be […]*

```diff
@@ -1,53 +1,38 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        7,
-        10,
-        22,
-        29,
-        30,
-        32,
-        38,
-        5,
         1,
+        2,
+        3,
+        4,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        5,
-        5,
         10,
         5,
         5,
         5,
         5,
-        5,
-        30,
         30
     ],
     "dependencies": [
-        "click.exceptions",
-        "click.termui",
-        "click.utils",
-        "typer.colors",
-        "typer.main",
-        "typer.models",
-        "typer.params",
-        "shutil",
+        "sys",
+        "_typeshed",
+        "typing",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "c5ff549135bc942c56bd006b25e9430d11aca40c240e6d2f7762a28e11ea3f28",
-    "id": "typer",
+    "hash": "81ee1e52c98cc1cd26d7a6aa6d5a9c23d100b4e14cdd725b405a720187e41f8c",
+    "id": "time",
     "ignore_all": true,
-    "interface_hash": "77eb44dfcf25f13187d20d29aaf6cb48eded4dc38ac76aa831bd663abd45a61b",
-    "mtime": 1685143295,
+    "interface_hash": "7816257c61ae61d9828ffbe5f5b912a849465f4aabae1d902ea98aeb326bea5b",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -81,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/__init__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/time.pyi",
     "plugin_data": null,
-    "size": 1602,
+    "size": 3663,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_compat_utils.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `su6-0.3.0/.mypy_cache/3.11/termios.meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6897435897435897%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(1, 2), (2, 3), (3, 4)], delete: [6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 5), (3, 5), (4, 5)], delete: [8, 7, 6, 5, 4, 3, 2]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (4, 'builtins'), (5, 'abc')], delete: [7, 6, 5, 4, 3, 1, "*

 * *                   '0]}',*

 * * "'hash'": "'2f0f08844c903b2aa786d04a8a488242c21b5912f570b5db810e5afc7ec29ba9'",*

 * * "'id'": "'termios'",*

 * * "'interface_hash'": "'6949464470ae855c517f57f5cd7944fe547de71b372e20a351af08f190 […]*

```diff
@@ -1,50 +1,38 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
         1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
+        2,
+        3,
+        4,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
+        5,
+        5,
+        5,
         30
     ],
     "dependencies": [
-        "click",
-        "builtins",
+        "sys",
         "_typeshed",
-        "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle",
         "typing",
-        "typing_extensions"
+        "typing_extensions",
+        "builtins",
+        "abc"
     ],
-    "hash": "929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a",
-    "id": "typer._compat_utils",
+    "hash": "2f0f08844c903b2aa786d04a8a488242c21b5912f570b5db810e5afc7ec29ba9",
+    "id": "termios",
     "ignore_all": true,
-    "interface_hash": "f13939f83ff3c74c0b399e38a0f09049771195ed55e4e7d096d0f5225ca3996b",
-    "mtime": 1685143295,
+    "interface_hash": "6949464470ae855c517f57f5cd7944fe547de71b372e20a351af08f190f9884f",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -78,13 +66,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_compat_utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/termios.pyi",
     "plugin_data": null,
-    "size": 94,
+    "size": 5095,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_completion_click7.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_completion_click7.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_completion_click7.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_completion_click7.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_completion_click8.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_completion_click8.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_completion_click8.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_completion_click8.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_completion_shared.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `su6-0.3.0/.mypy_cache/3.11/shutil.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6617918313570487%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 4)], delete: [20, 17, 16, 15, 14, 13, 12, 11, 10, 9, 8, 7, 6, 3]}',*

 * * "'dep_prios'": '{insert: [(0, 5)], delete: [20, 18, 17, 16, 15, 14, 13, 12, 11, 10, 9, 7, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (3, '_typeshed'), (5, 'typing_extensions')], "*

 * *                   'delete: [19, 18, 17, 16, 15, 14, 13, 12, 11, 10, 7, 5, 4, 2, 1]}',*

 * * "'hash'": "'14a2bb451d6170f6e211ac293eed7182c2d925a35b3c28b0bb5509c21bf1a000'",*

 * * "'id'": "'sh […]*

```diff
@@ -1,82 +1,44 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
+        4,
         1,
         2,
         3,
-        4,
         5,
         6,
-        7,
-        9,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
         1,
-        1,
-        1,
-        1,
-        1,
-        12
+        1
     ],
     "dep_prios": [
-        10,
-        10,
+        5,
         10,
         10,
         5,
         5,
         5,
-        10,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        10
+        30
     ],
     "dependencies": [
+        "collections.abc",
         "os",
-        "re",
-        "subprocess",
         "sys",
-        "enum",
-        "pathlib",
+        "_typeshed",
         "typing",
-        "click",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "array",
-        "click.core",
-        "click.exceptions",
-        "click.globals",
-        "click.utils",
-        "ctypes",
-        "io",
-        "mmap",
-        "pickle",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "07d57ab9af0bc9668092450a3be34d73bbc19793d036b5b9a1366b0434c02eb8",
-    "id": "typer._completion_shared",
+    "hash": "14a2bb451d6170f6e211ac293eed7182c2d925a35b3c28b0bb5509c21bf1a000",
+    "id": "shutil",
     "ignore_all": true,
-    "interface_hash": "8a2072c243e4201d8048e9c080be92b7fb7bf1f0af99bbcca8e61271fd19a2af",
-    "mtime": 1685143295,
+    "interface_hash": "57656da15158dbdecfaa2bfd4ddccf69e5796d41dc9c0e81fc787cb985d96f80",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -110,15 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_completion_shared.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/shutil.pyi",
     "plugin_data": null,
-    "size": 8541,
-    "suppressed": [
-        "shellingham"
-    ],
+    "size": 6658,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_typing.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/_typing.meta.json` & `su6-0.3.0/.mypy_cache/3.11/array.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7183333333333334%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 3), (1, 1), (2, 2), (5, 1)], delete: [6, 5, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(6, 30)], delete: [3, 1]}',*

 * * "'dependencies'": "{insert: [(2, '_typeshed'), (7, 'ctypes'), (8, 'mmap'), (9, 'pickle')], "*

 * *                   'delete: [9, 8, 6, 3, 1]}',*

 * * "'hash'": "'857e937ecf94979d69f776505b3837900fb0898aee25681aec6aecea918cecf7'",*

 * * "'id'": "'array'",*

 * * "'interface_hash'": "'e74f43bcf6812ded0e30399199d4635c9bc9566bf7e4a36c46596db0efe00fdd'",*

 * * "'mti […]*

```diff
@@ -1,53 +1,50 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        101,
-        491,
-        5,
+        3,
+        1,
+        2,
         6,
         7,
-        29,
-        43,
+        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        20,
         10,
         5,
         5,
         5,
         5,
-        5,
+        30,
         30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "typer.utils",
         "sys",
-        "os",
+        "_typeshed",
         "typing",
         "typing_extensions",
-        "types",
         "builtins",
-        "_collections_abc",
-        "_typeshed",
-        "abc"
+        "abc",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "1211bc8ebacfc892f46d646cc389f5e3793aa03da83de623e2c65f2b52adc389",
-    "id": "typer._typing",
+    "hash": "857e937ecf94979d69f776505b3837900fb0898aee25681aec6aecea918cecf7",
+    "id": "array",
     "ignore_all": true,
-    "interface_hash": "0f3d3599045f3d24c61dcdc82fc0d7878684a5647fb9689d5be4c96189e04edc",
-    "mtime": 1685143295,
+    "interface_hash": "e74f43bcf6812ded0e30399199d4635c9bc9566bf7e4a36c46596db0efe00fdd",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -81,13 +78,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/_typing.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/array.pyi",
     "plugin_data": null,
-    "size": 19743,
+    "size": 3717,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/colors.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/colors.meta.json` & `su6-0.3.0/.mypy_cache/3.11/contextlib.meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7181481481481481%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 5), (2, 2), (3, 3), (4, 6), (5, 7), (6, 8)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(1, 5), (2, 10), (3, 5), (4, 5), (5, 5), (6, 5), (7, 5)], delete: [2, '*

 * *                '1]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (2, 'sys'), (3, '_typeshed'), (4, 'types'), "*

 * *                   "(6, 'typing_extensions'), (7, 'builtins')], delete: [0]}",*

 * * "'hash'": "'c4656ab0b855c3aed90b09036223336af2d28ce8f7b002882c0cd4971d758511'",*

 * * "'id'": "'contextlib'",*

 * * "'interface_h […]*

```diff
@@ -1,29 +1,44 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        5,
         1,
-        1,
+        2,
+        3,
+        6,
+        7,
+        8,
         1
     ],
     "dep_prios": [
         5,
-        30,
-        30
+        5,
+        10,
+        5,
+        5,
+        5,
+        5,
+        5
     ],
     "dependencies": [
-        "builtins",
+        "collections.abc",
         "abc",
-        "typing"
+        "sys",
+        "_typeshed",
+        "types",
+        "typing",
+        "typing_extensions",
+        "builtins"
     ],
-    "hash": "7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f",
-    "id": "typer.colors",
+    "hash": "c4656ab0b855c3aed90b09036223336af2d28ce8f7b002882c0cd4971d758511",
+    "id": "contextlib",
     "ignore_all": true,
-    "interface_hash": "27b284b26e724e12cf37260c1baa2dfb8b4eacd2f12a30cc5a22b69d7b95ad25",
-    "mtime": 1685143295,
+    "interface_hash": "089d84d23bdd14c45d68f871f8d4896a74017a2ad540b58c2fdf81c057f81142",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/colors.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/contextlib.pyi",
     "plugin_data": null,
-    "size": 430,
+    "size": 8986,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/completion.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/completion.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/core.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/core.meta.json` & `su6-0.3.0/.mypy_cache/3.11/errno.meta.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6813867259918428%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{delete: [24, 23, 22, 21, 20, 19, 18, 17, 16, 15, 14, 13, 12, 11, 9, 8, 7, 6, 5, '*

 * *                '4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [26, 25, 24, 23, 22, 21, 20, 18, 17, 15, 13, 12, 11, 10, 9, 8, 7, 6, 5, '*

 * *                '4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (4, 'typing')], delete: [28, 27, 26, 25, 24, "*

 * *                   '23, 21, 20, 18, 17, 16, 15, 14, 13, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'hash'": "' […]*

```diff
@@ -1,107 +1,35 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        21,
-        22,
-        23,
-        24,
-        25,
-        26,
-        28,
-        38,
-        45,
-        1,
         2,
-        3,
-        4,
-        5,
-        6,
-        20,
-        36,
-        38,
-        75,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        10,
-        10,
-        10,
-        10,
-        5,
         5,
         10,
-        20,
-        10,
-        10,
-        10,
-        10,
-        5,
-        5,
-        10,
-        10,
-        20,
-        20,
         5,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "click.core",
-        "click.formatting",
-        "click.parser",
-        "click.types",
-        "click.utils",
-        "typer.completion",
-        "typer._compat_utils",
-        "typer.rich_utils",
-        "click.shell_completion",
-        "errno",
-        "inspect",
-        "os",
+        "collections.abc",
         "sys",
-        "gettext",
-        "typing",
-        "click",
-        "rich",
-        "typer",
-        "warnings",
         "builtins",
-        "_typeshed",
-        "_warnings",
         "abc",
-        "click.exceptions",
-        "contextlib",
-        "posixpath",
-        "typer._completion_click8",
-        "types",
-        "typing_extensions"
+        "typing"
     ],
-    "hash": "4e854e1f3b38cac177e4a25af37050960cc2cdc54d10c257791d45283ac3a5a9",
-    "id": "typer.core",
+    "hash": "bd0401f598c4a64b36aec1483018fe5d595ea6c95bdead83dc5e75db0925a27c",
+    "id": "errno",
     "ignore_all": true,
-    "interface_hash": "33d5bc0ff98d72d3db1e6bf73791db31120d3dafa533c19c29166de8075ffbde",
-    "mtime": 1685143295,
+    "interface_hash": "e1e65cfbee39cc37932c3082a2d6faa8252a44c9a46d46fbf725ed1021d90fb4",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -135,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/core.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/errno.pyi",
     "plugin_data": null,
-    "size": 26545,
+    "size": 3911,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/main.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/main.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/models.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/models.meta.json` & `su6-0.3.0/.mypy_cache/3.11/os/path.meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6931776556776558%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(1, 7)], delete: [8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [10, 9, 7, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (1, 'posixpath'), (4, 'typing')], delete: [12, 11, 10, "*

 * *                   '7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'hash'": "'1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433'",*

 * * "'id'": "'os.path'",*

 * * "'interface_hash'": "'a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e'",*

 * * "'mtime'": […]*

```diff
@@ -1,59 +1,35 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        18,
-        22,
-        24,
-        25,
-        1,
-        2,
-        3,
-        16,
-        1,
         1,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        25,
-        25,
-        25,
-        10,
         10,
         5,
-        10,
         5,
         30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "typer._compat_utils",
-        "click.shell_completion",
-        "typer.core",
-        "typer.main",
-        "inspect",
-        "io",
-        "typing",
-        "click",
+        "sys",
+        "posixpath",
         "builtins",
         "abc",
-        "click.core",
-        "click.types",
-        "enum"
+        "typing"
     ],
-    "hash": "0d625201001a209a45048efff3154017d132f4d3479b8755ea29f6b81ecdeca9",
-    "id": "typer.models",
+    "hash": "1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433",
+    "id": "os.path",
     "ignore_all": true,
-    "interface_hash": "239046e43ed828fba7030bdc4119029e194d6de90d24865db4033b0bab8d21c6",
-    "mtime": 1685143295,
+    "interface_hash": "a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -87,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/models.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/path.pyi",
     "plugin_data": null,
-    "size": 15981,
+    "size": 186,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/params.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/params.meta.json` & `su6-0.3.0/.mypy_cache/3.11/weakref.meta.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6943223443223443%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(0, 13), (2, 2), (4, 12), (5, 14), (6, 15)], delete: [5, 4, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 5), (4, 5), (5, 5), (6, 5), (7, 5)], delete: [6, 5, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, '_typeshed'), (3, "*

 * *                   "'_weakref'), (4, '_weakrefset'), (6, 'typing_extensions')], delete: [7, 6, 3, "*

 * *                   '1, 0]}',*

 * * "'hash'": "'2f4d35940e2c4b0c2eb1bf2a5ba693d7594eb77431269f2de4e9683bb3f3d […]*

```diff
@@ -1,44 +1,47 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        5,
-        8,
+        13,
         1,
+        2,
         3,
-        1,
-        1,
+        12,
+        14,
+        15,
         1,
         1
     ],
     "dep_prios": [
         5,
-        25,
-        5,
         10,
         5,
-        30,
-        30,
+        5,
+        5,
+        5,
+        5,
+        5,
         30
     ],
     "dependencies": [
-        "typer.models",
-        "click.shell_completion",
+        "collections.abc",
+        "sys",
+        "_typeshed",
+        "_weakref",
+        "_weakrefset",
         "typing",
-        "click",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "click.core",
-        "click.types"
+        "abc"
     ],
-    "hash": "fcf07893bfc8bf4aa53628a147a0b9383364d9146d16d97b31bf5d993a818c4c",
-    "id": "typer.params",
+    "hash": "2f4d35940e2c4b0c2eb1bf2a5ba693d7594eb77431269f2de4e9683bb3f3d9e2",
+    "id": "weakref",
     "ignore_all": true,
-    "interface_hash": "e8e28933e640b7a78446e418ed017d302c5b8ec515ab27ca1c0cc9c2eac83b45",
-    "mtime": 1685143295,
+    "interface_hash": "13b7e4e6a79b3335dcdeae4b8f3f06a016f46d17c1fa6f02850816d065481b1a",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/params.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/weakref.pyi",
     "plugin_data": null,
-    "size": 13401,
+    "size": 6020,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/rich_utils.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/rich_utils.meta.json` & `su6-0.3.0/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/utils.data.json` & `su6-0.3.0/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/typer/utils.meta.json` & `su6-0.3.0/.mypy_cache/3.11/ctypes/wintypes.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6956776556776557%*

 * *Differences: {"'data_mtime'": '1685143683',*

 * * "'dep_lines'": '{insert: [(1, 23)], delete: [8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [10, 9, 8, 7, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'ctypes'), (4, 'typing')], delete: [12, 11, 10, 9, 8, 4, 3, 2, "*

 * *                   '1, 0]}',*

 * * "'hash'": "'defeeb073c43c6345deb22a8d25df81981445c4754febdceecfffcf2ad494435'",*

 * * "'id'": "'ctypes.wintypes'",*

 * * "'interface_hash'": "'9096eb2cb1b060b28548100a7e883a3d72ab90d909c4cd3fdbc685aefeda3c80'",*

 * * "'mtime'": '1685283 […]*

```diff
@@ -1,59 +1,35 @@
 {
-    "data_mtime": 1685143685,
+    "data_mtime": 1685143683,
     "dep_lines": [
-        7,
-        8,
-        1,
-        2,
-        3,
-        5,
-        1,
-        1,
-        1,
         1,
+        23,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        10,
-        5,
         5,
-        5,
-        5,
-        30,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "typer._typing",
-        "typer.models",
-        "inspect",
-        "copy",
-        "typing",
+        "ctypes",
         "typing_extensions",
         "builtins",
         "abc",
-        "click",
-        "click.core",
-        "click.shell_completion",
-        "click.types",
-        "types"
+        "typing"
     ],
-    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
-    "id": "typer.utils",
+    "hash": "defeeb073c43c6345deb22a8d25df81981445c4754febdceecfffcf2ad494435",
+    "id": "ctypes.wintypes",
     "ignore_all": true,
-    "interface_hash": "a2a85c807b26672ed4a26c19c9b4e841141ca67ec475f5c25733d86efba2979d",
-    "mtime": 1685143295,
+    "interface_hash": "9096eb2cb1b060b28548100a7e883a3d72ab90d909c4cd3fdbc685aefeda3c80",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -87,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/ctypes/wintypes.pyi",
     "plugin_data": null,
-    "size": 7293,
+    "size": 5284,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/urllib/__init__.data.json` & `su6-0.3.0/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/urllib/__init__.meta.json` & `su6-0.3.0/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7324074074074074%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 2), (1, 1), (2, 3), (3, 4), (4, 7)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5), (3, 5), (4, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, 'typing'), (3, "*

 * *                   "'typing_extensions'), (4, 'types'), (6, '_typeshed')], delete: [2]}",*

 * * "'hash'": "'9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1'",*

 * * "'id'": "'urllib.parse'",*

 * * "'interface_hash'": "'02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd070 […]*

```diff
@@ -1,29 +1,44 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
+        2,
+        1,
+        3,
+        4,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
+        5,
+        5,
         30,
         30
     ],
     "dependencies": [
+        "collections.abc",
+        "sys",
+        "typing",
+        "typing_extensions",
+        "types",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
-    "id": "urllib",
+    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
+    "id": "urllib.parse",
     "ignore_all": true,
-    "interface_hash": "697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3",
-    "mtime": 1685143295,
+    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
     "plugin_data": null,
-    "size": 0,
+    "size": 6532,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.mypy_cache/3.11/urllib/parse.data.json` & `su6-0.3.0/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.mypy_cache/3.11/urllib/parse.meta.json` & `su6-0.3.0/.mypy_cache/3.11/textwrap.meta.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7456481481481482%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 2)], delete: [4, 3, 2, 0]}',*

 * * "'dep_prios'": '{delete: [2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 're'), (4, 'typing')], delete: [6, 4, 3, 2, 1]}",*

 * * "'hash'": "'e9e1065949260d153ff9f03e68e2165ac7bdfb5188abc4fcf52e1569ff5a27b6'",*

 * * "'id'": "'textwrap'",*

 * * "'interface_hash'": "'29232ba58f8215dd6357b76e6f62c44a51e72d89c8e61f20e5095cce0c3941c6'",*

 * * "'mtime'": '1685283590',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/textw […]*

```diff
@@ -1,44 +1,35 @@
 {
     "data_mtime": 1685143683,
     "dep_lines": [
-        2,
         1,
-        3,
-        4,
-        7,
+        2,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "sys",
-        "typing",
-        "typing_extensions",
-        "types",
+        "re",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
-    "id": "urllib.parse",
+    "hash": "e9e1065949260d153ff9f03e68e2165ac7bdfb5188abc4fcf52e1569ff5a27b6",
+    "id": "textwrap",
     "ignore_all": true,
-    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
-    "mtime": 1685143295,
+    "interface_hash": "29232ba58f8215dd6357b76e6f62c44a51e72d89c8e61f20e5095cce0c3941c6",
+    "mtime": 1685283590,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/textwrap.pyi",
     "plugin_data": null,
-    "size": 6532,
+    "size": 3233,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.2.1/.ruff_cache/content/1f88fbdfcbf2d8d6` & `su6-0.3.0/.ruff_cache/content/1f88fbdfcbf2d8d6`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.ruff_cache/content/684d0841c18787fb` & `su6-0.3.0/.ruff_cache/content/684d0841c18787fb`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.ruff_cache/content/68c4553df91c1f5e` & `su6-0.3.0/.ruff_cache/content/68c4553df91c1f5e`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.ruff_cache/content/881c84062ed51136` & `su6-0.3.0/.ruff_cache/content/881c84062ed51136`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.ruff_cache/content/b8d965aa2b8fd993` & `su6-0.3.0/.ruff_cache/content/b8d965aa2b8fd993`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.ruff_cache/content/b990e7d90d89db2a` & `su6-0.3.0/.ruff_cache/content/b990e7d90d89db2a`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/.ruff_cache/content/be4a1815dbb4c4` & `su6-0.3.0/.ruff_cache/content/be4a1815dbb4c4`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/LICENSE.txt` & `su6-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6-0.2.1/pyproject.toml` & `su6-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -18,30 +18,58 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "black",
-    "mypy",
-    "ruff",
-    "bandit",
-    "isort",
     "typer[all]",
     "plumbum",
 ]
 
 [template.plugins.default]
 src-layout = true
 
 [project.optional-dependencies]
+all = [
+    "black",
+    "mypy",
+    "ruff",
+    "bandit",
+    "isort",
+    "pydocstyle",
+]
+
+black = [
+    "black"
+]
+
+mypy = [
+    "mypy"
+]
+
+ruff = [
+    "ruff"
+]
+
+bandit = [
+    "bandit"
+]
+
+isort = [
+    "isort"
+]
+
+pydocstyle = [
+    "pydocstyle"
+]
+
 dev = [
-  "hatch",
-  "python-semantic-release",
+    "hatch",
+    "python-semantic-release",
 ]
 
 [project.scripts]
 su6 = "su6.cli:app"
 
 [project.urls]
 Documentation = "https://github.com/robinvandernoord/su6-checker#readme"
@@ -106,14 +134,27 @@
     "B108"  # hard coded /tmp/... files are fine for me tbh
 ]
 
 [tool.isort]
 profile = "black"
 extend_skip_glob = ["*.bak/*"]
 
+[tool.pydocstyle]
+convention = "google"
+match-dir = '(?!venv)[^\.].*'
+add_select = [
+    "D213", # = Multi-line docstring summary should start at the second line
+    "D416", # = Google-style section name checks.
+    "D417", # = Missing argument descriptions in the docstring
+]
+add_ignore = [
+    "D200", # = One-line docstring should fit on one line with quotes
+    "D212", # = Multi-line docstring summary should start at the first line
+]
+
 ### and if it's a project and NOT a package, add this to make it not look for anything buildable: ###
 # make this a meta package: not a library but simply allow me to run `pip install .[dev]`
 #[build-system]
 #build-backend = "setuptools.build_meta"
 #requires = ["setuptools"]
 #
 #[tool.setuptools.packages.find]
```

