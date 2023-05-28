# Comparing `tmp/deez_py-0.1.0.tar.gz` & `tmp/deez_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deez_py-0.1.0.tar", max compression
+gzip compressed data, was "deez_py-0.1.1.tar", max compression
```

## Comparing `deez_py-0.1.0.tar` & `deez_py-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3372 2023-05-28 18:29:18.278283 deez_py-0.1.0/README.rst
--rw-r--r--   0        0        0      213 2023-05-28 18:29:18.278283 deez_py-0.1.0/deez_py/__init__.py
--rw-r--r--   0        0        0      154 2023-05-28 18:29:18.278283 deez_py-0.1.0/deez_py/__main__.py
--rw-r--r--   0        0        0     8141 2023-05-28 18:18:15.690579 deez_py-0.1.0/deez_py/lexer.py
--rw-r--r--   0        0        0      674 2023-05-28 17:56:42.794879 deez_py-0.1.0/deez_py/tokens.py
--rw-r--r--   0        0        0     1333 2023-05-28 18:29:31.654358 deez_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4250 1970-01-01 00:00:00.000000 deez_py-0.1.0/setup.py
--rw-r--r--   0        0        0     4412 1970-01-01 00:00:00.000000 deez_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3372 2023-05-28 18:31:22.334973 deez_py-0.1.1/README.rst
+-rw-r--r--   0        0        0      213 2023-05-28 18:32:20.087294 deez_py-0.1.1/deez_py/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-28 18:29:18.278283 deez_py-0.1.1/deez_py/__main__.py
+-rw-r--r--   0        0        0     8141 2023-05-28 18:18:15.690579 deez_py-0.1.1/deez_py/lexer.py
+-rw-r--r--   0        0        0      674 2023-05-28 17:56:42.794879 deez_py-0.1.1/deez_py/tokens.py
+-rw-r--r--   0        0        0     1333 2023-05-28 18:33:10.255573 deez_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4250 1970-01-01 00:00:00.000000 deez_py-0.1.1/setup.py
+-rw-r--r--   0        0        0     4412 1970-01-01 00:00:00.000000 deez_py-0.1.1/PKG-INFO
```

### Comparing `deez_py-0.1.0/README.rst` & `deez_py-0.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 🚨 Installation
 ---------------
 
 With :code:`pip`:
 
 .. code-block:: console
 
-   python3 -m pip install deez_py
+   python3 -m pip install deez-py
 
 
 🚸 Usage
 --------
 
 .. code-block:: python3
```

### Comparing `deez_py-0.1.0/deez_py/lexer.py` & `deez_py-0.1.1/deez_py/lexer.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.0/deez_py/tokens.py` & `deez_py-0.1.1/deez_py/tokens.py`

 * *Files identical despite different names*

### Comparing `deez_py-0.1.0/pyproject.toml` & `deez_py-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deez_py"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities."
 authors = [
     "Mahmoud Harmouch <business@wiseai.dev>",
     "BatikanHyt <batikanhyt@gmail.com>",
     "ThePrimeagen <the.primeagen@gmail.com>"
 ]
 license = "GNU General Public License v3.0"
```

### Comparing `deez_py-0.1.0/setup.py` & `deez_py-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 ['deez_py']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'deez-py',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities.',
-    'long_description': '=========\ndeez_py\n=========\n\n.. image:: https://img.shields.io/badge/License-GPLv3-blue.svg\n   :target: https://github.com/ThePrimeagen/ts-rust-zig-deez_py/tree/master/python/LICENSE\n   :alt: License\n\n.. image:: https://img.shields.io/pypi/v/deez_py.svg\n   :target: https://pypi.org/project/deez_py/\n   :alt: pypi version\n\n**deez_py** is a Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities.\n\n🛠️ Requirements\n---------------\n\n**deez_py** requires Python 3.9 or above.\n\nTo install Python 3.9, I recommend using `pyenv`_.\n\n.. code-block:: bash\n\n   # install pyenv\n   git clone https://github.com/pyenv/pyenv ~/.pyenv\n\n   # setup pyenv (you should also put these three lines in .bashrc or similar)\n   # if you are using zsh\n   cat << EOF >> ~/.zshrc\n   # pyenv config\n   export PATH="${HOME}/.pyenv/bin:${PATH}"\n   export PYENV_ROOT="${HOME}/.pyenv"\n   eval "$(pyenv init -)"\n   EOF\n\n   # or if you using the default bash shell, do this instead:\n   cat << EOF >> ~/.bashrc\n   # pyenv config\n   export PATH="${HOME}/.pyenv/bin:${PATH}"\n   export PYENV_ROOT="${HOME}/.pyenv"\n   eval "$(pyenv init -)"\n   EOF\n   # Close and open a new shell session\n   # install Python 3.9.10\n   pyenv install 3.9.10\n\n   # make it available globally\n   pyenv global system 3.9.10\n\n\nTo manage the Python 3.9 virtualenv, I recommend using `poetry`_.\n\n.. code-block:: bash\n\n   # install poetry\n   curl -sSL https://install.python-poetry.org | python3 -\n   poetry --version\n   Poetry version 1.1.13\n\n   # Having the python executable in your PATH, you can use it:\n   poetry env use 3.9.10\n\n   # However, you are most likely to get the following issue:\n   Creating virtualenv deez_py-dxc671ba-py3.9 in ~/.cache/pypoetry/virtualenvs\n\n   ModuleNotFoundError\n\n   No module named \'virtualenv.seed.via_app_data\'\n\n   at <frozen importlib._bootstrap>:973 in _find_and_load_unlocked\n\n   # To resolve it, you need to reinstall virtualenv through pip\n   sudo apt remove --purge python3-virtualenv virtualenv\n   python3 -m pip install -U virtualenv\n\n   # Now, you can just use the minor Python version in this case:\n   poetry env use 3.9.10\n   Using virtualenv: ~/.cache/pypoetry/virtualenvs/deez_py-dxc671ba-py3.9\n\n\n🚨 Installation\n---------------\n\nWith :code:`pip`:\n\n.. code-block:: console\n\n   python3 -m pip install deez_py\n\n\n🚸 Usage\n--------\n\n.. code-block:: python3\n\n   >>> from deez_py import Lexer\n   >>> lex = Lexer(\'=+(){},;\')\n   >>> for _ in range(9):\n   >>>     print(lex.get_next_token())\n   ... \n   Token(type=<TokenType.Equal: \'=\'>, literal=\'=\')\n   Token(type=<TokenType.Plus: \'+\'>, literal=\'+\')\n   Token(type=<TokenType.LParen: \'(\'>, literal=\'(\')\n   Token(type=<TokenType.RParen: \')\'>, literal=\')\')\n   Token(type=<TokenType.LSquirly: \'{\'>, literal=\'{\')\n   Token(type=<TokenType.RSquirly: \'}\'>, literal=\'}\')\n   Token(type=<TokenType.Comma: \',\'>, literal=\',\')\n   Token(type=<TokenType.Semicolon: \';\'>, literal=\';\')\n   Token(type=<TokenType.Eof: \'EOF\'>, literal=\'EOF\')\n\n📝 License\n----------\n\nThis program and the accompanying materials are made available under the terms and conditions of the `GNU GENERAL PUBLIC LICENSE`_.\n\n.. _GNU GENERAL PUBLIC LICENSE: http://www.gnu.org/licenses/\n.. _deez_py: https://pypi.org/project/deez_py/\n.. _pyenv: https://github.com/pyenv/pyenv\n.. _poetry: https://github.com/python-poetry/poetry\n',
+    'long_description': '=========\ndeez_py\n=========\n\n.. image:: https://img.shields.io/badge/License-GPLv3-blue.svg\n   :target: https://github.com/ThePrimeagen/ts-rust-zig-deez_py/tree/master/python/LICENSE\n   :alt: License\n\n.. image:: https://img.shields.io/pypi/v/deez_py.svg\n   :target: https://pypi.org/project/deez_py/\n   :alt: pypi version\n\n**deez_py** is a Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities.\n\n🛠️ Requirements\n---------------\n\n**deez_py** requires Python 3.9 or above.\n\nTo install Python 3.9, I recommend using `pyenv`_.\n\n.. code-block:: bash\n\n   # install pyenv\n   git clone https://github.com/pyenv/pyenv ~/.pyenv\n\n   # setup pyenv (you should also put these three lines in .bashrc or similar)\n   # if you are using zsh\n   cat << EOF >> ~/.zshrc\n   # pyenv config\n   export PATH="${HOME}/.pyenv/bin:${PATH}"\n   export PYENV_ROOT="${HOME}/.pyenv"\n   eval "$(pyenv init -)"\n   EOF\n\n   # or if you using the default bash shell, do this instead:\n   cat << EOF >> ~/.bashrc\n   # pyenv config\n   export PATH="${HOME}/.pyenv/bin:${PATH}"\n   export PYENV_ROOT="${HOME}/.pyenv"\n   eval "$(pyenv init -)"\n   EOF\n   # Close and open a new shell session\n   # install Python 3.9.10\n   pyenv install 3.9.10\n\n   # make it available globally\n   pyenv global system 3.9.10\n\n\nTo manage the Python 3.9 virtualenv, I recommend using `poetry`_.\n\n.. code-block:: bash\n\n   # install poetry\n   curl -sSL https://install.python-poetry.org | python3 -\n   poetry --version\n   Poetry version 1.1.13\n\n   # Having the python executable in your PATH, you can use it:\n   poetry env use 3.9.10\n\n   # However, you are most likely to get the following issue:\n   Creating virtualenv deez_py-dxc671ba-py3.9 in ~/.cache/pypoetry/virtualenvs\n\n   ModuleNotFoundError\n\n   No module named \'virtualenv.seed.via_app_data\'\n\n   at <frozen importlib._bootstrap>:973 in _find_and_load_unlocked\n\n   # To resolve it, you need to reinstall virtualenv through pip\n   sudo apt remove --purge python3-virtualenv virtualenv\n   python3 -m pip install -U virtualenv\n\n   # Now, you can just use the minor Python version in this case:\n   poetry env use 3.9.10\n   Using virtualenv: ~/.cache/pypoetry/virtualenvs/deez_py-dxc671ba-py3.9\n\n\n🚨 Installation\n---------------\n\nWith :code:`pip`:\n\n.. code-block:: console\n\n   python3 -m pip install deez-py\n\n\n🚸 Usage\n--------\n\n.. code-block:: python3\n\n   >>> from deez_py import Lexer\n   >>> lex = Lexer(\'=+(){},;\')\n   >>> for _ in range(9):\n   >>>     print(lex.get_next_token())\n   ... \n   Token(type=<TokenType.Equal: \'=\'>, literal=\'=\')\n   Token(type=<TokenType.Plus: \'+\'>, literal=\'+\')\n   Token(type=<TokenType.LParen: \'(\'>, literal=\'(\')\n   Token(type=<TokenType.RParen: \')\'>, literal=\')\')\n   Token(type=<TokenType.LSquirly: \'{\'>, literal=\'{\')\n   Token(type=<TokenType.RSquirly: \'}\'>, literal=\'}\')\n   Token(type=<TokenType.Comma: \',\'>, literal=\',\')\n   Token(type=<TokenType.Semicolon: \';\'>, literal=\';\')\n   Token(type=<TokenType.Eof: \'EOF\'>, literal=\'EOF\')\n\n📝 License\n----------\n\nThis program and the accompanying materials are made available under the terms and conditions of the `GNU GENERAL PUBLIC LICENSE`_.\n\n.. _GNU GENERAL PUBLIC LICENSE: http://www.gnu.org/licenses/\n.. _deez_py: https://pypi.org/project/deez_py/\n.. _pyenv: https://github.com/pyenv/pyenv\n.. _poetry: https://github.com/python-poetry/poetry\n',
     'author': 'Mahmoud Harmouch',
     'author_email': 'business@wiseai.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ThePrimeagen/ts-rust-zig-deez_py',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `deez_py-0.1.0/PKG-INFO` & `deez_py-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deez-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python implementation of a lexical analyzer that provides comprehensive scanning, and lookahead capabilities.
 Home-page: https://github.com/ThePrimeagen/ts-rust-zig-deez_py
 License: GNU General Public License v3.0
 Keywords: python,deez_py,lexer
 Author: Mahmoud Harmouch
 Author-email: business@wiseai.dev
 Requires-Python: >=3.9,<4.0
@@ -105,15 +105,15 @@
 🚨 Installation
 ---------------
 
 With :code:`pip`:
 
 .. code-block:: console
 
-   python3 -m pip install deez_py
+   python3 -m pip install deez-py
 
 
 🚸 Usage
 --------
 
 .. code-block:: python3
```

